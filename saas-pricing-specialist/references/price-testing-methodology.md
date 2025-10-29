# Metodologia de Testes de Preço para SaaS

Guia completo sobre como testar preços de forma segura e científica: A/B testing, multivariate, cohort experiments, testes com novos clientes vs. base existente.

---

## Por Que Testar Preços?

**Pricing research (surveys, entrevistas) te dá hipóteses.**

**Pricing testing te dá DADOS REAIS.**

**Diferença:**
- Survey: "Eu pagaria R$500"
- Test: Cliente REALMENTE paga R$500 (ou não)

**Dados > Opiniões.**

---

## Princípios de Price Testing

### 1. Testar com Dados Reais de Compra

**Não testar:**
- Clicks
- Page views
- "Interesse"

**Testar:**
- Conversion rate (compra real)
- Revenue per visitor
- LTV (Lifetime Value)

---

### 2. Significância Estatística

**Precisa de volume suficiente.**

**Regra prática:**
- Mínimo 100 conversions por variante
- Ou 1.000+ visitors (se conversion rate ~10%)

**Se não tem volume:** Teste qualitativo (entrevistas) em vez de quantitativo.

---

### 3. Isolar Variável de Preço

**Testar apenas preço (não mudar outras coisas).**

**Ruim:**
- Variante A: R$99 + design velho
- Variante B: R$149 + design novo

**Problema:** Não sabe se diferença é preço ou design.

**Bom:**
- Variante A: R$99
- Variante B: R$149
- (tudo mais igual)

---

### 4. Evitar Descoberta (Clientes Vendo Preços Diferentes)

**Maior risco de price testing.**

**Cenário ruim:**
- Cliente A vê R$99
- Cliente B vê R$149
- Cliente B descobre que A pagou menos
- **Backlash, perda de confiança**

**Mitigações:**
- Testar em cohorts separados (geografia, canal)
- Comunicar transparência se descoberto
- Ter política de price matching temporária

---

## Metodologia 1: A/B Test de Preço Absoluto

### Conceito

**Testar 2 preços diferentes, medir qual gera mais revenue.**

**Setup:**
- 50% do tráfego vê Preço A
- 50% vê Preço B
- Medir conversion + revenue

---

### Exemplo Prático

**Hipótese:** "Preço de R$149/mês gera mais revenue que R$99/mês."

**Setup:**
- Grupo A: R$99/mês
- Grupo B: R$149/mês
- Duração: 4 semanas
- Volume: 2.000 visitors (1.000 cada)

**Resultados:**

| Grupo | Preço | Visitors | Conversions | Conv Rate | Revenue Total | Rev/Visitor |
|-------|-------|----------|-------------|-----------|---------------|-------------|
| A | R$99 | 1.000 | 80 | 8% | R$7.920 | R$7,92 |
| B | R$149 | 1.000 | 60 | 6% | R$8.940 | R$8,94 |

**Análise:**
- Grupo A: Conv rate maior (8% vs. 6%)
- Grupo B: Revenue/visitor maior (R$8,94 vs. R$7,92)
- **Grupo B é vencedor (+13% revenue/visitor)**

**Decisão:** Adotar R$149/mês.

---

### Métrica Correta: Revenue per Visitor

**NÃO otimizar para conversion rate.**

**Exemplo de erro:**

| Preço | Conv Rate | Revenue/Visitor |
|-------|-----------|-----------------|
| R$50 | 15% | R$7,50 |
| R$200 | 5% | R$10,00 |

**R$50 tem conversion 3x maior, mas R$200 gera +33% revenue.**

**Vencedor:** R$200.

---

### Quando Usar A/B de Preço Absoluto

**✅ Tem tráfego suficiente (1.000+ visitors/mês)**

**✅ Produto self-service (não sales-led)**

**✅ Quer testar 2 preços específicos**

---

## Metodologia 2: Multivariate Test (Múltiplas Variáveis)

### Conceito

**Testar preço + outras variáveis simultaneamente.**

**Exemplo: Preço × Billing Frequency**

**4 Variantes:**
1. R$99/mês, mensal
2. R$99/mês, anual (R$990)
3. R$149/mês, mensal
4. R$149/mês, anual (R$1.490)

**Medir:** Qual combinação maximiza revenue.

---

### Exemplo Prático

**Resultados:**

| Variante | Preço Mensal | Billing | Conv Rate | ACV (Annual Contract Value) | Rev/Visitor |
|----------|--------------|---------|-----------|----------------------------|-------------|
| A | R$99 | Mensal | 10% | R$1.188 | R$118,80 |
| B | R$99 | Anual | 8% | R$990 | R$79,20 |
| C | R$149 | Mensal | 7% | R$1.788 | R$125,16 |
| D | R$149 | Anual | 6% | R$1.490 | R$89,40 |

**Análise:**
- **Variante C (R$149 mensal) gera mais revenue/visitor**
- Anual tem conversion menor (commitment maior)
- R$149 > R$99 mesmo com conversion menor

**Decisão:** Adotar R$149/mês (mensal).

---

### Cuidado: Tamanho de Amostra

**Multivariate precisa de MUITO mais tráfego.**

**Exemplo:**
- A/B test (2 variantes): 1.000 visitors cada = 2.000 total
- Multivariate (4 variantes): 1.000 cada = **4.000 total**

**Se não tem volume:** Fica com A/B simples.

---

## Metodologia 3: Sequential Testing (Teste Sequencial)

### Conceito

**Testar preços em sequência (não paralelo).**

**Processo:**
1. Mês 1: R$99 (baseline)
2. Mês 2: R$149
3. Mês 3: R$199
4. Comparar resultados

---

### Vantagens

**✅ Não precisa de split de tráfego**
- Todos veem mesmo preço

**✅ Sem risco de clientes descobrirem preços diferentes**

---

### Desvantagens

**❌ Sazonalidade**
- Mês 1 (Janeiro) vs. Mês 3 (Março) podem ter demanda diferente
- Confunde resultados

**❌ Mudanças externas**
- Competidor lança novo produto
- Marketing campaign muda
- Difícil isolar efeito do preço

**❌ Demorado**
- 3 meses para testar 3 preços

---

### Quando Usar Sequential

**✅ Baixo volume (não dá para split)**

**✅ Produto muito early-stage**

**✅ Aceita que dados serão menos confiáveis**

---

## Metodologia 4: Cohort-Based Testing

### Conceito

**Testar preços em cohorts NATURALMENTE separados.**

**Exemplos de cohorts:**
1. **Geografia:** Brasil vs. México
2. **Canal:** Organic vs. Paid ads
3. **Produto:** Feature A vs. Feature B users
4. **Tempo:** Signups de Janeiro vs. Fevereiro

---

### Exemplo: Teste por Geografia

**Setup:**
- Brasil: R$299/mês
- México: R$249/mês (mesmo produto, preço diferente)
- Duração: 3 meses

**Resultados:**

| País | Preço | Signups | Conv Rate | MRR | Rev/Signup |
|------|-------|---------|-----------|-----|------------|
| Brasil | R$299 | 500 | 8% | R$11.960 | R$23,92 |
| México | R$249 | 400 | 10% | R$9.960 | R$24,90 |

**Análise:**
- México: Conv rate maior (10% vs. 8%)
- México: Rev/signup maior (R$24,90 vs. R$23,92)
- **México (R$249) performa melhor**

**Insight:** R$299 pode estar caro. Considerar reduzir para R$249 também no Brasil.

---

### Vantagens

**✅ Cohorts separados = sem risco de descoberta**

**✅ Natural (não precisa de ferramenta de A/B test)**

---

### Desvantagens

**❌ Cohorts podem ser diferentes**
- Brasil vs. México: Mercados diferentes
- Não é comparação perfeita

**❌ Confounders (variáveis confusas)**
- México pode ter competitor diferente, economia diferente

---

### Quando Usar Cohort Testing

**✅ Não pode fazer A/B test (risco de descoberta)**

**✅ Tem cohorts naturalmente separados**

**✅ Aceita que comparação não é perfeita**

---

## Metodologia 5: New Customer Test (Apenas Novos Clientes)

### Conceito

**Testar preço APENAS com novos clientes, não mexer com base existente.**

**Mais seguro.**

---

### Setup

**Clientes existentes:** Mantêm preço atual (R$99)

**Novos clientes (a partir de hoje):**
- 50%: R$99 (controle)
- 50%: R$149 (teste)

**Duração:** 2-3 meses

**Medir:** Conversion, churn, LTV de cada cohort.

---

### Vantagens

**✅ Sem risco com base existente**
- Clientes atuais não são afetados

**✅ Pode testar aumento significativo**
- Ex: +50% de preço

---

### Desvantagens

**❌ Cria 2 pricing tiers diferentes**
- Clientes antigos (R$99) e novos (R$149)
- Pode gerar atrito se descoberto

**❌ Precisa de volume de novos signups**

---

### Quando Usar

**✅ Quer testar aumento de preço, mas tem medo de churnar base**

**✅ Tem volume suficiente de novos clientes**

**✅ Pode grandfather clientes antigos depois**

---

## Metodologia 6: Price Increase Test (Teste de Aumento)

### Conceito

**Testar aumento de preço para % da base existente.**

**Mais arriscado, mas dados valiosos.**

---

### Setup

**Selecionar cohort pequeno (5-10% da base):**
- Cohort A (controle): Mantém R$99
- Cohort B (teste): Aumenta para R$149

**Critérios de seleção:**
- Clientes similar (mesmo tenure, uso, vertical)
- NÃO high-value accounts (risco menor se churnar)

**Duração:** 1-2 meses

**Medir:**
- Churn rate
- Complaints
- Downgrade rate

---

### Exemplo

**Base:** 1.000 clientes em R$99/mês

**Teste:**
- 900 clientes (90%): Mantém R$99 (controle)
- 100 clientes (10%): Aumenta para R$149 (teste)

**Resultados após 1 mês:**

| Grupo | Preço | Clientes Início | Churn | Churn Rate | MRR Final |
|-------|-------|-----------------|-------|------------|-----------|
| Controle | R$99 | 900 | 18 | 2% | R$87.318 |
| Teste | R$149 | 100 | 5 | 5% | R$14.155 |

**Análise:**
- Churn aumentou de 2% para 5% (+3pp)
- MRR/cliente: R$97 (controle) vs. R$141,55 (teste)
- **+46% MRR/cliente, mesmo com +3pp churn**

**Decisão:** Aumento é viável. Rolar para toda base (com comunicação adequada).

---

### Cuidados

**⚠️ Risco de backlash**
- Clientes descobrem que outros não tiveram aumento
- Reputação ruim

**⚠️ Não testar com clientes VIP**
- Risco muito alto

**⚠️ Ter plano de rollback**
- Se churn >10%, reverter

---

### Quando Usar

**✅ Quer testar aumento para base existente**

**✅ Tem base grande (1.000+ clientes)**

**✅ Aceita risco de algum churn**

---

## Metodologia 7: Grandfathered Test

### Conceito

**Aumentar preço para novos, manter (grandfather) para existentes.**

**Depois, medir:**
- Conversion de novos com preço novo
- Retention de antigos (têm deal melhor, menos churn?)

---

### Setup

**A partir de hoje:**
- Clientes existentes: R$99 (grandfathered)
- Novos clientes: R$149

**Medir:**
- Conversion rate de novos (R$149)
- Churn rate de grandfathered (R$99) vs. novos (R$149)

---

### Insights

**Se conversion de novos (R$149) é OK:**
- Preço R$149 funciona

**Se churn de grandfathered é MENOR que novos:**
- Grandfathering gera loyalty
- Clientes valorizam ter "deal especial"

---

### Exemplo

**Resultados após 6 meses:**

| Cohort | Preço | Conv Rate (Novos) | Churn/Ano (Existentes) |
|--------|-------|-------------------|------------------------|
| Grandfathered | R$99 | N/A | 15% |
| Novo pricing | R$149 | 7% (vs. 9% antes) | 20% |

**Análise:**
- Novo preço (R$149): Conversion caiu de 9% para 7% (-22%)
- Mas revenue/visitor: Aumentou (+50% de preço > -22% conversion)
- Grandfathered: Churn menor (15% vs. 20%)

**Decisão:** Manter R$149 para novos, continuar grandfathering antigos.

---

## O Que Medir em Price Tests

### Métricas Primárias

#### 1. Conversion Rate

**% de visitors que compram.**

```
Conversion Rate = Conversions / Visitors
```

**Exemplo:**
- 1.000 visitors
- 80 conversions
- Conversion = 8%

---

#### 2. Revenue per Visitor

**Receita média por visitor.**

```
Rev/Visitor = Total Revenue / Visitors
```

**Exemplo:**
- Preço: R$149
- Conversion: 6%
- Rev/Visitor = R$149 × 6% = **R$8,94**

**Métrica mais importante para price tests.**

---

#### 3. Average Contract Value (ACV)

**Valor médio do contrato.**

```
ACV = Total Revenue / Conversions
```

**Exemplo:**
- Revenue total: R$8.940
- Conversions: 60
- ACV = R$149/mês × 12 = **R$1.788/ano**

---

### Métricas Secundárias

#### 4. Churn Rate (para testes com base existente)

**% de clientes que cancelam.**

```
Churn Rate = Cancelamentos / Clientes Início
```

**Importante:** Preço mais alto pode aumentar churn.

---

#### 5. LTV (Lifetime Value)

**Valor total que cliente gera ao longo da vida.**

```
LTV = ARPU × (1 / Churn Rate)
```

**Exemplo:**
- ARPU: R$149/mês
- Churn: 3%/mês
- LTV = R$149 / 0.03 = **R$4.967**

**Ideal:** Medir LTV de cohorts com preços diferentes.

---

#### 6. LTV:CAC Ratio

**Retorno sobre custo de aquisição.**

```
LTV:CAC = LTV / CAC
```

**Benchmark:**
- Bom: 3:1 ou maior
- Muito bom: 5:1+

**Price test pode melhorar LTV (preço maior) sem aumentar CAC.**

---

## Ferramentas para Price Testing

### A/B Testing Tools

**SaaS:**
- **Google Optimize** (descontinuado, mas alternativas)
- **Optimizely** (enterprise, caro)
- **VWO** (Visual Website Optimizer)
- **Split.io** (feature flags + A/B)

**Custom:**
- Implementar próprio A/B test (backend)
- Feature flags (LaunchDarkly, etc.)

---

### Analytics

**Medir resultados:**
- **Google Analytics** (grátis, básico)
- **Mixpanel** (eventos, funnels)
- **Amplitude** (product analytics)
- **Segment** (data pipeline)

---

### Pricing-Specific

**Plataformas especializadas:**
- **Price Intelligently** (agora ProfitWell)
- **Simon-Kucher** (consultoria)

---

## Duração Ideal de Teste

**Pergunta:** Quanto tempo rodar teste?

**Regra geral:** Até atingir significância estatística.

---

### Calculadora de Sample Size

**Fórmula simplificada:**

```
Sample size por variante = 16 × (p × (1-p)) / (MDE²)
```

**Onde:**
- p = baseline conversion rate
- MDE = Minimum Detectable Effect (diferença mínima que importa)

---

**Exemplo:**
- Baseline conversion: 8% (p = 0.08)
- MDE: 20% (quer detectar diferença de 20% em conversion)
- MDE² = 0.04

```
Sample size = 16 × (0.08 × 0.92) / (0.04²)
            = 16 × 0.0736 / 0.0016
            = 736 visitors por variante
```

**Total:** 1.472 visitors (2 variantes).

---

### Duração

**Se tem 1.000 visitors/mês:**
- Precisa de 1.472 total
- **Duração: ~1.5 meses**

**Se tem 10.000 visitors/mês:**
- **Duração: ~1 semana**

---

### Mínimo: 1-2 Semanas

**Mesmo com volume alto, rodar mínimo 1-2 semanas.**

**Por quê:**
- Capturar variação semanal (fim de semana vs. semana)
- Evitar viés de timing

---

## Quando NÃO Fazer Price Testing

### Cenário 1: Volume Muito Baixo

**Se tem <500 visitors/mês:**
- A/B test não vai ter significância
- Levaria 6+ meses

**Alternativa:** Pricing research (entrevistas, Van Westendorp).

---

### Cenário 2: Sales-Led (Não Self-Service)

**Se pricing é negociado:**
- Cada deal é custom
- Não há "preço fixo" para testar

**Alternativa:** Win/loss analysis.

---

### Cenário 3: Risco de Backlash Muito Alto

**Se:**
- Base pequena (100 clientes)
- Comunidade tight-knit (todos se conhecem)
- Risco de descoberta é 100%

**Alternativa:** Testar só com novos clientes ou aumentar para todos (sem A/B).

---

## Comunicação de Price Changes Durante Teste

**Se cliente descobre teste:**

### Opção 1: Transparência

**Email:**
```
Olá [Nome],

Estamos testando diferentes preços para encontrar o equilíbrio certo.
Você foi selecionado para [Preço A].

Se encontrar outro preço, entre em contato - garantimos price matching.

Obrigado pela compreensão.
```

**Vantagens:** Honesto, confiança.

**Desvantagens:** Revela que está testando (pode afetar comportamento).

---

### Opção 2: Price Matching Silencioso

**Se cliente reclama:**
- "Eu vi R$99, mas vocês mostraram R$149!"

**Resposta:**
- "Você tem razão, aplicamos R$99 para você."
- Honrar preço mais baixo

**Vantagens:** Mantém cliente feliz.

**Desvantagens:** Perde dados (se todos pedem menor preço).

---

### Opção 3: Explicar Segmentação

**Resposta:**
- "Diferentes preços para diferentes segmentos (empresa vs. individual, etc.)"

**Funciona se:** Segmentação faz sentido.

**Não funciona se:** Segmentos são idênticos (óbvio que é teste).

---

## Case Study: Intercom Price Test Gone Wrong

**Contexto (2018):**
- Intercom mudou modelo de pricing
- De per-seat para per-seat + per-conversation
- Testou com % da base

**Problema:**
- Alguns clientes viram conta aumentar 2-3x
- Descobriram que nem todos foram afetados
- **Backlash massivo no Twitter, comunidade**

**Resultado:**
- Intercom teve que fazer grandfathering
- PR ruim
- Churn elevado

**Lição:**
- Comunicar mudanças grandes ANTES
- Ser transparente sobre motivação
- Oferecer grandfathering ou transição suave

---

## Checklist de Price Testing

**Antes de rodar teste:**

### Preparação
- [ ] **Hipótese clara:** O que está testando? Qual preço espera ganhar?
- [ ] **Métrica primária definida:** Revenue/visitor? LTV?
- [ ] **Sample size calculado:** Tem volume suficiente?
- [ ] **Duração estimada:** Quanto tempo vai levar para significância?

### Setup
- [ ] **Variável isolada:** Só preço muda (nada mais)?
- [ ] **Cohorts aleatórios:** Split de tráfego é verdadeiramente randômico?
- [ ] **Tracking implementado:** Analytics capturando dados corretamente?

### Risco
- [ ] **Plano de comunicação:** O que dizer se cliente descobre?
- [ ] **Rollback plan:** Como reverter se der errado?
- [ ] **Exclusão de VIPs:** Clientes high-value estão protegidos?

### Análise
- [ ] **Significância estatística:** Resultados são confiáveis (não flutuação)?
- [ ] **Confounders considerados:** Sazonalidade? Mudanças externas?
- [ ] **Decisão baseada em dados:** Vai implementar preço vencedor?

---

## Conclusão: Framework de Price Testing

**Processo recomendado:**

**1. Definir hipótese**
- Ex: "R$149 vai gerar +20% revenue/visitor vs. R$99"

**2. Escolher metodologia**
- Self-service + volume alto: A/B test
- Sales-led: Win/loss analysis
- Baixo volume: Sequential ou cohort test

**3. Calcular sample size e duração**
- Usar calculadora de sample size
- Estimar quanto tempo vai levar

**4. Implementar teste**
- Usar ferramenta (Optimizely, custom)
- Verificar tracking

**5. Rodar teste (1-2 meses típico)**
- Monitorar resultados
- Não parar cedo (aguardar significância)

**6. Analisar dados**
- Revenue/visitor é métrica #1
- Considerar LTV se possível

**7. Tomar decisão**
- Implementar preço vencedor
- Ou iterar (testar novo preço)

**8. Comunicar mudança (se necessário)**
- Para base existente
- Transparência sobre aumento

---

**Próximo arquivo:** `price-increases-playbook.md` (como aumentar preços sem churnar clientes: comunicação, timing, grandfathering, objeções)