# Guia de Estruturação de Tiers para SaaS

Guia completo sobre como estruturar tiers de pricing: quantos criar, quais features incluir, naming, Good-Better-Best framework, packaging e otimização.

---

## Por Que Tiered Pricing?

**Tiered pricing = Oferecer múltiplos planos com diferentes features e preços.**

**Benefícios:**

1. **Captura múltiplos segmentos**
   - SMB, mid-market, enterprise
   - Maximiza Total Addressable Market (TAM)

2. **Natural upgrade path**
   - Cliente começa pequeno, cresce para tier superior
   - Land & Expand built-in

3. **Price discrimination (boa)**
   - Quem pode/quer pagar mais, paga
   - Quem não pode, acessa tier básico

4. **Simplicidade para cliente**
   - Escolhe "pacote" que faz sentido
   - Vs. configurar tudo à la carte

---

## Quantos Tiers Criar?

### Regra de Ouro: 3-4 Tiers

**Por quê:**

**Muito pouco (1-2 tiers):**
- Não captura diferentes segmentos
- Deixa dinheiro na mesa (enterprise pagaria mais)
- Ou perde SMB (preço único alto demais)

**Ideal (3-4 tiers):**
- Cobre segmentos principais
- Não sobrecarrega escolha
- Sweet spot

**Muito (5+ tiers):**
- Paralisia de escolha
- Confusão
- Difícil comunicar diferenças

---

### Estruturas Comuns

#### Estrutura A: 3 Tiers (Clássico)

```
[ Starter / Basic ]
[ Professional / Pro ]
[ Enterprise / Premium ]
```

**Quando usar:**
- Produto estabelecido
- Não quer freemium
- Segmentos claros: SMB, Mid-market, Enterprise

**Exemplos:**
- Salesforce (Essentials, Professional, Enterprise)
- Intercom (Starter, Pro, Premium)

---

#### Estrutura B: 4 Tiers (Com Free)

```
[ Free ]
[ Starter / Plus ]
[ Professional / Business ]
[ Enterprise ]
```

**Quando usar:**
- Estratégia freemium
- Product-led growth
- Network effects importantes

**Exemplos:**
- Slack (Free, Pro, Business+, Enterprise Grid)
- Notion (Personal Free, Plus, Business, Enterprise)
- Zoom (Basic, Pro, Business, Enterprise)

---

#### Estrutura C: 2 Tiers + Enterprise Custom

```
[ Starter ]
[ Pro ]
[ Enterprise - Fale com vendas ]
```

**Quando usar:**
- Early-stage
- Simplicidade é prioridade
- Enterprise é pequena % mas custom pricing

**Exemplos:**
- Muitos SaaS B2B pequenos

---

## Naming de Tiers

**Nome do tier comunica posicionamento.**

---

### Padrões de Naming

#### Padrão 1: Progressão Simples

**Basic → Pro → Enterprise**

**Vantagens:**
- Claro, direto
- Fácil entender hierarquia

**Exemplos:**
- GitHub (Free, Team, Enterprise)
- Dropbox (Basic, Plus, Professional, Business)

---

#### Padrão 2: Metálico (Valorização)

**Bronze → Silver → Gold → Platinum**

**Ou:**

**Standard → Plus → Premium**

**Vantagens:**
- Sinaliza valor crescente
- Familiar (cartões de crédito, programas de fidelidade)

**Desvantagens:**
- Pode parecer genérico

**Exemplos:**
- Alguns SaaS usam, mas menos comum

---

#### Padrão 3: Tamanho/Uso

**Individual → Team → Business → Enterprise**

**Vantagens:**
- Auto-segmentação clara
- Cliente sabe qual tier é para ele

**Exemplos:**
- Canva (Free, Pro, Teams, Enterprise)
- Figma (Starter, Professional, Organization, Enterprise)

---

#### Padrão 4: Funcional/Criativo

**Nomes únicos alinhados com brand.**

**Exemplos:**
- Mailchimp (Free, Essentials, Standard, Premium)
- Basecamp (Personal, Business)
- Airtable (Free, Plus, Pro, Enterprise)

**Cuidado:** Não ser criativo demais (confunde).

---

### Coisas a Evitar em Naming

**❌ Nomes negativos**
- "Lite" (soa fraco)
- "Economy" (soa barato/inferior)

**❌ Nomes muito similares**
- "Pro" vs. "Pro Plus" vs. "Pro Premium" (confuso)

**❌ Números**
- "Tier 1", "Tier 2" (sem significado)

---

## Framework Good-Better-Best

**Estrutura clássica de 3 tiers.**

---

### Good (Tier de Entrada)

**Objetivo:** Barreira de entrada baixa, atrair volume.

**Características:**
- **Preço:** R$50-R$200/mês (SMB acessível)
- **Features:** Core/essencial
- **Limites:** Apertados (forçar upgrade)
- **Target:** Freelancers, micro-empresas, startups early

**Features típicas:**
- Funcionalidades básicas
- Limite de usuários (1-5)
- Limite de uso (ex: 1k contacts, 100 projects)
- Suporte: Email apenas
- Sem features "enterprise" (SSO, permissões avançadas, etc.)

**Pricing exemplo:**
- R$99/mês
- Até 5 usuários
- 1.000 contatos
- Email support

---

### Better (Tier Mais Popular)

**Objetivo:** Tier que você QUER que maioria dos clientes escolha.**

**Características:**
- **Preço:** R$200-R$1.000/mês (sweet spot)
- **Features:** Core + Advanced
- **Limites:** Generosos (suficiente para maioria)
- **Target:** SMB estabelecidos, mid-market small

**Features típicas:**
- Tudo do "Good"
- + Features avançadas (automation, analytics, integrações)
- Limites maiores (25-50 usuários, 10k contacts)
- Suporte: Email + Chat
- API access
- Integrações premium

**Pricing exemplo:**
- R$499/mês (destaque com badge "MAIS POPULAR")
- Até 25 usuários
- 10.000 contatos
- Integrações ilimitadas
- API access
- Priority support

**Estratégia:**
- Fazer melhor relação custo/benefício
- Badge "Mais Popular" ou "Recomendado"
- 50-60% dos clientes devem escolher este

---

### Best (Tier Premium/Enterprise)

**Objetivo:** Capturar clientes enterprise com alto willingness to pay.**

**Características:**
- **Preço:** R$1.000+/mês ou custom
- **Features:** Tudo + Enterprise features
- **Limites:** Ilimitados ou muito altos
- **Target:** Mid-market large, enterprise

**Features típicas:**
- Tudo do "Better"
- + SSO (SAML, Okta)
- + Admin controls (RBAC, permissions, audit logs)
- + SLA uptime (99.9%+)
- + Dedicated CSM
- + Custom integrações
- + Priority support 24/7
- + Training/onboarding dedicado
- + Data residency, compliance (SOC2, GDPR)

**Pricing exemplo:**
- "Fale com vendas" ou R$2.499+/mês
- Usuários ilimitados
- Tudo ilimitado
- SSO, SLA 99.95%
- Dedicated CSM
- Custom contract

**Estratégia:**
- 10-20% dos clientes, mas 40-60% da receita
- Pricing custom (cada deal é diferente)

---

## Diferenciação Entre Tiers

**Decisão crítica: O que vai em qual tier?**

---

### Dimensões de Diferenciação

#### 1. Limites Quantitativos (Usage Caps)

**Mais simples e comum.**

**Exemplos:**

**Mailchimp:**
- Free: 500 contatos
- Essentials: 50k contatos
- Standard: 100k contatos
- Premium: 200k+ contatos

**Slack:**
- Free: 90 dias de mensagens
- Pro: Mensagens ilimitadas

**Figma:**
- Starter: 3 projetos
- Professional: Ilimitado

**Vantagens:**
- Fácil entender
- Natural upgrade (cliente cresce, atinge limite)

**Desvantagens:**
- Pode não capturar diferença de valor
- Cliente pode otimizar para ficar no limite (não upgrade)

---

#### 2. Features Diferenciadas

**Diferentes features em cada tier.**

**Exemplo: CRM**

**Good (Starter):**
- Contact management
- Deal tracking
- Email integration

**Better (Pro):**
- Tudo do Starter +
- Automation (workflows)
- Reporting/analytics
- Custom fields
- API access

**Best (Enterprise):**
- Tudo do Pro +
- SSO
- Role-based permissions
- Audit logs
- Forecasting
- Custom integrations
- Dedicated CSM

**Como decidir quais features em qual tier:**

**Good/Starter = Core, essential**
- Features que definem a categoria
- Sem elas, produto não funciona
- Ex: CRM precisa de contact management

**Better/Pro = Advanced, productivity**
- Features que aumentam eficiência
- Power users precisam
- Ex: Automation, reporting, API

**Best/Enterprise = Enterprise, admin, compliance**
- Features que empresa grande PRECISA
- SMB não precisa/não valoriza
- Ex: SSO, audit logs, SLA

---

#### 3. Suporte/SLA

**Nível de atendimento diferenciado.**

**Exemplo:**

**Good:**
- Email support (resposta 48h)
- Help center self-service

**Better:**
- Email + Chat (resposta 12h)
- Priority queue

**Best:**
- Email + Chat + Phone (resposta 2h)
- 24/7 support
- Dedicated CSM
- SLA uptime 99.95%

---

#### 4. Segmentação por Uso (Individual vs. Team vs. Business)

**Não é feature, é TARGET.**

**Exemplo: Notion**

**Personal (Free):**
- Uso individual
- Docs ilimitados
- Colaboração limitada

**Team:**
- Uso em equipe
- Collaboration features
- Admin controls básicos

**Business:**
- Uso em empresa
- Advanced admin
- Permissões granulares

**Enterprise:**
- Large organization
- SSO, SCIM
- Advanced security

---

### Features que SÃO Enterprise (Sempre no tier mais alto)

**Nunca coloque no tier baixo/médio:**

1. **SSO (Single Sign-On)** - SAML, Okta
2. **SCIM** (User provisioning)
3. **Audit logs** (compliance)
4. **Advanced permissions** (RBAC)
5. **SLA** com uptime guarantee
6. **Dedicated CSM**
7. **Custom contract/terms**
8. **Data residency** (escolher região de servidor)
9. **White-label**
10. **Advanced security** (SOC2, GDPR compliance証書)

**Por quê?**
- Enterprise valoriza MUITO essas features
- Dispostos a pagar 5-10x mais
- SMB não precisa/não valoriza

---

## Packaging: Como Organizar Features em Tiers

### Estratégia 1: Additive (Cumulativo)

**Cada tier INCLUI tudo do anterior + adiciona mais.**

**Exemplo:**

```
Starter: A, B, C
Pro: A, B, C, D, E, F
Enterprise: A, B, C, D, E, F, G, H, I
```

**Vantagens:**
- Fácil entender ("upgrade = tudo que tinha + mais")
- Upsell natural

**Desvantagens:**
- Tier alto pode ter features demais (overwhelming)

**Uso:** Maioria dos SaaS usa este modelo.

---

### Estratégia 2: Segmented (Segmentado)

**Tiers têm features DIFERENTES (não cumulativos).**

**Exemplo:**

```
Marketing Tier: Features de marketing
Sales Tier: Features de vendas
Service Tier: Features de customer service
```

**Vantagens:**
- Segmentação clara por use case
- Cliente escolhe o que precisa

**Desvantagens:**
- Pode precisar de múltiplos tiers (compra Marketing + Sales)
- Complexidade

**Uso:** HubSpot (Marketing Hub, Sales Hub, Service Hub separados).

---

### Estratégia 3: Hybrid (Híbrido)

**Combina additive + segmented.**

**Exemplo: HubSpot**

**Eixo 1 (Produto):**
- Marketing Hub
- Sales Hub
- Service Hub

**Eixo 2 (Tier por produto):**
- Starter
- Professional
- Enterprise

**Matriz 3x3:**

```
           Starter    Professional    Enterprise
Marketing    R$200       R$2k           R$10k
Sales        R$200       R$2k           R$10k
Service      R$200       R$2k           R$10k
```

**Vantagens:**
- Captura segmentação + tiers
- Cross-sell oportunidades (compra Marketing + Sales)

**Desvantagens:**
- Complexidade máxima
- Só funciona se você tem produtos separados

---

## Pricing Gaps Entre Tiers

**Quanto deve ser a diferença de preço entre tiers?**

---

### Regra: 2-5x Entre Tiers Adjacentes

**Exemplo 1 (2-3x):**
```
Starter: R$99
Pro: R$299 (3x)
Enterprise: R$999 (3.3x)
```

**Exemplo 2 (3-5x):**
```
Starter: R$99
Pro: R$499 (5x)
Enterprise: R$2.499 (5x)
```

---

### Por Que Não 1.5x ou 10x?

**Gap muito pequeno (1.5x):**
```
Starter: R$100
Pro: R$150 (só 1.5x)
```

**Problema:**
- Pro não parece muito melhor
- Upgrade "óbvio demais" (todo mundo faz, perde revenue de quem pagaria mais)

---

**Gap muito grande (10x):**
```
Starter: R$100
Pro: R$1.000 (10x!)
```

**Problema:**
- Gap enorme dificulta upgrade
- Cliente em Starter nunca vai para Pro (pulo muito grande)
- Precisa de tier intermediário

---

### Sweet Spot: 3x

**Exemplo:**
```
Starter: R$100
Pro: R$300 (3x)
Enterprise: R$900 (3x)
```

**Por quê funciona:**
- Diferença suficiente para justificar features adicionais
- Não é pulo impossível
- Padrão da indústria

---

## Tier "Decoy" (Isca)

**Criar tier intermediário com má relação custo/benefício para empurrar para tier superior.**

**Já vimos em Pricing Psychology, mas vale reforçar.**

---

### Exemplo de Decoy Bem Feito

```
[ Starter: R$99/mês ]
  - 5 usuários
  - Features básicas

[ Pro: R$299/mês ]              ← DECOY
  - 10 usuários
  - Features avançadas

[ Business: R$399/mês ]         ← TARGET
  - 50 usuários
  - Tudo do Pro + Admin + SSO
```

**Análise:**
- Starter → Pro: +R$200 para +5 usuários
- Pro → Business: +R$100 para +40 usuários + features enterprise

**Business é obviamente melhor valor.**

**Resultado:** Maioria escolhe Business (não Pro).

---

### Cuidado com Decoy

**Se NINGUÉM escolhe o tier decoy:**
- Considere remover (fica estranho ter tier que ninguém usa)
- Ou ajuste pricing/features

**Regra:** Decoy deve ter 5-15% de escolha.
- 0% = Decoy óbvio demais (ruim)
- 30%+ = Não está funcionando como decoy

---

## Freemium como Tier 0

**Se usar freemium, ele é tier separado (Tier 0).**

---

### Como Estruturar Free Tier

#### Decisão 1: Limites de Uso vs. Features

**Opção A: Limites de Uso**
```
Free: Até 100 contatos
Paid: 1.000+ contatos
```

**Opção B: Features Limitadas**
```
Free: Core features
Paid: Core + Advanced features
```

**Opção C: Hybrid**
```
Free: Core features + até 100 contatos
Paid: Advanced features + ilimitado
```

**Mais comum:** Hybrid.

---

#### Decisão 2: Quão Generoso?

**Free tier generoso (Notion, Figma, Slack):**
- 80-90% do valor
- Conversion baixa (2-4%)
- Mas viralidade massiva

**Free tier restritivo (Calendly, Airtable):**
- 40-50% do valor
- Conversion alta (5-10%)
- Crescimento mais lento

**Escolha depende de:**
- COGS (custo baixo = pode ser generoso)
- Network effects (precisa de volume = generoso)
- Go-to-market (PLG = generoso, sales-led = restritivo)

---

## Tier Enterprise: "Fale com Vendas" vs. Preço Público

### Opção A: Custom Pricing (Fale com Vendas)

**Vantagens:**
- Maximiza revenue (negocia caso a caso)
- Flexibilidade (cada cliente é diferente)
- Qualifica leads (só sérios vão falar com vendas)

**Desvantagens:**
- Fricção (cliente quer ver preço)
- Precisa de sales team
- Não escala para SMB

**Quando usar:**
- Deals >R$50k/ano
- Produto complexo, customizado
- Enterprise com needs únicos

---

### Opção B: Preço Público (Transparente)

**Exemplo:**
```
Enterprise: R$2.499/mês
```

**Vantagens:**
- Transparência (cliente sabe o que esperar)
- Self-service possível
- Reduz fricção

**Desvantagens:**
- Deixa dinheiro na mesa (alguns pagariam R$5k)
- Menos flexibilidade

**Quando usar:**
- Produto simples, self-service
- Preço relativamente baixo (<R$2k/mês)
- Quer escalar sem sales

---

### Opção C: Hybrid (Range Público + Custom)

**Exemplo:**
```
Enterprise: A partir de R$2.499/mês
Fale com vendas para quote customizado
```

**Vantagens:**
- Transparência parcial (cliente tem noção)
- Flexibilidade para negociar

**Uso:** Muito comum em SaaS B2B.

---

## Optimização de Tiers: Dados a Analisar

### Métrica 1: Distribution (% escolha de cada tier)

**Ideal:**
- Starter: 30-40%
- Pro (target): 50-60%
- Enterprise: 10-20%

**Se Starter é 70%:**
- Pro está muito caro OU
- Starter tem features demais

**Se Enterprise é 40%:**
- Pro tem features de menos OU
- Pricing está bom (capturando empresas grandes)

---

### Métrica 2: Upgrade Rate

**% de clientes que fazem upgrade por ano.**

**Benchmark:**
- Bom: 20-30% upgrades/ano
- Médio: 10-20%
- Ruim: <10%

**Se muito baixo (<10%):**
- Tiers estão mal definidos
- Ou falta incentivo/comunicação de upgrade

---

### Métrica 3: Downgrade Rate

**% que fazem downgrade.**

**Benchmark:**
- Aceitável: 5-10%/ano
- Ruim: >15%

**Se alto:**
- Tier superior tem features que não usam
- Ou preço muito alto para valor recebido

---

### Métrica 4: Revenue por Tier

**% de MRR total por tier.**

**Exemplo:**
- Starter (40% dos clientes): 15% do MRR
- Pro (50% dos clientes): 45% do MRR
- Enterprise (10% dos clientes): 40% do MRR

**Normal:** Enterprise tem menos clientes mas gera mais revenue.

**Se Starter gera 50% do revenue:**
- Oportunidade de aumentar preço de Pro/Enterprise

---

## Design da Pricing Page

**Como apresentar tiers visualmente.**

---

### Layout: Horizontal vs. Vertical

#### Layout Horizontal (Mais Comum)

```
┌──────────┐  ┌──────────┐  ┌──────────┐
│ STARTER  │  │   PRO    │  │ENTERPRISE│
│  R$99    │  │  R$499   │  │  Custom  │
│          │  │          │  │          │
│ Features │  │ Features │  │ Features │
└──────────┘  └──────────┘  └──────────┘
```

**Quando usar:** Desktop, 3-4 tiers.

---

#### Layout Vertical (Mobile-Friendly)

```
┌─────────────────────┐
│ STARTER - R$99      │
│ Features...         │
└─────────────────────┘

┌─────────────────────┐
│ PRO - R$499         │
│ Features...         │
└─────────────────────┘

┌─────────────────────┐
│ ENTERPRISE - Custom │
│ Features...         │
└─────────────────────┘
```

**Quando usar:** Mobile, 4+ tiers.

---

### Destacar Tier Recomendado

**Badge "Mais Popular" ou "Recomendado".**

**Exemplo:**
```
┌──────────┐  ┌─────────────────┐  ┌──────────┐
│ STARTER  │  │ ✨ PRO - POPULAR ✨│  │ENTERPRISE│
│  R$99    │  │    R$499        │  │  Custom  │
└──────────┘  └─────────────────┘  └──────────┘
```

**Efeito:** +20-30% de escolha para esse tier.

---

### Feature Comparison Table

**Mostrar quais features em qual tier.**

**Exemplo:**

| Feature | Starter | Pro | Enterprise |
|---------|---------|-----|------------|
| **Usuários** | 5 | 25 | Ilimitado |
| **Contatos** | 1k | 10k | Ilimitado |
| **Automation** | ❌ | ✅ | ✅ |
| **API Access** | ❌ | ✅ | ✅ |
| **SSO** | ❌ | ❌ | ✅ |
| **Dedicated CSM** | ❌ | ❌ | ✅ |
| **Suporte** | Email | Email+Chat | 24/7 Phone |
| **Preço** | R$99/mês | R$499/mês | Custom |

**Vantagens:** Fácil comparar.

**Desvantagens:** Pode ficar longo (muitas features).

---

## Evolução de Tiers ao Longo do Tempo

**Tiers não são fixos. Evoluem com produto.**

---

### Quando Adicionar Novo Tier

**Cenário 1: Gap entre Starter e Pro muito grande**

**Antes:**
```
Starter: R$99 (5 users)
Pro: R$999 (50 users)  ← Gap de 10x!
```

**Problema:** Ninguém faz upgrade (pulo muito grande).

**Solução:** Adicionar tier intermediário.

**Depois:**
```
Starter: R$99 (5 users)
Plus: R$299 (15 users)    ← NOVO
Pro: R$999 (50 users)
```

---

**Cenário 2: Enterprise se tornou grande segmento**

**Antes:**
```
Starter: R$99
Pro: R$499
Enterprise: Custom (R$2k-R$10k)
```

**Problema:** Enterprise tem needs muito variados.

**Solução:** Split enterprise em 2 tiers.

**Depois:**
```
Starter: R$99
Pro: R$499
Business: R$2.499 (mid-market)
Enterprise: Custom (large enterprise)
```

---

### Quando Remover Tier

**Cenário: Ninguém escolhe tier intermediário**

**Antes:**
```
Starter: R$99 (40% escolhem)
Plus: R$299 (2% escolhem)    ← Ninguém quer!
Pro: R$999 (58% escolhem)
```

**Problema:** Plus é redundante, confunde.

**Solução:** Remover Plus.

**Depois:**
```
Starter: R$99
Pro: R$999
```

---

## Case Studies de Tier Structure

### Case 1: Slack - 4 Tiers

**Estrutura:**
```
Free: Grátis
  - 90 dias mensagens
  - 10 integrações

Pro: ~R$30/usuário ativo/mês
  - Mensagens ilimitadas
  - Integrações ilimitadas
  - Apps avançadas

Business+: ~R$60/usuário ativo/mês
  - Tudo do Pro
  - SSO (SAML)
  - Compliance (SOC2, etc.)
  - User provisioning (SCIM)

Enterprise Grid: Custom
  - Tudo do Business+
  - Unlimited workspaces
  - Advanced admin controls
  - Dedicated CSM
  - Custom contract/SLA
```

**Estratégia:**
- Free: Viralidade, land
- Pro: Monetização principal (50%+ da receita)
- Business+: Mid-market
- Grid: Large enterprise (Fortune 500)

**Resultado:** NRR ~140%, expansion massiva.

---

### Case 2: HubSpot - Matrix 3x3

**Produtos (Hubs):**
- Marketing Hub
- Sales Hub
- Service Hub

**Tiers (por produto):**
- Starter: R$200-R$500/mês
- Professional: R$2k-R$5k/mês
- Enterprise: R$10k+/mês

**Estratégia:**
- Land: 1 hub, tier Starter
- Expand: Upgrade tier OU adicionar hubs
- Cross-sell rate: 60%+ de clientes compram 2+ hubs

**Resultado:**
- ACV cresce de R$2.4k (1 hub Starter) para R$50k+ (3 hubs Enterprise)
- Land & Expand perfeito

---

### Case 3: Notion - Segmentação por Uso

**Estrutura:**
```
Personal: Grátis
  - Uso individual
  - Unlimited pages
  - Compartilhamento limitado

Plus: R$40/usuário/mês
  - Small teams (até 10)
  - Collaboration
  - Version history

Business: R$75/usuário/mês
  - Companies
  - Advanced permissions
  - Admin tools
  - SAML SSO

Enterprise: Custom
  - Large orgs (100+)
  - Advanced security
  - Dedicated support
  - Custom contract
```

**Diferenciação:** Não é só features, é USO (individual vs. team vs. business).

**Estratégia:**
- Personal: Viralidade massiva (free tier generoso)
- Plus: First conversion (bottom-up em empresas)
- Business: Expand quando empresa adota formalmente
- Enterprise: Grandes corporações

---

## Checklist de Tier Structure

**Ao criar/otimizar tiers, verificar:**

### Estrutura
- [ ] **Número de tiers:** 3-4 tiers (não muito, não pouco)?
- [ ] **Naming:** Claro, hierárquico, fácil entender?
- [ ] **Free tier:** Incluir ou não? Quão generoso?

### Diferenciação
- [ ] **Features:** Cada tier tem features claramente diferentes?
- [ ] **Enterprise features:** SSO, audit logs, etc. apenas no tier top?
- [ ] **Limites:** Quantitativos claros (usuários, storage, etc.)?

### Pricing
- [ ] **Gap entre tiers:** 2-5x entre tiers adjacentes?
- [ ] **Tier target:** Identificou qual tier quer que maioria escolha?
- [ ] **Decoy:** Há tier intermediário que faz tier superior parecer melhor?

### Apresentação
- [ ] **Tier recomendado:** Badge "Mais Popular" no tier target?
- [ ] **Comparison table:** Fácil comparar features entre tiers?
- [ ] **Mobile-friendly:** Funciona bem em mobile?

### Validação
- [ ] **Distribution:** % de escolha de cada tier faz sentido?
- [ ] **Upgrade path:** Clientes conseguem fazer upgrade naturalmente?
- [ ] **Revenue:** Tier enterprise gera revenue desproporcional (bom sinal)?

---

## Erros Comuns em Tier Structure

### Erro 1: Muitos Tiers (5+)

**Problema:** Paralisia de escolha.

**Exemplo:**
```
Free, Lite, Basic, Standard, Plus, Pro, Premium, Enterprise
```

**8 tiers = Confusão.**

**Solução:** Consolidar em 3-4.

---

### Erro 2: Diferenças Pouco Claras

**Exemplo:**
```
Pro: R$499 - "Features avançadas"
Business: R$699 - "Features de negócios"
```

**Problema:** Cliente não entende diferença.

**Solução:** Especificar exatamente quais features.

---

### Erro 3: Tier Básico Muito Limitado

**Exemplo:**
```
Starter: R$99/mês
- 1 usuário
- 10 contatos
```

**Problema:** Tão limitado que não serve para ninguém.

**Solução:** Tier básico deve ser FUNCIONAL (mesmo que limitado).

---

### Erro 4: Enterprise Features no Tier Médio

**Exemplo:**
```
Pro: R$499/mês
- SSO
- Audit logs
```

**Problema:** SSO/audit logs valem R$5k+/mês para enterprise. Você deixa dinheiro na mesa.

**Solução:** Enterprise features APENAS em tier enterprise.

---

### Erro 5: Nenhum Tier é "Popular"

**Problema:** Não há tier recomendado, cliente não sabe qual escolher.

**Solução:** Destacar tier target com badge/destaque visual.

---

## Conclusão: Framework de Tier Structure

**Processo recomendado:**

**1. Definir número de tiers (3-4)**

**2. Nomear tiers (Basic/Pro/Enterprise ou similar)**

**3. Definir target de cada tier:**
   - Starter: Freelancers, micro-empresas
   - Pro: SMB, startups
   - Enterprise: Mid-market, large corps

**4. Alocar features:**
   - Starter: Core
   - Pro: Core + Advanced
   - Enterprise: Tudo + Enterprise features

**5. Definir limites quantitativos:**
   - Usuários, storage, etc.

**6. Precificar (gaps de 2-5x):**
   - Starter: R$99
   - Pro: R$499 (5x)
   - Enterprise: R$2.499 (5x)

**7. Destacar tier target (badge "Popular")**

**8. Testar e iterar baseado em dados:**
   - % de escolha
   - Upgrade/downgrade rates
   - Revenue por tier

---

**Próximo arquivo:** `price-testing-methodology.md` (como testar preços: A/B testing, multivariate, cohort analysis, experimentos seguros)