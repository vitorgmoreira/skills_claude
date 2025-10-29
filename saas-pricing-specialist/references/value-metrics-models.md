# Value Metrics e Modelos de Cobrança para SaaS

Guia completo sobre value metrics (métricas de valor) e modelos de cobrança: per-user, usage-based, tiered, hybrid e outros.

---

## O Que é Value Metric?

**Value Metric é a unidade pela qual você cobra do cliente.**

**Não é o preço. É a MÉTRICA que determina quanto o cliente paga.**

### Exemplos de Value Metrics

| Produto | Value Metric | Pricing |
|---------|--------------|---------|
| Slack | Usuários ativos mensais | R$30/usuário ativo/mês |
| Stripe | Volume de transações (GMV) | 2.9% + R$0.30 por transação |
| AWS | Compute hours, storage GB | R$X/hora de EC2, R$Y/GB S3 |
| Mailchimp | Número de contatos | R$50 (até 500), R$100 (até 1k), etc. |
| Notion | Membros no workspace | R$40/membro/mês |
| Zapier | Tasks executadas/mês | R$99 (750 tasks), R$299 (2k tasks) |

---

## Por Que Value Metric Importa?

**Value metric é a decisão de pricing mais importante.**

### 1. Alinha Preço com Valor

**Bom value metric:** Cliente paga mais quando recebe mais valor.

**Exemplo:**
- **Stripe:** Quanto mais você vende (GMV), mais você paga. Justo, pois Stripe gera mais valor.
- **AWS:** Quanto mais você usa (compute, storage), mais você paga. Escala com crescimento.

**Mau value metric:** Cliente paga mais, mas não recebe mais valor.

**Exemplo:**
- **CRM cobrando por "projetos criados":** Criar mais projetos não significa mais valor. É arbitrário.

### 2. Facilita Expansion Revenue

**Value metric que cresce com cliente = NRR alto.**

**Exemplo:**
- Cliente começa pequeno: 5 usuários, R$150/mês
- Cliente cresce: 50 usuários, R$1.500/mês
- **Expansion automática de 10x**

### 3. Simplifica Decisão de Compra

**Cliente entende facilmente quanto vai pagar.**

**Bom:** "R$10/usuário/mês. Quantos usuários você tem? 10? Então R$100/mês."

**Ruim:** "Cobramos por uma combinação de usuários ativos, dados processados, e features habilitadas. Preciso de 30 minutos para calcular."

---

## Princípios de um Bom Value Metric (Patrick Campbell)

**Patrick Campbell (ProfitWell) define 3 critérios:**

### 1. Alinha com Valor Percebido

**Métrica cresce quando valor cresce.**

**Exemplo bom:**
- CRM cobra por "usuários de vendas"
- Mais vendedores = mais vendas = mais valor

**Exemplo ruim:**
- CRM cobra por "número de integrações ativadas"
- Mais integrações ≠ mais valor necessariamente

### 2. É Fácil de Entender

**Cliente consegue prever quanto vai pagar.**

**Teste:** Explique em uma frase.
- ✅ "R$50/usuário/mês"
- ✅ "2.9% do GMV"
- ❌ "Baseado em uma fórmula de MAUs ponderados por engagement score"

### 3. Cresce com o Cliente

**Métrica aumenta naturalmente conforme cliente escala.**

**Exemplo:**
- Startup: 5 usuários → R$250/mês
- Scale-up: 50 usuários → R$2.500/mês
- **Você cresce junto com cliente**

---

## Modelo 1: Per-User / Per-Seat Pricing

### Conceito

**Cobra por número de usuários (seats) que usam o produto.**

**Fórmula:**
```
Preço = Número de usuários × Preço por usuário
```

**Exemplos:**
- Slack: R$30/usuário ativo/mês
- Notion: R$40/membro/mês
- Zoom: R$75/host/mês
- Salesforce: R$1.000-R$3.000/usuário/mês

---

### Quando Usar Per-User Pricing

#### ✅ Produto é Colaborativo

**Usuários trabalham juntos, compartilham dados.**

**Exemplos:**
- Slack (comunicação em equipe)
- Notion (documentos compartilhados)
- Figma (design colaborativo)
- Google Workspace (docs, sheets compartilhados)

#### ✅ Cada Usuário Recebe Valor Individual

**Não é só "1 admin usa, 100 veem".**

**Exemplo:**
- CRM: Cada vendedor usa ativamente
- Project management: Cada membro da equipe usa

#### ✅ Número de Usuários Correlaciona com Valor

**Mais usuários = cliente maior = mais valor recebido.**

**Exemplo:**
- 5 usuários = startup
- 500 usuários = empresa grande
- Willingness to pay escala

---

### Variações de Per-User Pricing

#### 1. Usuários Ativos vs. Totais

**Opção A: Cobrar por todos os usuários cadastrados**
- Simples
- Cliente pode ter usuários inativos pagando

**Opção B: Cobrar apenas por usuários ativos (MAU)**
- Mais justo
- Exemplo: Slack cobra só quem usou no mês

**Recomendação:** Usuários ativos (melhor alinhamento com valor).

#### 2. Pricing por Tipo de Usuário

**Nem todo usuário tem mesmo valor.**

**Exemplo: Confluence (Atlassian)**
- Full user: R$200/mês (edita, cria)
- Viewer: R$20/mês (só visualiza)

**Exemplo: Intercom**
- Seat (agent de suporte): R$150/mês
- Viewer (manager): R$50/mês

**Quando usar:** Se há usuários "leves" vs. "pesados".

#### 3. Minimum Seats

**Forçar compra mínima.**

**Exemplo:**
- "Plano Pro: Mínimo 5 usuários, R$50/usuário = R$250/mês"
- Cliente com 3 usuários paga por 5

**Por quê:** Garantir deal size mínimo, evitar clientes muito pequenos.

---

### Vantagens de Per-User Pricing

#### ✅ Previsibilidade

- Cliente sabe exatamente quanto vai pagar
- MRR é estável e previsível

#### ✅ Expansion Natural

- Cliente cresce (contrata) → Mais usuários → Mais receita
- NRR cresce organicamente

#### ✅ Simplicidade

- Fácil explicar
- Fácil calcular
- Fácil fazer upsell ("Adicione mais 5 usuários")

---

### Desvantagens de Per-User Pricing

#### ❌ Incentiva Compartilhamento de Login

**Problema:** Cliente compra 1 licença, 5 pessoas compartilham.

**Solução:**
- Concurrent users (máximo simultâneo)
- Login único obrigatório
- Auditoria de uso

#### ❌ Punição por Crescimento

**Percepção:** "Se eu contratar mais gente, meu custo de SaaS sobe."

**Realidade:** É verdade. Pode criar atrito.

**Exemplo:**
- Empresa quer contratar 10 vendedores
- CRM cobra R$100/usuário
- Custo adicional: R$1k/mês
- CFO: "Por que nosso software fica mais caro?"

#### ❌ Não Captura Diferenças de Valor

**Problema:** Usuário pouco ativo paga igual ao power user.

**Exemplo:**
- Vendedor A: Usa CRM 8h/dia, fecha R$1M/ano
- Vendedor B: Usa 1h/semana, fecha R$100k/ano
- Ambos pagam R$100/mês

**Solução:** Hybrid model (per-user + usage).

---

### Benchmarks de Preço Per-User

**Por categoria:**

| Categoria | Preço/Usuário/Mês (SMB) | Preço/Usuário/Mês (Enterprise) |
|-----------|-------------------------|--------------------------------|
| **Comunicação** (Slack, Teams) | R$30-R$60 | R$60-R$150 |
| **Project Management** (Asana, Monday) | R$40-R$100 | R$100-R$300 |
| **CRM** (HubSpot, Pipedrive) | R$200-R$500 | R$1.000-R$3.000 |
| **Design** (Figma, Adobe) | R$60-R$150 | R$200-R$500 |
| **Storage** (Dropbox, Box) | R$50-R$100 | R$100-R$300 |
| **Analytics** (Mixpanel, Amplitude) | N/A (usage-based) | Custom |

---

### Case Studies de Per-User Pricing

#### Case 1: Slack - Usuários Ativos Mensais

**Modelo:**
- Cobra apenas usuários ativos (usaram no mês)
- R$30-R$60/usuário ativo/mês

**Por que funciona:**
- Justo: Cliente não paga por conta fantasma
- Expansion: Time cresce, mais pessoas usam
- Simplicidade: Fácil entender

**NRR:** ~140% (expansão massiva)

#### Case 2: Salesforce - Per-User Clássico

**Modelo:**
- Cobra por usuário cadastrado (não ativo)
- R$1.000-R$3.000/usuário/mês (Enterprise)

**Por que funciona:**
- Target é enterprise (grande willingness to pay)
- Cada usuário (sales rep) gera muito valor (vendas)
- Switching cost alto (dados, customizações)

**Problemas:**
- SMB acha caro
- Incentiva compartilhamento de login

---

## Modelo 2: Usage-Based Pricing

### Conceito

**Cobra baseado em quanto cliente USA o produto.**

**Fórmula:**
```
Preço = Unidades consumidas × Preço por unidade
```

**Exemplos:**
- Stripe: 2.9% de cada transação
- AWS: R$0.10/hora de EC2, R$0.023/GB de S3
- Twilio: R$0.05/SMS enviado
- Snowflake: R$X/TB de dados processados
- SendGrid: R$0.001/email enviado

---

### Quando Usar Usage-Based Pricing

#### ✅ Uso Varia MUITO entre Clientes

**Exemplo:**
- Cliente A: 100 emails/mês
- Cliente B: 1 milhão emails/mês
- Não faz sentido cobrar preço fixo

#### ✅ Valor é Diretamente Proporcional ao Uso

**Mais uso = mais valor.**

**Exemplo:**
- Twilio: Mais SMS = mais alcance = mais valor
- Stripe: Mais transações = mais receita do cliente = mais valor

#### ✅ Cliente Quer Controle de Custo

**Uso pouco, pago pouco.**

**Atrai clientes que têm medo de commitment.**

---

### Tipos de Usage Metrics

#### 1. Volume-Based (Quantidade)

**Cobra por unidades discretas.**

**Exemplos:**
- Emails enviados (SendGrid)
- SMS enviados (Twilio)
- API calls (Stripe, muitos APIs)
- Transações processadas (Stripe)
- Relatórios gerados (BI tools)

#### 2. Compute-Based (Processamento)

**Cobra por recursos consumidos.**

**Exemplos:**
- Horas de servidor (AWS EC2)
- GB de dados processados (Snowflake)
- Minutos de video (Zoom, Loom)
- CPU/RAM utilizados

#### 3. Storage-Based (Armazenamento)

**Cobra por dados armazenados.**

**Exemplos:**
- GB de storage (AWS S3, Dropbox)
- Número de registros no banco (alguns CRMs)
- Tamanho de repositório (GitHub storage)

#### 4. Transaction-Based (Take Rate)

**Cobra % de cada transação.**

**Exemplos:**
- Stripe: 2.9% + R$0.30
- Shopify Payments: 2.5% GMV
- Marketplace SaaS: 10-30% take rate

---

### Vantagens de Usage-Based Pricing

#### ✅ Alinhamento Perfeito com Valor

- Cliente paga quando recebe valor
- Não há desperdício ("pago só o que uso")

#### ✅ Expansion Automática

- Cliente cresce → Usa mais → Paga mais
- NRR pode ser massivo (Snowflake: 158% NRR)

#### ✅ Atrai Clientes Early-Stage

- Startup pode começar barato (uso baixo)
- Escala conforme cresce
- Reduz barreira de entrada

#### ✅ Previsibilidade de Custo (para cliente)

- Controle total: "Vou enviar 10k emails, vai custar R$100"
- Não há surpresas (se monitorar uso)

---

### Desvantagens de Usage-Based Pricing

#### ❌ Revenue Imprevisível (para vendor)

**Problema:** MRR varia todo mês.

**Exemplo:**
- Janeiro: Cliente usa 100k API calls = R$1k
- Fevereiro: Cliente usa 50k = R$500
- **Churn negativo? Ou só usou menos?**

**Solução:** Hybrid (base fee + usage).

#### ❌ Bill Shock (Susto na Conta)

**Problema:** Cliente usa mais que esperava, recebe conta alta.

**Exemplo:**
- AWS: Cliente esquece de desligar servidor, conta de R$10k
- Reputação ruim, churn

**Solução:**
- Alertas de uso
- Caps (limite de spend)
- Transparency (dashboard de uso em tempo real)

#### ❌ Complexidade de Billing

**Problema:** Calcular uso, faturar, disputas.

**Exemplo:**
- "Você cobrou 10.347 API calls, mas eu contei 9.982"
- Requer infraestrutura de metering/billing robusta

#### ❌ Incentiva Uso Eficiente (Menos Revenue)

**Problema:** Cliente otimiza para usar menos.

**Exemplo:**
- Cliente de AWS otimiza código, usa 50% menos compute
- AWS perde 50% da receita desse cliente

**Isso é contra-intuitivo para SaaS (queremos que usem mais).**

---

### Benchmarks de Usage-Based Pricing

**Por tipo de serviço:**

| Serviço | Métrica | Preço Típico |
|---------|---------|--------------|
| **Email (SendGrid)** | Emails enviados | R$0.001-R$0.01/email |
| **SMS (Twilio)** | SMS enviado | R$0.05-R$0.15/SMS |
| **Payment Processing (Stripe)** | % GMV | 2.5-3.5% + taxa fixa |
| **Cloud Storage (AWS S3)** | GB armazenado | R$0.023/GB/mês |
| **Cloud Compute (AWS EC2)** | Hora de servidor | R$0.10-R$5/hora |
| **Data Warehouse (Snowflake)** | TB processado | R$100-R$200/TB |
| **API calls** | Por 1.000 calls | R$1-R$50/1k calls |

---

### Case Studies de Usage-Based Pricing

#### Case 1: Snowflake - Pure Usage

**Modelo:**
- Cobra por TB de dados processados
- Sem commitment mínimo
- Pay-as-you-go

**Por que funciona:**
- Uso varia 100x entre clientes
- Cliente paga só quando usa (atrai startups)
- Expansion massiva (cliente processa mais dados)

**NRR:** 158% (líder da indústria)

**Problema:**
- Revenue volatility
- Solução: Contratos anuais com consumption commitment

#### Case 2: Stripe - Transaction-Based

**Modelo:**
- 2.9% + R$0.30 por transação
- Zero custo fixo

**Por que funciona:**
- Alinhamento perfeito: Cliente vende mais, Stripe ganha mais
- Barreira de entrada zero (startups adoram)
- Expansion automática

**NRR:** ~120%+

#### Case 3: AWS - Múltiplas Métricas

**Modelo:**
- Compute: R$/hora
- Storage: R$/GB
- Transfer: R$/GB transferido
- Centenas de serviços, cada um com própria métrica

**Por que funciona:**
- Granularidade: Cliente paga exatamente pelo que usa
- Escala: De R$10/mês (hobby) a R$10M/mês (enterprise)

**Problema:**
- Complexidade extrema
- Bill shock comum
- Necessita expertise para otimizar custos (daí surgiram startups como CloudHealth)

---

## Modelo 3: Tiered / Feature-Based Pricing

### Conceito

**Oferecer múltiplos tiers (planos) com diferentes features e preços.**

**Estrutura clássica: Good - Better - Best**

**Exemplo:**

| Tier | Preço | Features |
|------|-------|----------|
| **Starter** | R$99/mês | Features básicas, 5 usuários |
| **Professional** | R$499/mês | Features avançadas, 25 usuários |
| **Enterprise** | Custom | Tudo + SSO, SLA, suporte 24/7 |

---

### Quando Usar Tiered Pricing

#### ✅ Clientes Têm Necessidades Diferentes

**Não é one-size-fits-all.**

**Exemplo:**
- SMB: Quer básico, barato
- Mid-market: Precisa integrações, analytics
- Enterprise: Precisa SSO, compliance, SLA

#### ✅ Quer Capturar Múltiplos Segmentos

**Maximizar TAM (Total Addressable Market).**

**Exemplo:**
- Tier baixo: R$99 → Atrai SMB
- Tier médio: R$499 → Mid-market
- Tier alto: R$5k+ → Enterprise

#### ✅ Upsell é Parte da Estratégia

**Land em tier baixo, expand para tier alto.**

**Exemplo:**
- Cliente começa em Starter
- Cresce, precisa de features avançadas
- Upgrade para Pro

---

### Estrutura de Tiers

#### Regra: 3-4 Tiers é Ótimo

**Por quê:**
- Muito pouco (2 tiers): Não captura segmentos diferentes
- Muito (5+ tiers): Confuso, paralisia de escolha

**Estrutura recomendada:**

**Opção A: 3 Tiers (Clássico)**
1. **Starter / Basic**: SMB, entrada
2. **Professional / Pro**: Mid-market, mais popular
3. **Enterprise**: Large companies, custom

**Opção B: 4 Tiers (Com Free)**
1. **Free**: Freemium, viralidade
2. **Starter**: SMB convertido
3. **Professional**: Mid-market
4. **Enterprise**: Large

---

### Diferenciação Entre Tiers

**O que muda de um tier para outro?**

#### 1. Limites Quantitativos

**Caps em uso.**

**Exemplos:**
- Starter: 1.000 contatos
- Pro: 10.000 contatos
- Enterprise: Ilimitado

**Ou:**
- Starter: 5 usuários
- Pro: 25 usuários
- Enterprise: Ilimitado

#### 2. Features Específicas

**Features premium em tiers altos.**

**Padrão comum:**

**Starter:**
- Core features
- Email suporte

**Pro:**
- Core + Advanced features
- Integrações
- Analytics/reporting
- Priority support

**Enterprise:**
- Tudo do Pro +
- SSO (SAML, Okta)
- Admin controls (RBAC, permissions)
- API avançado
- SLA uptime
- Dedicated CSM
- Audit logs
- Custom integrações

#### 3. Suporte

**Níveis de SLA.**

**Starter:**
- Email support (resposta em 48h)

**Pro:**
- Priority email (resposta em 12h)
- Chat support

**Enterprise:**
- 24/7 phone support
- Dedicated CSM
- SLA de uptime 99.9%+
- Resposta <2h

---

### Psicologia de Tiered Pricing

#### Efeito Âncora (Anchoring)

**Tier mais caro "ancora" percepção.**

**Exemplo:**
- Tier 1: R$99
- Tier 2: R$499
- Tier 3: R$2.499 (anchoring)

**Resultado:** Tier 2 parece "razoável" (nem muito barato, nem caro).

#### Efeito Decoy (Isca)

**Criar tier intermediário para empurrar para tier superior.**

**Exemplo:**
- Tier 1: R$99 (50 contatos)
- Tier 2: R$299 (500 contatos) ← Decoy (má relação custo/benefício)
- Tier 3: R$399 (5.000 contatos) ← Melhor valor!

**Resultado:** Cliente compara Tier 2 vs 3, escolhe 3.

#### Posicionamento do "Popular"

**Destacar tier que você quer que maioria compre.**

**Exemplo:**
```
[ Starter ]    [✨ Pro - POPULAR ✨]    [ Enterprise ]
  R$99/mês           R$499/mês              Custom
```

**Badge "Popular" aumenta conversion para esse tier.**

---

### Good-Better-Best Pricing

**Framework clássico de 3 tiers.**

#### Good (Entrada)

**Objetivo:** Barreira de entrada baixa, atrair SMB.

**Características:**
- Features core
- Limites apertados
- Preço: R$50-R$200/mês
- Target: Freelancers, small teams

**Exemplo:** Mailchimp Free (até 500 contatos).

#### Better (Mais Popular)

**Objetivo:** Tier que maioria compra. Onde você quer mais clientes.

**Características:**
- Features avançadas
- Limites generosos
- Preço: R$200-R$1.000/mês
- Target: SMB, mid-market

**Exemplo:** Mailchimp Standard (R$500/mês).

#### Best (Premium)

**Objetivo:** Capturar clientes enterprise com alto willingness to pay.

**Características:**
- Features enterprise (SSO, SLA)
- Sem limites ou altíssimos
- Preço: R$1.000+/mês ou custom
- Target: Enterprise, large teams

**Exemplo:** Mailchimp Premium (custom pricing).

---

### Vantagens de Tiered Pricing

#### ✅ Captura Múltiplos Segmentos

- SMB, mid-market, enterprise
- Maximiza TAM

#### ✅ Upsell Built-in

- Cliente começa em tier baixo
- Naturalmente faz upgrade conforme cresce

#### ✅ Simplicidade para Cliente

- Escolhe plano que faz sentido
- Features claras por tier

---

### Desvantagens de Tiered Pricing

#### ❌ Paralisia de Escolha

**Muitos tiers = confusão.**

**Exemplo:**
- 5 tiers, cada um com 20 features diferentes
- Cliente não sabe qual escolher
- Desiste

**Solução:** Máximo 3-4 tiers, diferenças claras.

#### ❌ "Good Enough" Problem

**Tier básico é suficiente, ninguém faz upgrade.**

**Exemplo:**
- Free tier do Mailchimp (500 contatos) é suficiente para muitos
- Conversion baixa (<2%)

**Solução:** Limitar free tier, forçar upgrade.

#### ❌ Difícil Definir Diferenciação

**Quais features em qual tier?**

**Erro comum:**
- Tier básico muito limitado (ninguém compra)
- Tier premium não tem features suficientemente valiosas (ninguém faz upgrade)

**Solução:** Testar, iterar baseado em dados.

---

### Benchmarks de Tiered Pricing

**Estrutura típica:**

| Tier | Preço Típico | Target | % de Clientes |
|------|--------------|--------|---------------|
| **Free** | R$0 | Freemium, viral | 90-95% (se freemium) |
| **Starter** | R$50-R$200/mês | SMB, small teams | 40-60% (dos pagos) |
| **Professional** | R$200-R$1k/mês | Mid-market | 30-50% (dos pagos) |
| **Enterprise** | R$1k+/mês | Large companies | 10-20% (dos pagos, mas 50%+ da receita) |

---

### Case Studies de Tiered Pricing

#### Case 1: HubSpot - 3 Tiers Clássicos

**Estrutura:**
- **Starter:** R$200/mês (small teams)
- **Professional:** R$2k/mês (mid-market) ← Mais popular
- **Enterprise:** R$10k+/mês (large companies)

**Diferenciação:**
- Starter: Core CRM, email, forms
- Pro: Automation, reporting, integrações
- Enterprise: Custom objects, SSO, SLA

**Resultado:**
- Pro tier: 50% dos clientes
- Enterprise tier: 20% dos clientes, 60% da receita

#### Case 2: Notion - Segmentação por Uso

**Estrutura:**
- **Free:** Uso pessoal
- **Plus:** R$40/usuário (small teams)
- **Business:** R$75/usuário (companies)
- **Enterprise:** Custom (large orgs)

**Diferenciação:**
- Free vs. Plus: Collaboration features
- Plus vs. Business: Admin controls, analytics
- Business vs. Enterprise: SSO, SLA, advanced security

**Estratégia:** Land no Free (viralidade), expand para Plus/Business.

---

## Modelo 4: Hybrid Pricing (Combinação)

### Conceito

**Combinar múltiplos value metrics.**

**Exemplos de híbridos:**
1. **Base fee + Usage:** R$X/mês + R$Y por unidade
2. **Per-user + Tiers:** R$X/usuário, mas tier define features
3. **Per-user + Usage caps:** R$X/usuário com limite de uso
4. **Tiered + Usage overages:** Plano inclui X unidades, depois cobra por overage

---

### Quando Usar Hybrid Pricing

#### ✅ Clientes Variam em Tamanho E Uso

**Exemplo:**
- Cliente A: 5 usuários, 10k API calls/mês
- Cliente B: 50 usuários, 100k API calls/mês
- Cliente C: 5 usuários, 500k API calls/mês

**Só per-user:** Não captura valor de Cliente C.
**Só usage:** Não captura valor de equipe grande (Cliente B).
**Hybrid:** Captura ambos.

#### ✅ Quer Garantir Base Revenue + Upside

**Base fee:** MRR previsível.
**Usage:** Upside quando cliente usa mais.

#### ✅ Reduzir Volatilidade de Pure Usage

**Pure usage:** MRR varia muito mês a mês.
**Hybrid:** Base fee estabiliza, usage adiciona crescimento.

---

### Modelos de Hybrid Pricing

#### Modelo 1: Base Fee + Usage Overage

**Estrutura:**
- Plano inclui X unidades
- Uso acima de X: Cobra overage

**Exemplo: Zapier**
- **Starter:** R$99/mês (inclui 750 tasks)
- Overage: R$0.10/task adicional

**Exemplo: Mailchimp**
- **Standard:** R$500/mês (inclui 5k contatos)
- Overage: R$0.05/contato adicional

**Vantagens:**
- Cliente tem previsibilidade (base fee)
- Vendor tem upside (overages)

**Desvantagens:**
- Overages podem gerar bill shock

#### Modelo 2: Per-User com Usage Caps

**Estrutura:**
- Cobra por usuário
- Mas cada usuário tem limite de uso

**Exemplo: Figma**
- R$60/editor/mês
- Cada editor: 3 projetos ativos
- Projetos adicionais: +R$20/projeto

**Exemplo hipotético: CRM**
- R$100/usuário/mês
- Cada usuário: Até 1k API calls/mês
- API calls adicionais: R$0.01/call

#### Modelo 3: Tiered com Usage Incluído

**Estrutura:**
- Tiers definem features E allowance de uso
- Overage se exceder

**Exemplo: Vercel**
- **Hobby:** Grátis (100GB bandwidth)
- **Pro:** R$100/mês (1TB bandwidth)
- **Enterprise:** Custom (ilimitado)
- Overage: R$40/100GB adicional

#### Modelo 4: Per-User + Tiers de Features

**Estrutura:**
- Preço base por usuário
- Tiers definem quais features

**Exemplo: Slack**
- **Pro:** R$30/usuário ativo/mês
- **Business+:** R$60/usuário ativo/mês
- **Enterprise Grid:** Custom/usuário

**Diferença entre tiers:**
- Pro: Features básicas
- Business+: SSO, compliance
- Grid: Ilimitado workspaces, advanced admin

---

### Vantagens de Hybrid Pricing

#### ✅ Captura Valor de Múltiplas Dimensões

- Tamanho do time (per-user)
- Intensidade de uso (usage)
- Sofisticação (tier/features)

#### ✅ Revenue Previsível + Upside

- Base fee: MRR estável
- Usage/overages: Expansion

#### ✅ Flexibilidade

- Se adapta a clientes diversos

---

### Desvantagens de Hybrid Pricing

#### ❌ Complexidade

**Cliente pode ficar confuso.**

**Exemplo ruim:**
- "R$50/usuário/mês, mais R$0.01/API call, mais R$10/GB de storage, mais tier de features (Basic vs. Pro)"
- **Muito complicado!**

**Solução:** Máximo 2 dimensões (ex: per-user + tier).

#### ❌ Harder to Compare com Competidores

**Dificulta price shopping.**

**Exemplo:**
- Competidor A: R$100/usuário
- Você: R$50/usuário + R$0.05/transação
- **Qual é mais barato? Depende do uso.**

---

### Case Studies de Hybrid Pricing

#### Case 1: Intercom - Per-Seat + Usage (Conversas)

**Modelo antigo (até 2018):**
- Só per-user (R$150/seat)

**Problema:**
- Cliente com muito tráfego (muitas conversas) pagava igual a cliente com pouco
- Não capturava valor

**Modelo novo (2018+):**
- Base fee por seat: R$150/seat/mês
- + Cobrança por "conversations" resolvidas
- Overage: R$1-R$5/conversa (dependendo do tier)

**Resultado:**
- Revenue +40% no primeiro ano
- Melhor alinhamento com valor (empresas grandes com muito suporte pagam mais)

**Backlash:**
- Muitos clientes reclamaram (bill shock)
- PR ruim
- Intercom teve que fazer grandfathering

**Lição:** Hybrid funciona, mas comunicação é crítica.

#### Case 2: GitHub - Per-User + Tiers

**Modelo:**
- **Free:** Grátis (unlimited public repos)
- **Team:** R$20/usuário/mês (private repos, features de time)
- **Enterprise:** R$100/usuário/mês (SSO, audit logs, SLA)

**Híbrido:**
- Per-user (escala com time)
- + Tiers (segmenta por sofisticação)

**Por que funciona:**
- Freemium viral (open source)
- Land & expand (free → team → enterprise)

---

## Modelo 5: Freemium + Paid Tiers

### Conceito

**Tier Free + Tiers Paid.**

**Já coberto em Frameworks (Freemium), mas aqui focamos no pricing dos tiers pagos.**

**Estrutura:**
1. **Free:** Funcionalidade limitada
2. **Paid Tiers:** 2-3 opções pagas

---

### Estrutura de Freemium + Paid

**Exemplo: Notion**

| Tier | Preço | Limite | Target |
|------|-------|--------|--------|
| **Personal Free** | R$0 | Uso individual | Pessoas, estudantes |
| **Plus** | R$40/usuário | Small teams | Startups, pequenas empresas |
| **Business** | R$75/usuário | Companies | Mid-market |
| **Enterprise** | Custom | Large orgs | Enterprise |

**Estratégia:**
- Free: Viralidade, educação de mercado
- Plus: Primeira conversion (R$40 é acessível)
- Business: Upsell (mais features, admin)
- Enterprise: Large deals (SSO, SLA)

---

## Modelo 6: Per-Transaction (Take Rate)

### Conceito

**Cobra % de cada transação que passa pela plataforma.**

**Comum em marketplaces e payment processors.**

**Fórmula:**
```
Receita = GMV (Gross Merchandise Value) × Take Rate %
```

---

### Quando Usar Take Rate

#### ✅ Você Facilita Transações

**Exemplos:**
- Payment processor (Stripe)
- Marketplace (Airbnb, Uber)
- E-commerce platform (Shopify Payments)

#### ✅ Alinhamento Perfeito com Valor

**Cliente vende mais → Você ganha mais.**

---

### Benchmarks de Take Rate

**Por indústria:**

| Tipo | Take Rate | Exemplo |
|------|-----------|---------|
| **Payment Processing** | 2-3% + taxa fixa | Stripe, PayPal |
| **E-commerce (Shopify)** | 2-3% (se usar Shopify Payments) | Shopify |
| **Marketplace (dois lados)** | 10-30% | Airbnb (14%), Uber (25%), Etsy (6.5%) |
| **Fintech** | 1-5% | Wise, Remitly |
| **Delivery** | 15-30% | iFood, Uber Eats |

---

### Vantagens de Take Rate

#### ✅ Alinhamento com Sucesso do Cliente

- Você só ganha se cliente ganha

#### ✅ Expansion Automática

- Cliente vende R$10k/mês → Você ganha R$300
- Cliente vende R$1M/mês → Você ganha R$30k

#### ✅ Barreira de Entrada Baixa

- Sem custo fixo, startups adoram

---

### Desvantagens de Take Rate

#### ❌ Revenue Volátil

- Varia com GMV do cliente

#### ❌ Incentiva Disintermediação

**Cliente quer evitar take rate.**

**Exemplo:**
- Marketplace conecta vendedor e comprador
- Depois da 1ª transação, fazem transações diretas (fora da plataforma)
- Marketplace perde take rate

**Solução:** Lock-in via pagamentos, garantias, reputação.

---

## Escolhendo o Value Metric Certo

### Framework de Decisão

**Perguntas para fazer:**

#### 1. Como cliente percebe valor?

**Exemplo:**
- CRM: Valor está em fechar vendas → Per-user (vendedores) faz sentido
- Analytics: Valor está em insights de dados → Usage (dados processados) faz sentido

#### 2. O que escala quando cliente cresce?

**Exemplo:**
- Time cresce → Per-user
- Volume de negócios cresce → Usage (transações, API calls)

#### 3. O que cliente consegue prever?

**Exemplo:**
- Número de funcionários: Fácil prever
- API calls por mês: Mais difícil

**Se difícil prever → Pode causar bill shock.**

#### 4. Como competidores cobram?

**Benchmarking:**
- Se todos no mercado cobram per-user, cliente está acostumado
- Mudar para usage-based pode confundir

**Mas:** Oportunidade de diferenciar.

---

### Matriz de Decisão

| Se... | Então considere... |
|-------|-------------------|
| Produto é colaborativo, valor por pessoa | **Per-user** |
| Uso varia muito entre clientes (10x-100x) | **Usage-based** |
| Clientes têm necessidades diferentes (SMB vs. Enterprise) | **Tiered** |
| Ambos (time varia E uso varia) | **Hybrid (per-user + usage)** |
| Você facilita transações financeiras | **Take rate** |

---

## Erros Comuns em Value Metrics

### Erro 1: Métrica Não Correlaciona com Valor

**Exemplo ruim:** CRM cobrando por "número de dashboards criados".

**Problema:** Criar dashboards não = mais vendas.

**Solução:** Cobrar por usuários (vendedores) ou deals fechados.

### Erro 2: Métrica Difícil de Entender

**Exemplo ruim:** "Cobramos por MAUs ponderados por engagement score ajustado por segmento".

**Problema:** Cliente não entende quanto vai pagar.

**Solução:** Simplicidade. "R$X/usuário ativo" é claro.

### Erro 3: Métrica Incentiva Comportamento Errado

**Exemplo ruim:** Cobrar por "número de emails enviados" em ferramenta de email marketing.

**Problema:** Cliente envia menos emails para economizar → Pior resultado.

**Solução:** Cobrar por "número de contatos" (não penaliza enviar mais emails).

### Erro 4: Muito Granular (Múltiplas Métricas)

**Exemplo ruim:** "R$10/usuário + R$0.01/API call + R$5/GB storage + R$2/integração ativa".

**Problema:** Confusão, difícil calcular.

**Solução:** Máximo 2 dimensões.

---

## Checklist de Value Metric

**Ao definir seu value metric, perguntar:**

- [ ] **Alinha com valor percebido?** Cliente que recebe mais valor paga mais?
- [ ] **É fácil de entender?** Consigo explicar em 1 frase?
- [ ] **É previsível?** Cliente consegue estimar quanto vai pagar?
- [ ] **Cresce com cliente?** Métrica aumenta quando cliente escala?
- [ ] **É fácil de medir/meter?** Consigo trackear uso com precisão?
- [ ] **Competidores usam similar?** Ou há oportunidade de diferenciar?
- [ ] **Evita bill shock?** Não gera surpresas ruins na conta?

**Se resposta for "SIM" para maioria, seu value metric é sólido.**

---

## Conclusão: Recomendação por Tipo de SaaS

| Tipo de SaaS | Value Metric Recomendado | Exemplo |
|--------------|--------------------------|---------|
| **Comunicação/Colaboração** | Per-user (usuários ativos) | Slack, Notion |
| **CRM/Sales** | Per-user (sales reps) | Salesforce, Pipedrive |
| **Project Management** | Per-user | Asana, Monday |
| **Infrastructure (Cloud)** | Usage (compute, storage) | AWS, GCP |
| **Data/Analytics** | Usage (dados processados) | Snowflake, Databricks |
| **API/Developer Tools** | Usage (API calls) | Stripe API, Twilio |
| **Marketing Automation** | Hybrid (contacts + emails) | Mailchimp, ActiveCampaign |
| **E-commerce Platform** | Hybrid (base fee + % GMV) | Shopify |
| **Payment Processing** | Take rate (% transação) | Stripe, PayPal |
| **Design Tools** | Per-user (editors) | Figma, Adobe |

**Regra geral:**
- **B2B collaboration:** Per-user
- **Infrastructure/API:** Usage-based
- **Diversos segmentos:** Tiered ou Hybrid

---

**Próximo arquivo:** `pricing-psychology.md` (táticas psicológicas: anchoring, charm pricing, decoy, framing)