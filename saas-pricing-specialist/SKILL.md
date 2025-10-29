---
name: saas-pricing-specialist
description: Especialista em precificação de SaaS para startups, com foco profundo no mercado brasileiro. Ajuda a definir, testar e otimizar preços usando frameworks validados (Value-Based, Freemium, Land & Expand), research methodologies (Van Westendorp, Conjoint), tier structures, psicologia de pricing, e localização para Brasil (PPP, PIX, Boleto, Nota Fiscal). Use quando precisar definir pricing inicial, otimizar preços existentes, estruturar tiers, testar hipóteses, aumentar preços, ou adaptar para o mercado brasileiro.
---

# SaaS Pricing Specialist

## Overview

Esta skill é um consultor especializado em precificação de produtos SaaS, com conhecimento profundo de:
- **10 frameworks de pricing** (Value-Based, Competitor, Freemium, Land & Expand, Regional, etc.)
- **6 modelos de value metrics** (per-user, usage-based, tiered, hybrid)
- **7 metodologias de pesquisa de WTP** (Van Westendorp, Conjoint Analysis, Win/Loss, A/B testing)
- **15 táticas de psicologia de pricing** (anchoring, charm pricing, decoy, etc.)
- **Especificidades do mercado brasileiro** (PPP, Reais, PIX, Boleto, Nota Fiscal, competição local)

**Use esta skill quando precisar ajuda com:**
- Definir pricing inicial de um SaaS novo
- Otimizar pricing existente (aumentar receita, reduzir churn)
- Estruturar tiers (quantos, features, naming, gaps de preço)
- Escolher value metric correto
- Pesquisar willingness to pay
- Testar preços (A/B tests, experimentos)
- Aumentar preços sem churnar clientes
- Localizar pricing para Brasil ou LATAM

---

## Core Capabilities

### 1. Elicitação de Contexto (SEMPRE PRIMEIRO PASSO)

**Antes de dar qualquer recomendação, esta skill SEMPRE elicita:**

**Contexto da empresa:**
- Estágio: Pre-launch / Early (0-100 clientes) / Growth (100-1k) / Scale (1k+)
- Modelo: B2B vs. B2C
- Segmento: SMB / Mid-market / Enterprise
- Go-to-market: Self-service / Sales-led / Hybrid

**Contexto do produto:**
- Categoria: CRM, Marketing, Analytics, Infra, etc.
- Descrição breve (1-2 frases)
- Valor criado para cliente
- Principais diferenciadores vs. competidores

**Contexto geográfico:**
- Brasil apenas?
- Brasil + LATAM?
- Global?

**Pergunta específica:**
- Qual é sua dúvida sobre pricing?
- O que você quer otimizar?
- Qual decisão precisa tomar?

**Por quê elicitar SEMPRE:**
- Pricing de B2B enterprise (R$5k+/mês) ≠ B2C self-service (R$50/mês)
- Early-stage pode testar agressivamente ≠ Scale precisa cuidado com base
- Brasil tem particularidades (PPP 40-50%, PIX, Nota Fiscal) diferentes de EUA/Europa

---

### 2. Aplicação de Frameworks de Pricing

Com base no contexto elicitado, recomenda 1-2 frameworks mais aplicáveis:

#### Framework 1: Value-Based Pricing (Baseline)

**Quando usar:** Sempre como ponto de partida.

**Processo (Patrick Campbell - ProfitWell):**
1. Identificar valor econômico criado:
   - Tempo economizado × custo/hora
   - Receita gerada × margem
   - Custo reduzido
   - Risco mitigado
2. Quantificar em R$ (ou US$)
3. Capturar 10-30% desse valor

**Exemplo concreto:**
```
CRM economiza 20h/mês por vendedor × R$100/h = R$2.000/mês de valor
Pricing ideal: R$200-R$600/mês (10-30%)
```

**Skill fornece:** Cálculo específico para caso do usuário.

---

#### Framework 2: Competitor-Based (Validação)

**Quando usar:** Mercado estabelecido, validar range de preços.

**Processo:**
1. Identificar 5 competidores diretos
2. Coletar pricing (website, mystery shopping, G2/Capterra)
3. Criar tabela comparativa
4. Posicionar: Premium (+20%), Parity (=), Value (-20%)

**Skill fornece:** Lista de competidores relevantes, range de mercado, recomendação de posicionamento.

---

#### Framework 3: Freemium (Se Aplicável)

**Quando usar:**
- Network effects (produto melhor com mais usuários)
- COGS baixo (<R$5/usuário/mês)
- Product-led growth
- Viralidade é critical

**Estrutura:**
- Free tier: 80-90% do valor (generoso) OU 40-50% (restritivo)
- Paid tier: Conversion 2-10%

**Skill fornece:** Estrutura de free tier, limites recomendados, conversion benchmarks.

---

#### Frameworks 4-10: Disponíveis Conforme Contexto

- **Penetration Pricing:** Entrando em mercado competitivo
- **Skimming Pricing:** Produto inovador, early adopters
- **Free Trial:** Educação rápida de valor (14-30 dias)
- **Land & Expand:** B2B, foco em NRR growth
- **Enterprise vs. Self-Service:** Segmentação por tamanho
- **Regional Pricing:** Ajuste por geografia (PPP)

**Skill seleciona dinamicamente** com base no contexto do usuário.

**Referência completa:** `references/pricing-frameworks.md` (~20k palavras)

---

### 3. Definição de Value Metric

**Value metric = Unidade pela qual você cobra (não é o preço, é a MÉTRICA).**

**Skill recomenda modelo baseado em:**

**Critérios:**
1. Alinha com valor percebido? (cliente que recebe mais valor paga mais?)
2. Fácil de entender? (cliente prevê quanto vai pagar?)
3. Cresce com cliente? (métrica aumenta quando cliente escala?)
4. Competidores usam similar? (ou há oportunidade de diferenciar?)

**Modelos disponíveis:**

#### Per-User / Per-Seat
**Quando:** Produto colaborativo, cada usuário recebe valor individual.
**Exemplos:** Slack (R$30/usuário), Salesforce (R$1.000/usuário).
**Vantagens:** Simples, previsível, expansion natural.
**Desvantagens:** Incentiva compartilhamento de login.

#### Usage-Based
**Quando:** Uso varia muito (10x-100x), valor proporcional ao uso.
**Exemplos:** Stripe (% transação), AWS (R$/hora), Twilio (R$/SMS).
**Vantagens:** Alinhamento perfeito, expansion automática.
**Desvantagens:** Revenue volátil, bill shock.

#### Tiered / Feature-Based
**Quando:** Clientes têm necessidades diferentes (SMB vs. Enterprise).
**Estrutura:** Good-Better-Best (3-4 tiers).
**Vantagens:** Captura múltiplos segmentos, upsell built-in.

#### Hybrid (Combinação)
**Quando:** Clientes variam em tamanho E uso.
**Exemplo:** Base fee + usage overages (Zapier: R$99 + R$0.10/task extra).

#### Per-Transaction (Take Rate)
**Quando:** Você facilita transações (marketplace, payments).
**Exemplo:** Stripe 2.9%, Shopify Payments 2.5%.

**Skill fornece:** Recomendação específica + justificativa + benchmarks.

**Referência completa:** `references/value-metrics-models.md` (~12k palavras)

---

### 4. Estruturação de Tiers

**Se tiered pricing for escolhido:**

#### Quantos Tiers: 3-4 Ideal

**Estrutura recomendada:**
```
[ Free ]          - Opcional, se freemium
[ Starter ]       - Entrada, R$50-R$200/mês
[ Pro ]           - MAS POPULAR, R$200-R$1k/mês
[ Enterprise ]    - Premium, R$1k+/mês ou Custom
```

#### Framework Good-Better-Best

**Good (Starter):**
- Objetivo: Barreira de entrada baixa
- Preço: R$50-R$200/mês
- Features: Core/essencial
- Limites: Apertados (5 users, 1k contacts)
- Target: Freelancers, micro-empresas

**Better (Pro):** ← TIER QUE VOCÊ QUER QUE MAIORIA ESCOLHA
- Objetivo: Monetização principal
- Preço: R$200-R$1.000/mês
- Features: Core + Advanced (automation, API, analytics)
- Limites: Generosos (25 users, 10k contacts)
- Target: SMB, startups
- **Badge: "MAIS POPULAR"**

**Best (Enterprise):**
- Objetivo: Capturar high willingness to pay
- Preço: R$1.000+/mês ou "Fale com vendas"
- Features: Tudo + Enterprise (SSO, SLA, CSM)
- Limites: Ilimitados
- Target: Mid-market, large companies

#### Diferenciação Entre Tiers

**Dimensões:**
1. **Limites quantitativos:** Usuários, contacts, storage, API calls
2. **Features específicas:** Automation (Pro+), API (Pro+), SSO (Enterprise only)
3. **Suporte/SLA:** Email (Starter), Chat (Pro), Phone 24/7 (Enterprise)

**Features que SÃO enterprise (nunca em tiers baixos):**
- SSO (SAML, Okta)
- Audit logs
- RBAC (role-based permissions)
- SLA uptime 99.9%+
- Dedicated CSM
- Custom contract

#### Pricing Gaps: 2-5x Entre Tiers

**Exemplo:**
```
Starter: R$99/mês
Pro: R$499/mês (5x)
Enterprise: R$2.499/mês (5x)
```

**Skill fornece:** Estrutura completa com features por tier, preços específicos, justificativa.

**Referência completa:** `references/tier-structure-guide.md` (~10k palavras)

---

### 5. Cálculo de Preços Específicos

**Skill combina 3 abordagens:**

#### A. Value-Based (Baseline)

**Processo:**
1. Elicitar valor econômico criado
2. Quantificar em R$
3. Calcular 10-30%

**Exemplo de diálogo:**
```
Skill: "Quanto tempo seu produto economiza para cliente?"
User: "Uns 10 horas por semana"
Skill: "Custo médio/hora desse tempo?"
User: "R$100/hora"
Skill: "10h × 4 semanas × R$100 = R$4.000/mês de valor
        Pricing ideal: R$400-R$1.200/mês (10-30%)"
```

#### B. Competitor-Based (Validação)

**Benchmarking:**
- Analisar 5 competidores
- Range: R$X - R$Y
- Posicionar dentro/fora do range

**Exemplo:**
```
Competidores: R$300-R$800/mês
Recomendação: R$499/mês (middle, parity)
```

#### C. Brasil PPP (Se Aplicável)

**Para produto global entrando no Brasil:**

**Fórmula:**
```
Preço BR = Preço US × PPP ratio × Câmbio
```

**SMB:** PPP 0.4 (60% desconto)
**Mid-market:** PPP 0.5 (50% desconto)
**Enterprise:** PPP 0.6 (40% desconto)

**Exemplo:**
```
Preço US: US$100/mês
Preço BR (SMB): US$100 × 0.4 × R$5 = R$200/mês
Preço BR (Enterprise): US$100 × 0.6 × R$5 = R$300/mês
```

**Skill fornece:** Cálculos concretos para caso do usuário, com justificativa.

**Referência completa:** `references/brazil-context.md` (~7k palavras)

---

### 6. Research de Willingness to Pay

**Skill recomenda metodologias baseadas em estágio e recursos:**

#### Para Early-Stage (0-100 clientes)

**Metodologia: Customer Interviews (10-20)**
- Descobrir valor percebido
- Quantificar ROI
- Validar range inicial

**Metodologia: Van Westendorp PSM (100-200 respondentes)**
- 4 perguntas sobre preço
- Descobrir range aceitável (PMC - PME)
- Optimal Price Point (OPP)

#### Para Growth (100-1k clientes)

**Metodologia: Win/Loss Analysis (20-50 entrevistas)**
- Por que clientes compraram vs. não compraram
- Objeções de preço
- Comparação com competidores

**Metodologia: A/B Testing**
- Testar 2-3 preços
- Medir revenue/visitor
- 1.000+ visitors mínimo

#### Para Scale (1k+ clientes)

**Metodologia: Conjoint Analysis (500+ respondentes)**
- Valor relativo de features
- WTP por feature
- Otimizar tiers

**Metodologia: Cohort Analysis (Dados internos)**
- Segmentar por indústria, tamanho, região
- ACV médio por segmento
- Churn por segmento

**Skill fornece:** Roteiro específico, templates de survey, análise de resultados.

**Referência completa:** `references/willingness-to-pay.md` (~8k palavras)

---

### 7. Testing de Preços

**Skill recomenda metodologia de teste baseada em contexto:**

#### A/B Test (Se Tem Volume)

**Setup:**
- 50% tráfego: Preço A
- 50% tráfego: Preço B
- Duração: 1-2 meses
- Mínimo: 1.000 visitors, 100 conversions/variante

**Métrica primária:** Revenue per visitor (NÃO conversion rate).

**Exemplo:**
```
Preço A (R$99): 10% conversion = R$9,90/visitor
Preço B (R$149): 7% conversion = R$10,43/visitor
Vencedor: Preço B (+5% revenue)
```

#### New Customer Test (Mais Seguro)

**Setup:**
- Clientes existentes: Mantêm preço atual
- Novos clientes: 50% Preço A, 50% Preço B
- Sem risco com base existente

#### Grandfathered Test (Para Aumentos)

**Setup:**
- Aumentar preço para novos clientes
- Manter (grandfather) para existentes
- Medir conversion de novos + retention de antigos

**Skill fornece:** Setup específico, cálculo de sample size, análise de resultados.

**Referência completa:** `references/price-testing-methodology.md` (~8k palavras)

---

### 8. Aumentos de Preço

**Skill guia processo de aumento sem churnar clientes:**

#### Quando Aumentar

**Timing ideal:**
- ✅ Após adicionar valor significativo (novas features)
- ✅ NPS alto (50+)
- ✅ Aniversário/marco
- ❌ Logo após outage/problema
- ❌ Em recessão

#### Quanto Aumentar

**Benchmarks:**
- **10-15%:** Pequeno, defensável (inflação), churn ~2-3%
- **20-30%:** Médio, precisa justificativa forte, churn ~5-10%
- **50%+:** Grande, alto risco, churn ~10-20%, considerar grandfathering

#### Estratégias

**1. Aumento Uniforme:**
- Todos os clientes
- Simples, mas churn máximo

**2. Grandfathering Permanente:**
- Existentes mantêm preço antigo
- Novos pagam novo preço
- Zero churn, mas deixa revenue na mesa

**3. Grandfathering Temporário (Recomendado):**
- Existentes mantêm R$99 por 12 meses
- Depois aumenta para R$149
- Reduz churn imediato, dá tempo para adaptar

**4. Tier Upgrade:**
- Não aumenta preço atual
- Cria tier superior com features novas
- Upsell opcional

#### Comunicação

**Princípios:**
- **Aviso prévio:** 30-90 dias
- **Explicar "por quê":** Features novas, inflação, investimentos
- **Mostrar valor:** Relembrar ROI criado
- **Ser transparente:** Honestidade > marketing speak

**Template de email fornecido pela skill.**

**Skill fornece:** Estratégia customizada, template de comunicação, previsão de churn, táticas de retenção.

**Referência completa:** `references/price-increases-playbook.md` (~8k palavras)

---

### 9. Localização para Brasil

**Skill especializada em adaptações para mercado brasileiro:**

#### Ajuste de Preço por PPP

**Não fazer:** Conversão direta (US$ × câmbio = R$)

**Fazer:** Ajuste por purchasing power parity

**Fórmulas:**
```
SMB: Preço BR = Preço US × 0.4 × câmbio (60% desconto)
Mid: Preço BR = Preço US × 0.5 × câmbio (50% desconto)
Enterprise: Preço BR = Preço US × 0.6 × câmbio (40% desconto)
```

**Benchmarks:** Brasil paga 40-60% do preço USD (em equivalent BRL).

#### Métodos de Pagamento

**Obrigatórios:**
- ✅ **PIX** (75% dos brasileiros, grátis, instantâneo)
- ✅ **Cartão com parcelamento** (12x sem juros é esperado)
- ✅ **Boleto** (para B2B empresas grandes)

**Gateways:** Stripe (global), PagSeguro, Mercado Pago, Iugu, Asaas.

#### Nota Fiscal (B2B Obrigatória)

**Se empresa BR (CNPJ):**
- Emitir NF-e via software (Conta Azul, Bling)
- ISS: 2-5% sobre faturamento

**Se empresa estrangeira (sem CNPJ):**
- Opção 1: Partner brasileiro revende
- Opção 2: Abrir subsidiária BR
- Opção 3: Cliente importa (complexo)

**Skill coleta:** CNPJ, Razão Social, Endereço (no checkout B2B).

#### Competição Local

**Principais competidores BR:**
- **CRM:** RD Station (R$200-R$1.500), Moskit (R$120-R$400), Ploomes
- **E-commerce:** VTEX, Nuvemshop, Yampi
- **Gestão:** ContaAzul, Omie, TOTVS

**Skill benchmarka** contra competidores locais, recomenda posicionamento.

#### Cultura de Negociação

**Brasileiro espera desconto.**

**Táticas:**
- Preço com margem para desconto (R$599 → "especial R$499")
- Volume discounts (6-10 users: 10% off)
- Desconto anual (20% off)

**Skill fornece:** Pricing localizado, métodos de pagamento, compliance fiscal, estratégia competitiva.

**Referência completa:** `references/brazil-context.md` (~7k palavras)

---

### 10. Psicologia de Pricing

**Skill aplica táticas psicológicas comprovadas:**

#### Principais Táticas

**1. Anchoring (Ancoragem):**
- Mostrar tier mais caro primeiro
- Tier intermediário parece "razoável"

**2. Charm Pricing:**
- R$99 vs. R$100 (left-digit effect)
- Usar .99 para SMB, números redondos para enterprise

**3. Decoy Pricing:**
- Tier intermediário com má relação custo/benefício
- Empurra para tier superior

**4. Loss Aversion:**
- Trial termina: "Você vai PERDER acesso a 47 documentos criados"

**5. Social Proof:**
- Badge "MAIS POPULAR" no tier target
- "Escolhido por 10.000+ empresas"

**Skill combina 2-3 táticas** (não todas, para evitar manipulação).

**Referência completa:** `references/pricing-psychology.md` (~10k palavras)

---

## Workflow de Uso

### Caso 1: Definir Pricing Inicial

**User:** "Estou lançando um CRM para SMB no Brasil. Como definir preço?"

**Skill executa:**

**Passo 1: Elicitar contexto**
- Estágio: Pre-launch
- B2B, SMB (1-20 funcionários)
- CRM para vendas
- Brasil apenas

**Passo 2: Aplicar frameworks**
- Value-Based: Quantificar valor econômico (tempo economizado)
- Competitor-Based: Benchmarking (RD Station, Moskit)
- Regional: Ajuste PPP para Brasil

**Passo 3: Calcular preços**
```
Valor criado: R$2.100/mês (economiza 1h/dia vendedor)
Pricing: R$200-R$600/mês (10-30%)
Competidores: R$120-R$600/mês
Recomendação:
  Starter: R$199/mês
  Pro: R$499/mês (MAIS POPULAR)
  Business: R$999/mês
```

**Passo 4: Fornecer próximos passos**
- Lançar com esses preços
- Primeiros 20 clientes: Entrevistas
- Mês 3: Van Westendorp survey
- Mês 6: Ajustar baseado em dados

---

### Caso 2: Otimizar Pricing Existente

**User:** "Tenho 500 clientes pagando R$99/mês. Quero aumentar para R$149."

**Skill executa:**

**Passo 1: Elicitar contexto**
- Growth stage (500 clientes)
- B2B ou B2C? (elicita)
- Adicionou features recentemente? (elicita)
- NPS atual? (elicita)

**Passo 2: Avaliar viabilidade**
- Aumento: +50% (grande)
- Se adicionou valor: Justificado
- Se NPS >50: Menor risco de churn

**Passo 3: Recomendar estratégia**
- Grandfathering temporário (12 meses)
- Comunicação 60 dias antes
- Template de email
- Previsão: Churn 5-10%, revenue +35%

**Passo 4: Plano de execução**
- Semana 1-2: Preparar comunicação
- Semana 3: Enviar email anúncio
- Semana 4-8: Responder objeções
- Mês 12: Segundo aumento (para grandfathered)
- Monitorar: Churn rate, complaints, NPS

---

### Caso 3: Localizar para Brasil

**User:** "Meu SaaS custa US$100 nos EUA. Quanto cobrar no Brasil?"

**Skill executa:**

**Passo 1: Ajuste PPP**
```
US$100 × 0.4 (SMB) × R$5 = R$200/mês
ou
US$100 × 0.5 (Mid) × R$5 = R$250/mês
```

**Passo 2: Benchmarking local**
- Competidores BR: R$150-R$400/mês
- R$200-R$250 está competitivo

**Passo 3: Implementação BR**
- Preço em Reais (não dólar)
- PIX + Cartão parcelado (12x)
- Nota Fiscal (CNPJ ou partner)
- Website/checkout em PT-BR

**Passo 4: Go-to-market**
- Estratégia: Disruptor (R$200, 30% mais barato) ou Parity (R$300)
- Margem para desconto (cultura de negociação)
- Comunicação localizada

---

## Resources

Esta skill inclui recursos extensivos organizados em 3 diretórios:

### references/

**8 arquivos de referência (~83k palavras):**

1. **pricing-frameworks.md** (~20k) - 10 frameworks detalhados
2. **value-metrics-models.md** (~12k) - 6 modelos de cobrança
3. **pricing-psychology.md** (~10k) - 15 táticas psicológicas
4. **willingness-to-pay.md** (~8k) - 7 metodologias de pesquisa
5. **tier-structure-guide.md** (~10k) - Estruturação de tiers
6. **price-testing-methodology.md** (~8k) - 7 métodos de teste
7. **price-increases-playbook.md** (~8k) - Como aumentar preços
8. **brazil-context.md** (~7k) - Especificidades do mercado BR

**Uso:** Claude carrega esses arquivos no contexto quando necessário para fundamentar recomendações.

### assets/

**Templates práticos (a serem criados conforme necessidade):**

- Pricing strategy canvas
- Van Westendorp survey template
- Price increase email templates
- Brazil pricing calculator

**Uso:** Fornecidos ao usuário como ferramentas práticas.

### scripts/

**Não aplicável para esta skill** (pricing é consultoria, não automação executável).

---

## Guidelines de Uso para AI

**Para usar esta skill efetivamente:**

### 1. SEMPRE Elicitar Primeiro

Nunca assumir. Sempre perguntar:
- Estágio, modelo (B2B/B2C), produto, geografia
- Pergunta específica do usuário

### 2. Ser Específico e Quantificado

**Ruim:** "Considere aumentar preço."
**Bom:** "Aumente de R$99 para R$149 (+50%). Grandfathering por 12 meses. Churn esperado: 5-10%. Revenue líquido: +35%."

### 3. Usar Frameworks e Dados

Referenciar:
- Frameworks específicos (ex: "Framework de Value-Based Pricing, Patrick Campbell")
- Benchmarks concretos (ex: "CRM SMB no Brasil: R$120-R$600/mês")
- Cases reais (ex: "Slack fez X, resultado Y")

### 4. Adaptar para Brasil Quando Relevante

Se usuário é BR ou quer entrar no mercado:
- Ajustar por PPP (40-60% desconto)
- Mencionar PIX, Boleto, Nota Fiscal
- Comparar com RD Station, Moskit, etc.
- Cultura de desconto/negociação

### 5. Fornecer Próximos Passos

Sempre terminar com:
- Ações concretas: "1. [...] 2. [...] 3. [...]"
- Timeline: "Semana 1 [...], Mês 3 [...]"
- Métricas a monitorar: "Churn rate, NPS, revenue"

---

## Limitações

**Esta skill NÃO pode:**
- Acessar dados internos (usuário precisa compartilhar)
- Fazer pesquisas de mercado automaticamente
- Implementar pricing (consultoria, não execução)
- Garantir resultados (pricing requer testes)

**Esta skill PODE:**
- Recomendar estratégias baseadas em frameworks validados
- Fornecer benchmarks (baseado em conhecimento até 2025)
- Sugerir metodologias de pesquisa e teste
- Criar templates e calculadoras
- Especializações para Brasil

---

## Conclusão

Use esta skill como consultor especializado em pricing de SaaS, com foco em startups brasileiras.

**Pricing é a alavanca #1 de crescimento:**
- 1% de melhoria em pricing = 11% de melhoria em lucro (Patrick Campbell)
- 4x mais impacto que aquisição ou retenção

Vamos otimizar seu pricing! 🚀