# Métricas e KPIs para B2B SaaS

## Hierarquia de Métricas

### Métricas North Star (Prioridade Máxima)

A métrica North Star é a única métrica que melhor captura o valor core que você entrega aos clientes.

**Exemplos por tipo de produto**:
- **Produto de colaboração**: Usuários ativos semanais colaborando
- **Produto de analytics**: Dashboards ativos com decisões tomadas
- **Produto de vendas**: Deals fechados na plataforma
- **Produto de automação**: Horas economizadas por cliente

**Características de uma boa North Star**:
- Expressa valor entregue ao cliente
- Reflete crescimento da empresa
- É acionável pelo time
- Fácil de entender e comunicar

### Métricas Primárias (Acompanhar Semanalmente)

1. **MRR (Monthly Recurring Revenue)** - Receita recorrente mensal
2. **Churn Rate** - Taxa de cancelamento de clientes
3. **Net Revenue Retention (NRR)** - Retenção líquida de receita
4. **CAC (Customer Acquisition Cost)** - Custo de aquisição de cliente
5. **LTV (Lifetime Value)** - Valor vitalício do cliente

### Métricas Secundárias (Acompanhar Mensalmente)

1. **MQL → SQL Conversion** - Qualificação de leads
2. **Sales Cycle Length** - Duração do ciclo de vendas
3. **Win Rate** - Taxa de fechamento
4. **Average Contract Value (ACV)** - Valor médio do contrato
5. **Expansion MRR** - Receita de expansão
6. **Engagement Metrics** - Uso do produto

## Métricas Detalhadas

### 1. MRR (Monthly Recurring Revenue)

**Definição**: Receita previsível e recorrente normalizada mensalmente

**Cálculo**:
```
MRR = Soma de todas as assinaturas mensais
(Contratos anuais: valor anual / 12)
```

**Componentes**:
- **New MRR**: MRR de novos clientes
- **Expansion MRR**: MRR adicional de clientes existentes (upgrade, cross-sell)
- **Contraction MRR**: MRR perdido de downgrades
- **Churned MRR**: MRR perdido de cancelamentos

**Fórmula do crescimento**:
```
MRR Crescimento = New MRR + Expansion MRR - Contraction MRR - Churned MRR
Growth Rate = (MRR mês atual - MRR mês anterior) / MRR mês anterior
```

**Benchmarks**:
- Seed: 15-30% crescimento mensal
- Series A: 10-20% crescimento mensal
- Series B+: 5-10% crescimento mensal

**Armadilhas**:
- Incluir receitas não recorrentes (setup fees, consultoria)
- Não normalizar contratos anuais
- Contar MRR antes de pagamento recebido

### 2. ARR (Annual Recurring Revenue)

**Definição**: Receita recorrente anualizada

**Cálculo**:
```
ARR = MRR × 12
```

**Quando usar**: Útil para comparar com mercado e competidores

**Marcos importantes**:
- $1M ARR: Produto validado, time pequeno
- $5M ARR: PMF confirmado, pronto para Series A
- $10M ARR: Escala inicial, processos estabelecidos
- $50M ARR: Escala madura, múltiplos produtos/segmentos

### 3. Churn Rate

#### Revenue Churn (Mais importante para B2B)

**Definição**: % de MRR perdido por mês

**Cálculo**:
```
Monthly Revenue Churn = (MRR Churned no mês) / (MRR no início do mês)
```

**Benchmarks B2B SaaS**:
- Excelente: < 1% mensal (< 12% anual)
- Bom: 1-2% mensal (12-24% anual)
- Aceitável: 2-3% mensal (24-36% anual)
- Problemático: > 3% mensal (> 36% anual)

**Por segmento**:
- SMB: 3-7% mensal é normal (alta rotatividade de empresas pequenas)
- Mid-market: 1-3% mensal
- Enterprise: < 1% mensal

#### Customer Churn

**Definição**: % de clientes que cancelam por mês

**Cálculo**:
```
Monthly Customer Churn = (Clientes perdidos no mês) / (Clientes no início do mês)
```

**Uso**: Indicador de fit e satisfação, mas menos crítico que Revenue Churn para B2B

#### Churn Anualizado

**Cálculo**:
```
Annual Churn = 1 - (1 - Monthly Churn)^12
```

**Exemplo**: 2% churn mensal = 21.5% churn anual (não 24%!)

### 4. Net Revenue Retention (NRR)

**Definição**: % de receita retida de uma cohort de clientes, incluindo expansão

**Cálculo**:
```
NRR = (MRR início período + Expansion - Contraction - Churn) / MRR início período

Exemplo:
Cohort de Jan/2024 tinha $100k MRR
Em Jan/2025:
- Expansion: +$30k (upgrades)
- Contraction: -$5k (downgrades)
- Churn: -$10k (cancelamentos)
NRR = ($100k + $30k - $5k - $10k) / $100k = 115%
```

**Benchmarks**:
- Excelente: > 120%
- Bom: 100-120%
- Aceitável: 90-100%
- Problemático: < 90%

**Por que é importante**:
- NRR > 100% significa crescimento sem novos clientes
- Mostra land-and-expand funcionando
- Principal métrica para empresas públicas de SaaS

**Famosos NRRs públicos**:
- Snowflake: 158%
- Datadog: 130%
- Slack: 143%
- Zoom: 130%

### 5. CAC (Customer Acquisition Cost)

**Definição**: Custo total para adquirir um novo cliente

**Cálculo completo**:
```
CAC = (Vendas + Marketing + Tecnologia de Aquisição) / Novos Clientes
```

**Por canal**:
- **CAC Blended**: Custo médio de todos os canais
- **CAC por canal**: Calcular separadamente para inbound, outbound, partnerships, etc.

**Componentes**:
- Salários do time de vendas e marketing (fully loaded)
- Software e ferramentas (CRM, marketing automation, etc.)
- Advertising e paid media
- Eventos e marketing de conteúdo
- Agências e freelancers

**Benchmarks**:
- SMB: CAC = 3-5 meses de MRR do cliente
- Mid-market: CAC = 5-12 meses de MRR
- Enterprise: CAC = 12-24 meses de MRR

**Evolução esperada**:
- Early stage: CAC alto e ineficiente (aprendendo)
- Growth stage: CAC otimizado e escalável
- Mature: CAC estável com múltiplos canais

### 6. LTV (Lifetime Value)

**Definição**: Receita total esperada de um cliente durante toda sua vida

**Cálculo simplificado**:
```
LTV = ARPA / Revenue Churn Rate

Exemplo:
ARPA = $500/mês
Revenue Churn = 2%/mês
LTV = $500 / 0.02 = $25,000
```

**Cálculo com expansão**:
```
LTV = ARPA × Gross Margin / (Churn Rate - Expansion Rate)

Exemplo:
ARPA = $500/mês
Gross Margin = 80%
Churn Rate = 2%/mês
Expansion Rate = 0.5%/mês
LTV = $500 × 0.80 / (0.02 - 0.005) = $26,667
```

**Componentes**:
- **ARPA**: Average Revenue Per Account
- **Gross Margin**: Receita - custos diretos (hosting, support)
- **Churn**: Taxa de perda de clientes
- **Expansion**: Taxa de crescimento dentro da base

### 7. LTV:CAC Ratio

**Definição**: Relação entre valor vitalício e custo de aquisição

**Cálculo**:
```
LTV:CAC = LTV / CAC
```

**Benchmarks**:
- Excelente: > 4:1
- Bom: 3:1 a 4:1
- Aceitável: 2:1 a 3:1
- Problemático: < 2:1

**Interpretação**:
- **< 1:1**: Perdendo dinheiro em cada cliente (insustentável)
- **1:1 a 2:1**: Baixa margem, difícil crescer
- **3:1 a 4:1**: Saudável e escalável
- **> 5:1**: Pode estar sub-investindo em crescimento

### 8. CAC Payback Period

**Definição**: Tempo para recuperar o custo de aquisição

**Cálculo**:
```
CAC Payback = CAC / (ARPA × Gross Margin)

Exemplo:
CAC = $5,000
ARPA = $500/mês
Gross Margin = 80%
Payback = $5,000 / ($500 × 0.80) = 12.5 meses
```

**Benchmarks**:
- Excelente: < 6 meses
- Bom: 6-12 meses
- Aceitável: 12-18 meses
- Problemático: > 18 meses

**Por que é importante**:
- Determina quanto capital necessário para crescer
- Payback curto = menos capital intensivo
- Payback longo = precisa de mais fundraising

### 9. Rule of 40

**Definição**: Soma de crescimento e lucratividade deve ser > 40%

**Cálculo**:
```
Rule of 40 = Revenue Growth Rate + EBITDA Margin

Exemplo:
Growth = 60% ao ano
EBITDA Margin = -20% (queimando caixa)
Rule of 40 = 60% + (-20%) = 40% ✓
```

**Benchmarks**:
- Public SaaS médio: ~40%
- Top performers: > 50%
- Early stage: Não se aplica (foca em crescimento)

**Trade-offs**:
- **High growth, low margin**: Investindo pesado em crescimento
- **Low growth, high margin**: Otimizando para lucro
- **Balanced**: Crescimento sustentável e lucratividade

### 10. Métricas de Vendas

#### Sales Cycle Length

**Definição**: Tempo médio do primeiro contato até fechamento

**Benchmarks**:
- SMB: 1-3 meses
- Mid-market: 3-6 meses
- Enterprise: 6-18 meses

#### Win Rate

**Definição**: % de oportunidades que fecham

**Cálculo**:
```
Win Rate = Deals Won / (Deals Won + Deals Lost)
```

**Benchmarks**:
- Excelente: > 30%
- Bom: 20-30%
- Aceitável: 15-20%
- Problemático: < 15%

#### Sales Efficiency (Magic Number)

**Definição**: Quanto de receita gerado para cada $1 investido em vendas e marketing

**Cálculo**:
```
Magic Number = (ARR deste quarter - ARR quarter anterior) / (S&M spend quarter anterior)
```

**Benchmarks**:
- Excelente: > 1.0
- Bom: 0.75 - 1.0
- Aceitável: 0.5 - 0.75
- Problemático: < 0.5

**Interpretação**:
- Magic Number > 0.75: Pode acelerar investimento em S&M
- Magic Number < 0.5: Reduzir S&M e focar em eficiência

### 11. Métricas de Produto/Engajamento

#### Daily/Monthly Active Users (DAU/MAU)

**Definição**: Usuários únicos ativos diariamente e mensalmente

**Stickiness Ratio**:
```
Stickiness = DAU / MAU

Exemplo:
DAU = 5,000
MAU = 20,000
Stickiness = 25%
```

**Benchmarks**:
- Produtos usados diariamente: > 20%
- Produtos usados semanalmente: 10-20%
- Produtos usados mensalmente: 5-10%

#### Feature Adoption

**Definição**: % de clientes usando features específicas

**Tracking**:
- Features críticas: > 80% dos clientes devem usar
- Features secundárias: 30-50% é aceitável
- Features raramente usadas: considerar deprecar

#### Time to Value (TTV)

**Definição**: Tempo até cliente alcançar "aha moment"

**Benchmarks**:
- Excelente: < 1 dia
- Bom: < 1 semana
- Aceitável: < 1 mês
- Problemático: > 1 mês

### 12. Métricas de Satisfação

#### Net Promoter Score (NPS)

**Definição**: Probabilidade de cliente recomendar (0-10)

**Cálculo**:
```
NPS = % Promoters (9-10) - % Detractors (0-6)
```

**Benchmarks B2B SaaS**:
- Excelente: > 50
- Bom: 30-50
- Aceitável: 10-30
- Problemático: < 10

#### Customer Satisfaction (CSAT)

**Definição**: Satisfação com interação específica (1-5)

**Quando medir**:
- Após onboarding
- Após ticket de suporte
- Após feature launch

## Dashboard Recomendado por Estágio

### Pre-Seed / Seed (0-20 clientes)

**Foco**: Validação de PMF

Métricas essenciais:
1. Número de clientes ativos
2. Revenue Churn mensal
3. Usuários ativos semanais (por cliente)
4. NPS ou feedback qualitativo
5. Time to Value

### Seed / Series A (20-100 clientes)

**Foco**: Repetibilidade e escala inicial

Métricas essenciais:
1. MRR e crescimento mês a mês
2. Net Revenue Retention
3. CAC por canal
4. CAC Payback Period
5. Sales Cycle Length
6. Win Rate
7. Churn Rate (revenue e customer)

### Series A+ (100+ clientes)

**Foco**: Eficiência e escala

Métricas essenciais:
1. ARR e crescimento
2. Net Revenue Retention
3. LTV:CAC ratio
4. Rule of 40
5. Magic Number
6. Churn por segmento
7. Expansion MRR
8. Sales efficiency por rep
9. Cohort analysis completo

## Análise de Cohorts

**Por que é importante**: Entender comportamento ao longo do tempo, não só snapshot atual

**Como fazer**:
1. Agrupar clientes por mês de aquisição
2. Acompanhar métricas mês a mês para cada cohort
3. Identificar tendências (cohorts melhorando ou piorando?)

**Métricas para análise de cohort**:
- Revenue retention por cohort
- Expansion rate por cohort
- Churn rate por cohort
- Payback period por cohort

## Métricas por Segmento

Sempre quebrar métricas principais por:

1. **Segmento de cliente**: SMB vs. Mid-market vs. Enterprise
2. **Vertical**: Diferentes indústrias podem ter comportamentos distintos
3. **Canal de aquisição**: Inbound vs. Outbound vs. Partnerships
4. **Geografia**: Brasil vs. Internacional (se aplicável)
5. **Plano/Pricing tier**: Starter vs. Professional vs. Enterprise

## Armadilhas Comuns no Brasil

### 1. Confundir Receita Faturada com MRR

**Problema**: Contar receita anual antecipada como MRR de um mês

**Solução**: Normalizar sempre mensalmente (ARR / 12)

### 2. Ignorar Inadimplência

**Problema**: No Brasil, inadimplência pode ser 10-30% do faturado

**Solução**:
- Contar MRR apenas de clientes adimplentes
- Ter métrica separada para "MRR at risk"
- Investir em cobrança e recuperação

### 3. Não Ajustar por Moeda

**Problema**: Com câmbio volátil, receita em reais pode ser enganosa

**Solução**:
- Se tem receita internacional, reportar em USD
- Se só Brasil, reportar em BRL mas acompanhar poder de compra
- Comparar com benchmark internacional em USD

### 4. Pilotos/POCs Eternos

**Problema**: "Clientes" que nunca viram pagantes de fato

**Solução**:
- Não contar pilots em MRR
- Limitar duração de pilots (60 dias)
- Ter métrica separada: "Pilots → Paid conversion rate"

## Ferramentas de Tracking

### Gratuitas/Baratas
- Google Sheets + Data Studio
- Metabase (open source)
- Redash (open source)

### Pagas (Seed+)
- ChartMogul (foco em SaaS metrics)
- Baremetrics (similar a ChartMogul)
- Looker / Tableau / Power BI (empresas maiores)

### Integrações necessárias
- Stripe / Chargebee / Recurly (billing)
- Salesforce / HubSpot / Pipedrive (CRM)
- Segment / Mixpanel / Amplitude (produto)

## Frequência de Review

**Diária**:
- MRR atual
- Novos signups
- Churn do dia

**Semanal**:
- MRR growth rate
- Pipeline e forecast
- Product engagement

**Mensal**:
- Todas as métricas principais
- Cohort analysis
- Board deck preparation

**Trimestral**:
- Revisão estratégica profunda
- Ajuste de metas
- Planning do próximo quarter
