# Retention Cohorts Analysis

**Programa Reforge**: Retention & Engagement

## O que é Cohort Retention Analysis

Análise de cohort é a metodologia de **agrupar usuários por data de entrada** (ou outro atributo) e rastrear seu comportamento ao longo do tempo, especialmente **retenção**.

### Por que Cohorts importam

**Problema com métricas agregadas**:
- "100 usuários ativos" não diz se são os mesmos ou diferentes
- Crescimento pode mascarar churn alto
- Impossível ver padrões de retenção

**Cohort Analysis resolve**:
- Mostra **retenção real** ao longo do tempo
- Identifica quando usuários churnam (D1? D7? M3?)
- Permite comparar cohorts (mês A melhor que mês B?)
- Valida se mudanças de produto melhoraram retenção

## Tipos de Retenção

### 1. Unbounded Retention (Classic Retention)

**Definição**: % de usuários que retornam **pelo menos uma vez** após período X

**Fórmula**:
```
D7 Retention = (Usuários ativos D7+) / (Total usuários no cohort)
```

"D7+" significa D7, D8, D9... qualquer dia após D7.

**Quando usar**:
- Apps sociais, messaging, consumo de conteúdo
- Produtos onde uso frequente é esperado

**Exemplo (Instagram)**:
- 100 users signup dia 0
- D7: 70 users abrem o app pelo menos uma vez entre D7-D14
- D7 Retention = 70%

**Curva típica**:
```
100% ┤
     │●
  80%│  ●
     │    ●
  60%│      ●
     │        ●──●──●──●  (plateau)
  40%│
     └───────────────────────
     D1  D7  D14 D30 D60 D90
```

Curva é **decrescente** e eventualmente **estabiliza** (core retained users).

### 2. Bounded Retention (N-Day Retention)

**Definição**: % de usuários que retornam **exatamente** no período X

**Fórmula**:
```
D7 Bounded Retention = (Usuários ativos apenas em D7) / (Total usuários)
```

**Quando usar**:
- Apps transacionais (e-commerce, food delivery)
- Uso é periódico, não diário

**Exemplo (DoorDash)**:
- 100 users fazem primeira ordem dia 0
- Week 4: 30 users fazem ordem exatamente na semana 4
- W4 Bounded Retention = 30%

**Curva típica**:
```
100% ┤
     │●
  50%│  ●
     │    ●
  30%│      ●──●──●──●  (plateau)
     │
  10%│
     └───────────────────────
     W1  W4  W8  W12 W16 W20
```

Curva também decresce mas **plateau é a retention natural** (frequência de uso).

### 3. Smile Graph (Retention Curve)

**O que é**: Curva de retenção onde usuários inicialmente churnam, depois retention **sobe**

**Formato**:
```
  60%┤                    ╱●
     │                  ╱
  40%│                ╱
     │              ╱
  20%│●──●──●────●╱  (dip, depois sobe)
     └───────────────────────
     D1  D7  D30 D90 D180
```

**Por que acontece**:
- Usuários iniciais são **experimentadores** (low intent, alta churn)
- Usuários que ficam 30+ dias são **committed** (high intent, baixa churn)
- Produto tem curva de aprendizado, valor aumenta com tempo

**Exemplos**:
- **B2B SaaS**: Trial users churnam, paying customers ficam
- **Gaming**: Casual gamers saem, hardcore gamers ficam e intensificam
- **Marketplaces**: Browsers saem, transactors ficam

**Implicação**: Focar em levar users até o ponto onde curva sobe (ativação crítica).

## Como Construir Cohort Table

### Estrutura Básica

**Formato clássico**:

| Cohort  | M0   | M1   | M2   | M3   | M6   | M12  |
|---------|------|------|------|------|------|------|
| Jan 24  | 100% | 65%  | 52%  | 45%  | 38%  | 32%  |
| Feb 24  | 100% | 68%  | 55%  | 48%  | 40%  | -    |
| Mar 24  | 100% | 70%  | 58%  | 50%  | -    | -    |
| Apr 24  | 100% | 72%  | 60%  | -    | -    | -    |
| May 24  | 100% | 75%  | -    | -    | -    | -    |

**Como ler**:
- **Linhas**: Cada cohort (mês de signup)
- **Colunas**: Períodos após signup (M0 = mês de entrada, M1 = 1 mês depois)
- **Células**: % de usuários do cohort que estão ativos naquele período
- **Diagonal**: Cohorts mais recentes têm menos dados

### Métricas para Rastrear

**Além de retention %**, rastrear:

1. **Cohort Size**: Quantos usuários no cohort
   - Permite ponderar (cohort de 10 users não é significativo)

2. **Absolute Retained Users**: # absoluto de users retidos
   - 50% de 100 = 50 users vs. 50% de 10 = 5 users

3. **Revenue Retention**: % de MRR retido (para SaaS)
   - Pode ser > 100% (expansão > churn)

4. **Feature Adoption**: % que usa feature X em cada período
   - Correlaciona feature uso com retention

## Padrões de Retenção e Diagnósticos

### Padrão 1: Queda Acentuada em D1-D7 (Early Drop)

**Curva**:
```
100%│●
  60%│  ●
  40%│    ●
  30%│      ●──●──●
     └─────────────
     D0  D1  D7  D30
```

**Diagnóstico**: Problema de **onboarding/ativação**
- Users não têm "aha moment" rápido
- Produto é confuso ou difícil de usar
- Value proposition não é clara

**Soluções**:
1. Reduzir time-to-value (TTV)
2. Onboarding guiado (tooltips, checklist)
3. Quick wins (mostrar valor imediato)
4. Better expectation setting (marketing → produto)

### Padrão 2: Queda Gradual Contínua (Slow Bleed)

**Curva**:
```
100%│●
  80%│  ●
  60%│    ●
  40%│      ●
  20%│        ●
     └─────────────
     D0  D7  D30 D90
```

**Diagnóstico**: Problema de **core value ou substitute**
- Produto não resolve problema bem o suficiente
- Alternativa melhor existe
- Necessidade não é frequente

**Soluções**:
1. Aprofundar core value (fazer o principal ainda melhor)
2. Adicionar features que aumentam stickiness
3. Criar habit loops (triggers, reminders)
4. Aumentar switching cost (integrations, data lock-in)

### Padrão 3: Queda em Mês 3-6 (Mid-Term Churn)

**Curva**:
```
100%│●
  70%│  ●──●
  50%│        ●
  30%│          ●──●
     └─────────────────
     M0  M1  M3  M6  M12
```

**Diagnóstico**: Problema de **lack of depth ou expansion**
- Usuário esgotou use cases iniciais
- Produto não evoluiu com necessidade
- Falta de features avançadas

**Soluções**:
1. Feature adoption (mostrar advanced features)
2. New use cases (educação, templates)
3. Upsell para tier superior (mais value)
4. Customer success proativo (check-ins)

### Padrão 4: Cohorts Melhorando (Good Signal!)

**Curva**:
```
100%│● ● ● ●  (múltiplos cohorts)
  70%│  ●╱●╱●╱● (cohorts recentes melhores)
  50%│    ●╱
  30%│      ●
     └─────────────────
     M0  M1  M3  M6  M12
```

**Diagnóstico**: Produto está **melhorando!**
- Changes de produto estão funcionando
- Onboarding melhorou
- Product-market fit aumentando

**Ação**: Identifique **o que mudou** entre cohorts e duplique

### Padrão 5: Cohorts Piorando (Red Flag!)

**Curva**:
```
100%│● ● ● ●  (múltiplos cohorts)
  70%│  ●╲●╲●╲● (cohorts recentes piores)
  50%│    ●╲
  30%│      ●
     └─────────────────
     M0  M1  M3  M6  M12
```

**Diagnóstico**: Algo **quebrou** ou **qualidade caiu**
- Bugs introduzidos
- Aquisição de lower-quality users
- Competidor melhor surgiu

**Ação urgente**: Diagnosticar causa e reverter

## Benchmarks de Retenção

### B2C Social/Content

**D1 Retention**: 40-60%
**D7 Retention**: 20-35%
**D30 Retention**: 10-20%

**Exemplos**:
- Instagram: D1 ~50%, D7 ~30%
- TikTok: D1 ~55%, D7 ~40% (muito alta!)
- Twitter: D1 ~40%, D7 ~15%

### B2C SaaS/Subscription

**M1 Retention**: 60-80%
**M3 Retention**: 50-70%
**M12 Retention**: 40-60%

**Churn mensal**: 3-7%

### B2B SMB SaaS

**M1 Retention**: 85-95%
**M3 Retention**: 75-85%
**M12 Retention**: 60-75%

**Churn mensal**: 2-5%

### B2B Enterprise SaaS

**M1 Retention**: 95%+
**M3 Retention**: 90%+
**M12 Retention**: 80-90%

**Churn anual**: 5-15%

### E-commerce/Marketplace

**M1 Bounded Retention**: 20-40%
**M3 Bounded Retention**: 15-25%
**M12 Bounded Retention**: 10-20%

(Uso periódico, não diário)

## Análises Avançadas

### 1. Segmentação de Cohorts

**Por canal de aquisição**:
| Cohort       | D7 Ret | D30 Ret |
|--------------|--------|---------|
| Organic      | 45%    | 28%     | ⭐ Melhor
| Paid (FB)    | 30%    | 15%     |
| Referral     | 60%    | 40%     | ⭐⭐ Melhor!
| Partnerships | 38%    | 22%     |

**Insight**: Priorizar canais com melhor retention (não apenas volume).

**Por feature adotada**:
| Cohort                  | M3 Ret |
|-------------------------|--------|
| Usou Feature A          | 75%    | ⭐
| Não usou Feature A      | 40%    |

**Insight**: Feature A é crítica para retenção → força adoção em onboarding.

**Por ICP (Ideal Customer Profile)**:
| Cohort             | M12 Ret |
|--------------------|---------|
| ICP Match (High)   | 80%     | ⭐
| ICP Match (Medium) | 60%     |
| ICP Match (Low)    | 35%     |

**Insight**: Focar aquisição em High ICP match.

### 2. Revenue Retention (para SaaS)

**Gross Revenue Retention (GRR)**:
```
GRR = (MRR início - MRR churned - MRR contraction) / MRR início
```

**Net Revenue Retention (NRR)**:
```
NRR = (MRR início - churn - contraction + expansion) / MRR início
```

**Exemplo**:
- Cohort Jan 24: $100k MRR início
- M12: $10k churned, $5k contraction, $30k expansion
- GRR = ($100k - $10k - $5k) / $100k = 85%
- NRR = ($100k - $10k - $5k + $30k) / $100k = 115% ⭐

**Benchmarks SaaS**:
- **GRR > 90%**: Excelente (low churn)
- **NRR > 110%**: Excelente (expansion > churn)
- **NRR > 120%**: World-class

### 3. Survival Analysis (Kaplan-Meier)

**O que é**: Análise estatística que estima **média de tempo até churn**

**Output**: "Median Retention Time = 180 dias"

**Quando usar**:
- Prever LTV
- Entender "half-life" do produto
- Comparar grupos (ex: users de Feature A vs. B)

**Ferramenta**: Python (lifelines library), R, ou built-in em Amplitude/Mixpanel

## Como Usar Cohorts para Tomada de Decisão

### Use Case 1: Priorizar Roadmap

**Pergunta**: Feature A (melhorar search) ou Feature B (social sharing)?

**Análise**:
1. Cohort de usuários que usaram search avançado → 80% M3 retention
2. Cohort de usuários que compartilharam → 90% M3 retention

**Decisão**: Priorizar Feature B (social) - maior impacto em retenção.

### Use Case 2: Validar Mudança de Produto

**Cenário**: Lançamos novo onboarding em março

**Análise**:
| Cohort  | D7 Ret |
|---------|--------|
| Jan 24  | 25%    |
| Feb 24  | 27%    |
| Mar 24  | 35%    | ⭐ Novo onboarding
| Apr 24  | 37%    |

**Conclusão**: Novo onboarding funcionou (+10pp D7 retention)!

### Use Case 3: Detectar Problema Cedo

**Monitoramento semanal**:
- Cohort Week 15: D7 retention = 30% ✅
- Cohort Week 16: D7 retention = 22% ⚠️

**Ação**: Investigar imediatamente (bug? change de produto? marketing ruim?)

## Ferramentas e Implementação

**Ferramentas de Analytics**:
- **Amplitude**: Cohort analysis nativo, excelente UX
- **Mixpanel**: Retention reports built-in
- **Heap**: Auto-capture, fácil setup
- **Metabase/Looker**: Custom SQL para cohorts

**Query SQL Básico (PostgreSQL)**:

```sql
WITH cohorts AS (
  SELECT
    user_id,
    DATE_TRUNC('month', signup_date) AS cohort_month
  FROM users
),
activity AS (
  SELECT
    user_id,
    DATE_TRUNC('month', activity_date) AS activity_month
  FROM user_activity
)
SELECT
  c.cohort_month,
  a.activity_month,
  COUNT(DISTINCT a.user_id) AS active_users,
  COUNT(DISTINCT c.user_id) AS cohort_size,
  ROUND(100.0 * COUNT(DISTINCT a.user_id) / COUNT(DISTINCT c.user_id), 2) AS retention_pct
FROM cohorts c
LEFT JOIN activity a ON c.user_id = a.user_id
GROUP BY c.cohort_month, a.activity_month
ORDER BY c.cohort_month, a.activity_month;
```

## Checklist de Análise de Retention

**Toda empresa deve**:
- [ ] Ter cohort table para user retention (mensal no mínimo)
- [ ] Rastrear D1, D7, D30 retention (produtos daily use)
- [ ] Rastrear M1, M3, M12 retention (produtos subscription)
- [ ] Segmentar cohorts por canal, feature, ICP
- [ ] Comparar cohorts mês a mês (melhorando ou piorando?)
- [ ] Ter dashboard de retention visível para todo time
- [ ] Revisar retention em reviews/retros
- [ ] Conectar retention com revenue (LTV)
- [ ] Identificar padrão de curva (onde churn acontece?)
- [ ] Ter plano de ação para melhorar retention

---

**Retention é a métrica mais honesta. Crescimento sem retention é crescimento falso.** 📊
