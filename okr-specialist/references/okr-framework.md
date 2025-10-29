# OKR Framework Completo

Guia completo sobre o framework OKR (Objectives and Key Results), cobrindo história, conceitos fundamentais, filosofia e metodologia.

---

## 📜 História dos OKRs

### Origem: Intel (1970s)

**Andy Grove**, CEO da Intel, criou o conceito de OKRs nos anos 1970 baseado no sistema MBO (Management by Objectives) de Peter Drucker.

**Problema que Andy Grove queria resolver**:
- Intel estava crescendo rapidamente
- Times trabalhavam em silos
- Falta de alinhamento estratégico
- Dificuldade de priorizar o que realmente importava

**Solução: iMBOs (Intel Management by Objectives)**:
```
"I will _______ (Objective)
as measured by _______ (Key Results)"
```

**Exemplo histórico da Intel (1980)**:
```
O: Dominar o mercado de microprocessadores de 8 bits
  KR1: Alcançar 2000 design wins
  KR2: Atingir 25% market share
  KR3: Lançar 8086 no prazo (Q2 1980)
```

---

### Popularização: Google (1999)

**John Doerr**, investidor do Kleiner Perkins (ex-Intel), introduziu OKRs para Google quando a empresa tinha apenas 40 funcionários.

**Por que Google adotou OKRs**:
- Estava crescendo rapidamente (de 40 para 500+ pessoas em 1 ano)
- Precisava manter alinhamento sem burocracia
- Cultura de transparência e ambição

**Primeiros OKRs do Google (1999)**:
```
O: Construir um mecanismo de busca de classe mundial
  KR1: Crawl 1 bilhão de URLs até fim do ano
  KR2: Alcançar 10 milhões de queries por dia
  KR3: Atingir latência média <0.5 segundos
```

**Impacto**:
- Google usou OKRs para crescer de 40 para 100.000+ funcionários
- Larry Page: "OKRs nos ajudaram a crescer 10x, múltiplas vezes"
- Tornou-se case de sucesso global

---

### Adoção no Vale do Silício (2000s-2010s)

Empresas que adotaram OKRs:
- **LinkedIn** (2010s): Escalar de 500 para 10.000+ funcionários
- **Twitter** (2012): Alinhar produto pós-IPO
- **Uber** (2013): Coordenar hiper-crescimento global
- **Airbnb** (2015): Focar após expansão global
- **Dropbox, Spotify, Netflix** (2010s): Manter cultura de execução

**Livro "Measure What Matters" (2018)**:
John Doerr publicou o livro que popularizou OKRs globalmente, com cases de Google, Intel, Gates Foundation, Bono (U2), e outros.

---

## 🎯 Conceitos Fundamentais

### O que é um OKR?

```
OKR = Objective + Key Results

OBJECTIVE (O QUÊ)
- Qualitativo
- Inspirador
- Desafiador
- Time-bound

KEY RESULTS (COMO MEDIR)
- Quantitativo
- Mensurável
- Verificável
- Com número/métrica
```

### Anatomia de um OKR

```
OBJECTIVE: Tornar-se a plataforma líder de CRM para PMEs no Brasil
         └─ Qualitativo, inspirador, ambicioso

  KR1: Crescer de 50 para 200 clientes pagantes
       └─ Métrica clara: clientes pagantes

  KR2: Atingir NPS de 60+
       └─ Métrica clara: NPS

  KR3: Alcançar brand awareness de 40% no segmento PME
       └─ Métrica clara: brand awareness %
```

---

### Diferença: Objective vs Key Result

| Aspecto | Objective | Key Result |
|---------|-----------|------------|
| Tipo | Qualitativo | Quantitativo |
| Inspiração | Alto | Neutro |
| Mensurabilidade | Subjetivo | 100% mensurável |
| Exemplo | "Dominar o mercado" | "Atingir 40% market share" |
| Pergunta | "O que queremos?" | "Como medimos progresso?" |

**Regra simples**:
- Se tem número → Key Result
- Se não tem número → Objective

---

### OKRs vs Outras Metodologias

#### OKRs vs KPIs

| OKR | KPI |
|-----|-----|
| Ambicioso (stretch goal) | Estável (BAU - business as usual) |
| Mudança desejada | Saúde operacional |
| Temporário (trimestral) | Contínuo (sempre monitorado) |
| Score esperado: 60-70% | Target: 100% |

**Exemplo**:
```
KPI: Manter uptime de 99.9% (operacional, contínuo)
OKR: Reduzir P95 latency de 500ms para 100ms (mudança, ambicioso)
```

#### OKRs vs Metas de Performance

| OKR | Meta de Performance |
|-----|---------------------|
| Alinhamento de time/empresa | Avaliação individual |
| Público e transparente | Privado (entre gestor e IC) |
| Stretch goal (espera-se 60-70%) | Deve ser 100% atingido |
| Não afeta bônus diretamente | Afeta bônus/promoção |

**Regra de Ouro**: **Nunca vincule OKRs a performance review individual**. Isso cria incentivos para sandbagging (metas conservadoras).

#### OKRs vs Projetos/Roadmap

| OKR | Projeto/Roadmap |
|-----|-----------------|
| Outcome (resultado de negócio) | Output (entrega) |
| "Aumentar engagement 50%" | "Lançar feature de notificações" |
| Flexível (caminho pode mudar) | Fixo (escopo definido) |
| Medido por impacto | Medido por conclusão |

**Exemplo**:
```
❌ OKR ruim (é projeto):
KR: Lançar feature de relatórios

✅ OKR bom (é outcome):
KR: Aumentar % de usuários que tomam decisões baseadas em dados de 20% para 50%
   └─ Feature de relatórios é UMA das formas de atingir isso
```

---

## 🧬 Filosofia do OKR

### Princípio 1: Outcomes, não Outputs

**Output**: O que você entrega (features, projetos, tasks)
**Outcome**: O resultado de negócio que você gera (valor, impacto, mudança)

```
❌ Output thinking:
KR1: Lançar 5 novas features
KR2: Fazer 20 entrevistas com clientes
KR3: Redesenhar homepage

✅ Outcome thinking:
KR1: Aumentar engagement (DAU/MAU) de 25% para 45%
KR2: Reduzir churn de 8% para 3%
KR3: Aumentar conversion rate de 2% para 5%
```

**Por que outcomes importam**:
- Outputs não garantem valor (você pode entregar feature que ninguém usa)
- Outcomes forçam foco em impacto real
- Permite flexibilidade no "como" atingir

---

### Princípio 2: Ambição (Stretch Goals)

**OKRs não são promessas, são aspirações**.

```
Score esperado ao definir OKR: 0.6-0.7 (60-70%)

Se você tem 100% de certeza de atingir → Não é OKR, é BAU
Se você tem 30% de certeza → Pode ser moonshot demais
Se você tem 60-70% de certeza → Sweet spot ✅
```

**Por que stretch goals**:
- Forçam pensamento não-linear (não apenas +10% do ano passado)
- Evitam complacência
- Motivam inovação e criatividade

**Exemplo**:
```
Situação atual: 100 clientes, crescendo ~10%/trimestre

❌ OKR conservador:
KR: Crescer de 100 para 110 clientes (+10%)
└─ Apenas continuando o que já funciona

✅ OKR ambicioso:
KR: Crescer de 100 para 200 clientes (+100%)
└─ Força time a testar canais novos, otimizar funil, etc.
```

---

### Princípio 3: Alinhamento e Transparência

**OKRs são públicos**. Todo mundo vê os OKRs de todo mundo.

#### Por que transparência?

1. **Alinhamento vertical** (top-down):
```
CEO OKRs
  ↓ [cascata]
VP Product OKRs
  ↓ [cascata]
PM OKRs
```

2. **Alinhamento horizontal** (cross-functional):
```
Product → vê OKRs de → Sales
Engineering → vê OKRs de → Marketing
```

3. **Evita silos**:
- Times sabem no que outros estão trabalhando
- Facilitam colaboração
- Identificam dependências cedo

**Exemplo de transparência na prática**:
```
Google: Todo funcionário pode ver OKRs do CEO no intranet
Resultado: Clareza de prioridades, alinhamento, accountability
```

---

### Princípio 4: Foco (Menos é Mais)

**Regra de Foco**:
```
3-5 Objectives (não mais)
3-5 Key Results por Objective (não mais)
Total: 9-25 Key Results

❌ Evite: 10 Objectives, 50 Key Results
└─ Time fica disperso, nada é prioridade
```

**Por que focar**:
- Atenção é recurso escasso
- Fazer 3 coisas bem > fazer 10 coisas mal
- Priorização forçada revela o que realmente importa

**Como priorizar** (quando tiver muitos OKRs candidatos):
1. Ordene por impacto esperado
2. Pergunte: "Se só pudéssemos fazer 3 coisas, quais seriam?"
3. Corte o resto (ou deixe como "aspirational OKRs")

---

### Princípio 5: Desacoplamento de Performance Review

**OKRs NÃO devem afetar avaliação individual diretamente**.

#### Por que desacoplar?

**Problema do coupling**:
```
Se OKR afeta bônus/promoção:
  → Incentiva sandbagging (metas conservadoras)
  → Pessoas evitam stretch goals
  → OKRs viram negociação política
  → Perde-se a ambição
```

**Solução**:
```
OKR = Ferramenta de alinhamento e foco (time/empresa)
Performance Review = Avaliação individual (1:1 com gestor)

Avalia-se:
✅ Contribuição para OKRs do time (esforço, qualidade)
❌ Score final do OKR (0.0-1.0)
```

**Exemplo**:
```
Situação: Time teve OKR ambicioso, score final foi 0.4

❌ Ruim: Todos recebem avaliação ruim por score baixo
✅ Bom: Avalia-se:
  - Pessoa X teve excelente contribuição, apesar do score baixo
  - Pessoa Y não se engajou, mesmo com OKR ambicioso
```

---

## 🏗️ Estrutura de OKRs

### Níveis de OKRs

```
1. COMPANY OKRs (Estratégico)
   - Definido por: CEO + Leadership Team
   - Ciclo: Trimestral (às vezes Anual para visão)
   - Quantidade: 3-5 Objectives

2. TEAM OKRs (Tático)
   - Definido por: Head de área + Time
   - Ciclo: Trimestral
   - Alinhamento: 60% com Company, 40% bottom-up
   - Quantidade: 3-5 Objectives

3. INDIVIDUAL OKRs (Execução) [Opcional]
   - Definido por: IC + Manager
   - Ciclo: Trimestral
   - Alinhamento: Contribui para ≥1 Team OKR
   - Quantidade: 3-5 Objectives
```

---

### Cascata de OKRs (Alignment)

#### Exemplo completo de cascata:

```
COMPANY (Q1 2024)
├─ O1: Atingir product-market fit comprovado
│   ├─ KR1: Crescer MRR de R$100k para R$300k
│   ├─ KR2: Atingir NPS de 50+
│   └─ KR3: Alcançar retention rate 90%+ (mês a mês)
│
└─ O2: Construir brand reconhecida no segmento PME
    ├─ KR1: Atingir 40% brand awareness (pesquisa)
    ├─ KR2: Gerar 10.000 MQLs orgânicos
    └─ KR3: Aparecer em top 3 de Google para [keyword]

────────────────────────────────────────────────

TEAM - PRODUCT (Q1 2024)
├─ O1: Criar produto que gera valor recorrente
│   ├─ KR1: Aumentar DAU/MAU de 20% para 40%
│   │   └─ [Contribui para Company O1.KR3 - retention]
│   ├─ KR2: 70% dos usuários usando ≥3 features core
│   │   └─ [Contribui para Company O1.KR2 - NPS]
│   └─ KR3: Reduzir time-to-value de 7 para 2 dias
│       └─ [Contribui para Company O1.KR3 - retention]
│
└─ O2: Descobrir próxima onda de valor (bottom-up)
    ├─ KR1: Validar 3 hipóteses de features com usuários
    ├─ KR2: Lançar 1 beta de feature high-impact
    └─ KR3: Atingir 80% satisfaction na beta

────────────────────────────────────────────────

TEAM - SALES (Q1 2024)
├─ O1: Construir engine de aquisição escalável
│   ├─ KR1: Crescer pipeline de 50 para 150 SQLs/mês
│   │   └─ [Contribui para Company O1.KR1 - MRR]
│   ├─ KR2: Aumentar win rate de 15% para 30%
│   │   └─ [Contribui para Company O1.KR1 - MRR]
│   └─ KR3: Reduzir CAC de R$5k para R$2.5k
│       └─ [Contribui para Company O1.KR1 - MRR sustentável]

────────────────────────────────────────────────

TEAM - MARKETING (Q1 2024)
├─ O1: Tornar marca top-of-mind no segmento PME
│   ├─ KR1: Crescer tráfego orgânico de 5k para 20k/mês
│   │   └─ [Contribui para Company O2.KR2 - MQLs]
│   ├─ KR2: Publicar 30 artigos high-quality SEO
│   │   └─ [Contribui para Company O2.KR3 - Google ranking]
│   └─ KR3: Gerar 5.000 MQLs via conteúdo
│       └─ [Contribui para Company O2.KR2 - MQLs]
```

---

### Regras de Alinhamento

#### Regra 1: 60/40
```
60% dos Team OKRs: Alinhados com Company OKRs (top-down)
40% dos Team OKRs: Iniciativas do próprio time (bottom-up)
```

**Por que 60/40**:
- Garante alinhamento estratégico (60%)
- Permite inovação e iniciativas do time (40%)
- Evita micromanagement

#### Regra 2: Contribuição, não Duplicação
```
❌ Ruim (duplicação):
Company KR: Crescer MRR de R$100k para R$300k
Team KR: Crescer MRR de R$100k para R$300k
└─ Time apenas repete o Company KR

✅ Bom (contribuição):
Company KR: Crescer MRR de R$100k para R$300k
Team Sales KR: Aumentar win rate de 15% para 30%
Team Marketing KR: Crescer pipeline de 50 para 150 SQLs/mês
└─ Times contribuem com pedaços específicos
```

#### Regra 3: Alinhamento Explícito
```
Ao escrever Team OKR, indique:
"[Contribui para Company O1.KR2]"

Benefícios:
- Clareza de conexão
- Facilita priorização
- Evita trabalho desalinhado
```

---

## 📊 Ciclos e Cadência

### Ciclo Recomendado: Trimestral

**Por que trimestral (13 semanas)**:
- ✅ Longo o suficiente para gerar impacto real
- ✅ Curto o suficiente para manter foco
- ✅ Alinha com ano fiscal (4 trimestres)
- ✅ Permite ajustes frequentes (4x/ano)

**Alternativas**:
- **Mensal**: Para early-stage startups (pré-PMF)
- **Semestral**: Para empresas mais maduras
- **Anual**: Para visão estratégica (Company-level apenas)

---

### Timeline de um Ciclo Trimestral

```
SEMANA -2 (Planejamento Liderança)
├─ Leadership Team define Company OKRs draft
├─ Analisa resultados do trimestre anterior
└─ Define contexto estratégico

SEMANA -1 (Planejamento Times)
├─ Heads de área compartilham Company OKRs com times
├─ Times propõem seus Team OKRs alinhados
├─ Sessão de review e ajustes
└─ Finalização e publicação de todos OKRs

SEMANA 1-6 (Primeira Metade)
├─ Check-ins semanais (15-30min)
├─ Tracking de progresso
└─ Ajustes táticos (não mudar OKRs)

SEMANA 7 (Mid-Quarter Review)
├─ Revisão de progresso (all-hands ou por time)
├─ Ajuste de OKRs se contexto mudou drasticamente
└─ Realinhamento de energia/recursos

SEMANA 8-12 (Segunda Metade)
├─ Check-ins semanais (continuam)
├─ Sprint final para OKRs at-risk
└─ Preparação para scoring

SEMANA 13 (Fechamento)
├─ Scoring final (cada KR recebe 0.0-1.0)
├─ Review e retrospectiva
├─ Documentação de learnings
└─ Início do planejamento do próximo trimestre
```

---

### Check-ins Semanais

**Formato**: 15-30 minutos, síncrono ou assíncrono

**Agenda**:
1. Revisar progresso de cada KR (score atual)
2. Identificar blockers e riscos
3. Definir ações da semana
4. Atualizar confidence (on track / at risk / off track)

**Template**:
```
Week 5 of 13 | [Data]

KR1: Crescer MRR de R$100k para R$300k
├─ Score atual: 0.35 (progresso: R$170k MRR)
├─ Confidence: 🟢 On track
└─ Update: Fechamos 15 novos clientes este mês, pipeline forte

KR2: Atingir NPS de 50+
├─ Score atual: 0.20 (progresso: NPS 38)
├─ Confidence: 🟡 At risk
├─ Blocker: Churn aumentou devido a bug crítico
└─ Action: Priorizando fix do bug, enviando pesquisa de NPS adicional

KR3: Alcançar retention 90%+
├─ Score atual: 0.60 (progresso: retention 86%)
├─ Confidence: 🟢 On track
└─ Update: Onboarding melhorado ajudou, mas ainda precisamos 4pp
```

---

## 🎓 Metodologia Google de OKRs

### Google's OKR Best Practices

#### 1. Score esperado: 0.6-0.7

```
Ao definir OKRs, pergunte:
"Qual é a probabilidade de atingirmos 100% disso?"

Se resposta for:
- 90%+ → Não é ambicioso o suficiente
- 60-70% → Sweet spot ✅
- <40% → Moonshot demais (pode ser desmotivador)
```

**Google separa**:
- **Committed OKRs**: Espera-se 1.0 (100%) - ex: compliance, launches críticos
- **Aspirational OKRs**: Espera-se 0.6-0.7 (maioria dos OKRs)

#### 2. OKRs públicos (Internal Transparency)

**Na prática do Google**:
- Todo OKR está no sistema interno (Google's internal tool)
- Qualquer funcionário pode ver OKRs de qualquer outro (até CEO)
- OKRs são apresentados em All-Hands (TGIF - Thank God It's Friday)

**Benefícios observados**:
- Alinhamento natural entre times
- Reduz silos e duplicação de esforços
- Aumenta accountability

#### 3. Grading rigoroso

**Google faz grading de 0.0-1.0**:
```
0.0-0.3: Vermelho (underperformance severa)
0.4-0.6: Amarelo (progresso, mas abaixo da ambição)
0.7-1.0: Verde (sucesso!)

1.0 consistente → Sinal de sandbagging
```

**Larry Page sobre scoring 1.0**:
> "Se você está consistentemente batendo 1.0, seus OKRs não são ambiciosos o suficiente."

#### 4. OKRs não afetam promoção/bônus

**Google é explícito**:
- Performance review ≠ OKR score
- Avalia-se contribuição, esforço, qualidade
- Pessoa pode ter score 0.4 e ainda receber avaliação "Exceeds"

**Razão**: Incentiva stretch goals sem medo de punição

---

### Erros que Google Aprendeu (Early Days)

#### Erro 1: Muitos OKRs
```
Google no começo: Times tinham 10-15 OKRs
Resultado: Dispersão, nada era prioridade

Fix: Limitar a 3-5 Objectives
```

#### Erro 2: OKRs muito conservadores
```
Problema: Times com medo de falhar definiam OKRs fáceis
Resultado: Score 1.0 consistente, pouca inovação

Fix: Cultura de "failing is ok", grading público, incentivo a ambição
```

#### Erro 3: OKRs viram roadmap
```
Problema: KRs eram lista de features a lançar
Resultado: Foco em output, não outcome

Fix: Treinamento em "outcomes thinking", exemplos claros
```

---

## 🌍 OKRs em Outras Empresas (Cases)

### LinkedIn

**Contexto**: IPO em 2011, crescimento rápido (500 → 10.000 funcionários)

**Adaptação**:
- Ciclo anual (não trimestral) para strategic OKRs
- Ciclo trimestral para execution OKRs
- Separação: Strategic vs Operational OKRs

**Exemplo de OKR LinkedIn (2015)**:
```
O: Tornar-se a plataforma essencial para profissionais
  KR1: Crescer active users de 300M para 400M
  KR2: Atingir 50% dos usuários visitando semanalmente
  KR3: Dobrar engagement em grupos profissionais
```

**Aprendizado**:
> "OKRs nos forçaram a priorizar. Antes, tínhamos 20 prioridades. OKRs nos fizeram escolher 5." - Jeff Weiner, CEO

---

### Twitter

**Contexto**: Pós-IPO (2013), precisava de foco

**Desafio**: Empresa muito descentralizada, silos fortes

**Solução com OKRs**:
- Introduziu Company OKRs muito claros
- Todos Team OKRs precisavam mapear para Company
- Rituais semanais de alinhamento

**Exemplo OKR Twitter (2015)**:
```
O: Simplificar experiência para novos usuários
  KR1: Reduzir time-to-follow de 10min para 2min
  KR2: Aumentar % de novos usuários que completam onboarding de 40% para 70%
  KR3: Dobrar retention D7 (day 7)
```

---

### Intel (Origem)

**OKR histórico que salvou Intel (1980s)**:

**Contexto**: Intel fabricava memória DRAM. Japoneses estavam dominando mercado.

**Decisão**: Pivotar para microprocessadores

**OKR de Andy Grove (1985)**:
```
O: Tornar-se líder global em microprocessadores
  KR1: Alcançar 2000 design wins com 8086
  KR2: Atingir 50% market share em PC microprocessors
  KR3: Reduzir custo de produção em 30%
```

**Resultado**: Intel se tornou dominante em CPUs por décadas

**Lição**: OKRs podem guiar pivots estratégicos críticos

---

## 📏 Medindo Sucesso de OKRs

### Sinais de que OKRs estão funcionando:

✅ **Time tem clareza de prioridades**
- Pergunta: "Quais são suas top 3 prioridades?"
- Resposta deve ser: seus 3 Objectives

✅ **Decisões ficam mais fáceis**
- "Devemos trabalhar em X ou Y?"
- Resposta: "Qual contribui mais para nossos OKRs?"

✅ **Cross-functional alignment melhora**
- Times sabem no que outros estão trabalhando
- Menos surpresas, mais colaboração

✅ **Ambição aumenta**
- Times param de pensar +10%, começam a pensar +100%
- Inovação aumenta

✅ **Foco melhora**
- Menos projetos paralelos
- Mais profundidade, menos dispersão

---

### Sinais de que OKRs NÃO estão funcionando:

❌ **Scores sempre 1.0**
- Indica sandbagging (metas conservadoras)
- OKRs não são stretch goals

❌ **Ninguém olha OKRs após semana 1**
- Falta de check-ins regulares
- OKRs viraram "documento de gaveta"

❌ **OKRs são lista de tarefas**
- KRs são outputs (features, projetos)
- Não são outcomes (métricas de negócio)

❌ **Times trabalham em coisas fora dos OKRs**
- Falta de disciplina de foco
- OKRs não refletem real priorização

❌ **Medo de falhar**
- Times evitam OKRs ambiciosos
- Cultura não aceita scores baixos

---

## 🚀 Implementando OKRs (Primeiras Vezes)

### Fase 1: Pilotar (Trimestre 1)

**Escopo**: Apenas Company-level OKRs
- CEO + Leadership definem 3-5 OKRs
- Comunicam para toda empresa
- Fazem check-ins mensais (não semanais ainda)

**Objetivo**: Aprender a mecânica, ganhar confiança

---

### Fase 2: Expandir (Trimestre 2-3)

**Escopo**: Company + Team OKRs
- Heads de área criam Team OKRs alinhados
- Check-ins semanais começam
- Grading rigoroso no final

**Objetivo**: Cascata, alinhamento vertical

---

### Fase 3: Maturidade (Trimestre 4+)

**Escopo**: Company + Team + Individual (opcional)
- OKRs em todos níveis
- Cultura de transparência e ambição estabelecida
- Rituais bem definidos

**Objetivo**: OKRs viraram "sistema operacional" da empresa

---

## 📚 Recursos Adicionais

**Livros recomendados**:
1. **"Measure What Matters"** - John Doerr (essencial)
2. **"Radical Focus"** - Christina Wodtke (OKRs para startups)
3. **"High Output Management"** - Andy Grove (origem dos OKRs)

**Ferramentas**:
- Notion, Asana, Linear (templates de OKR)
- Google Sheets (simple tracking)
- Ferramentas dedicadas: Gtmhub, Perdoo, Weekdone

**Recursos online**:
- Google's OKR Playbook (re:Work website)
- WhatMatters.com (site de John Doerr)

---

**Próximos guias**:
- [okr-writing-guide.md](okr-writing-guide.md) - Como escrever OKRs de alta qualidade
- [okr-cadence-rituals.md](okr-cadence-rituals.md) - Rituais e ciclos detalhados
- [okr-common-mistakes.md](okr-common-mistakes.md) - Erros comuns e como evitar
