# North Star Framework

**Programa Reforge**: Growth Series, Advanced Growth Strategy

## O que é North Star Metric

A North Star Metric (NSM) é a **métrica única** que melhor captura o **valor core** que seu produto entrega aos clientes. É a métrica que, quando cresce de forma sustentável, indica que a empresa está saudável e crescendo da maneira certa.

### Princípios Fundamentais

1. **Captura valor ao cliente** (não apenas valor à empresa)
2. **É leading indicator** de sucesso de longo prazo (revenue, retention)
3. **Une o time** em torno de objetivo comum
4. **Guia decisões** de produto, marketing, e growth

### O que North Star NÃO é

❌ **Não é apenas uma métrica de vaidade**: Não é "usuários totais" se usuários inativos não geram valor
❌ **Não é apenas métrica de receita**: MRR é lagging, não mostra saúde do produto
❌ **Não é múltiplas métricas**: É **uma** métrica (mas tem input metrics que a alimentam)
❌ **Não é fixa para sempre**: Pode evoluir conforme empresa muda de estágio

## Como Identificar sua North Star

### Framework de Seleção

Usar 3 critérios para avaliar candidatas a North Star:

#### 1. **Expressa valor entregue** (Value)
- A métrica reflete o valor que o cliente recebe?
- Quando esta métrica sobe, o cliente está melhor?
- Ela conecta com o "why" do seu produto?

#### 2. **Captura amplitude de uso** (Breadth)
- Reflete quantos clientes estão recebendo valor?
- Inclui tanto depth (intensidade) quanto breadth (abrangência)?

#### 3. **É leading indicator** (Leading)
- Prediz sucesso futuro (receita, retenção, word-of-mouth)?
- Pode ser influenciada por ações do time?
- Pode ser medida com frequência (semanal/mensal)?

### Processo de Definição (5 Passos)

**Passo 1: Defina a proposta de valor core**
- Por que clientes usam seu produto?
- Qual problema você resolve?
- Quando o cliente tem "aha moment"?

Exemplo (Airbnb): "Permitir que qualquer pessoa viaje e se hospede como um local"

**Passo 2: Liste momentos de valor**
- Quais ações no produto geram valor ao cliente?
- Quando o cliente percebe que o produto funciona?

Exemplo (Airbnb):
- Descobrir acomodação única no destino
- Fazer reserva de forma confiável
- Ter experiência positiva na estadia
- Retornar e reservar novamente

**Passo 3: Identifique candidatas a North Star**
- Transforme momentos de valor em métricas mensuráveis
- Liste 3-5 candidatas

Exemplo (Airbnb):
- Noites reservadas
- Buscas realizadas
- Perfis de hospedagem criados
- Gross Booking Value (GBV)
- Usuários ativos mensais

**Passo 4: Avalie contra os 3 critérios**

Criar tabela de avaliação (1-10 pontos cada critério):

| Métrica Candidata         | Valor | Breadth | Leading | Total |
|---------------------------|-------|---------|---------|-------|
| Noites reservadas         | 10    | 9       | 9       | 28    | ⭐
| Buscas realizadas         | 3     | 8       | 5       | 16    |
| Perfis criados            | 2     | 5       | 6       | 13    |
| GBV                       | 7     | 8       | 7       | 22    |
| MAU                       | 4     | 9       | 6       | 19    |

**Passo 5: Valide com stakeholders e dados**
- A métrica ressoa com time de produto, eng, marketing, sales?
- Há correlação histórica entre esta métrica e receita/retenção?
- É possível instrumentar e rastrear?

**Decisão (Airbnb)**: **Nights Booked** 🎯
- Captura valor (hospedagem realizada)
- Breadth (total de experiências criadas)
- Leading (prediz receita, NPS, retention)

## Input Metrics

Uma North Star sozinha não é acionável. **Input Metrics** são as métricas que **impulsionam** a North Star.

### Framework de Input Metrics

Para cada Input Metric, deve responder:
1. **Influencia diretamente a NSM?** (causalidade, não apenas correlação)
2. **O time pode movê-la?** (tem controle sobre ela)
3. **É mensurável?** (pode rastrear com precisão)

### Estrutura de Input Metrics

```
       North Star Metric
              ↑
     _________|_________
    |         |         |
 Input 1   Input 2   Input 3
    ↑         ↑         ↑
Sub-inputs Sub-inputs Sub-inputs
```

### Exemplo: Airbnb

**North Star**: Nights Booked

**Input Metrics** (nível 1):
1. **Active Bookers** (breadth: quantos usuários únicos fazem reservas)
2. **Booking Frequency** (depth: quantas vezes cada booker reserva)
3. **Nights per Booking** (depth: duração média de estadia)

**Sub-Input Metrics** (nível 2):

Para **Active Bookers**:
- New Bookers (aquisição)
- Retained Bookers (retenção)
- Resurrected Bookers (reativação)

Para **Booking Frequency**:
- Discovery (listagens vistas)
- Consideration (listagens salvas, contato com host)
- Conversion (taxa de busca → reserva)

Para **Nights per Booking**:
- Supply de estadas longas
- Incentivos (desconto semanal/mensal)
- Traveler type (negócios vs. lazer)

### Hierarquia de Inputs

**Nível 1**: Input Metrics diretas (3-5 métricas)
- Diretamente multiplicam/somam para formar NSM
- Ex: Bookers × Frequency = Bookings

**Nível 2**: Sub-inputs (5-10 métricas)
- Alimentam as Input Metrics
- Aqui é onde times específicos atuam

**Nível 3**: Tactical metrics
- Métricas de features, experimentos, campanhas específicas
- Mais granulares, time/squad-level

## Exemplos de North Star por Tipo de Produto

### B2C Social/Community

**Facebook**
- **NSM**: Daily Active Users (DAU)
- **Input Metrics**: New Users, Retained Users, Resurrected Users
- **Rationale**: DAU captura engagement diário, prediz receita de ads

**Reddit**
- **NSM**: Weekly Active Posters
- **Input Metrics**: New Posters, Communities Joined, Posts per Poster
- **Rationale**: Posters criam conteúdo que atrai mais usuários (flywheel)

### B2C Marketplace

**Uber**
- **NSM**: Rides per Week
- **Input Metrics**: Active Riders, Ride Frequency, Ride Completion Rate
- **Rationale**: Rides captura valor (transporte realizado), impulsiona receita

**DoorDash**
- **NSM**: Orders per Month
- **Input Metrics**: Monthly Orderers, Order Frequency, Cart Size
- **Rationale**: Orders = valor ao cliente + merchant + dasher

### B2C SaaS/Subscription

**Spotify**
- **NSM**: Time Spent Listening
- **Input Metrics**: Monthly Active Listeners, Sessions per Listener, Minutes per Session
- **Rationale**: Listening time prediz churn e willingness to pay

**Netflix**
- **NSM**: Hours Watched per Month
- **Input Metrics**: Monthly Viewers, Viewing Days per Month, Hours per Day
- **Rationale**: Watch time indica content-market fit, prediz retention

### B2B SaaS

**Slack**
- **NSM**: Messages Sent per Week
- **Input Metrics**: Weekly Active Teams, Members per Team, Messages per Member
- **Rationale**: Mensagens = comunicação acontecendo, switching cost alto

**Notion**
- **NSM**: Collaborative Docs Created
- **Input Metrics**: Active Workspaces, Members per Workspace, Docs per Member
- **Rationale**: Docs colaborativos = network effects, stickiness

**HubSpot**
- **NSM**: Weekly Active Contacts
- **Input Metrics**: Active Users, Contacts Added, Contact Interactions
- **Rationale**: Contacts gerenciados = CRM sendo usado para propósito core

**Asana**
- **NSM**: Tasks Completed per Week
- **Input Metrics**: Active Teams, Tasks Created, Completion Rate
- **Rationale**: Tasks completadas = trabalho sendo gerenciado e concluído

### B2B Horizontal SaaS

**Calendly**
- **NSM**: Meetings Scheduled
- **Input Metrics**: Active Schedulers, Invitees per Scheduler, Meetings per Invitee
- **Rationale**: Meetings agendados = propósito core do produto

**Loom**
- **NSM**: Videos Watched
- **Input Metrics**: Videos Created, Shares per Video, Views per Video
- **Rationale**: Videos assistidos = comunicação assíncrona acontecendo

### Developer Tools

**GitHub**
- **NSM**: Weekly Active Contributors
- **Input Metrics**: Active Repositories, Contributors per Repo, Commits per Contributor
- **Rationale**: Contributors ativos = desenvolvimento ativo, lock-in alto

**Figma**
- **NSM**: Collaborative Design Files Created
- **Input Metrics**: Active Teams, Designers per Team, Files per Designer
- **Rationale**: Arquivos colaborativos = design em tempo real (core value)

### E-commerce

**Amazon**
- **NSM**: Purchases per Month
- **Input Metrics**: Monthly Shoppers, Shopper Frequency, Items per Purchase
- **Rationale**: Compras = valor entregue, prediz GMV e receita

## Como Usar North Star no Dia a Dia

### 1. Priorização de Roadmap

**Pergunta guia**: "Esta feature vai mover a North Star?"

Criar rubric de priorização:
- **Impacto na NSM**: Alto (3pts), Médio (2pts), Baixo (1pt)
- **Confiança**: Alta (3pts), Média (2pts), Baixa (1pt)
- **Esforço**: Baixo (3pts), Médio (2pts), Alto (1pt)

Priorizar iniciativas com maior score.

**Exemplo**:
- Feature A: Auto-save documents
  - Impacto NSM (docs criados): Alto (evita perda, aumenta confiança) = 3
  - Confiança: Alta (dados mostram 20% abandonam por perda) = 3
  - Esforço: Médio (2 semanas eng) = 2
  - **Score: 8**

- Feature B: Dark mode
  - Impacto NSM: Baixo (preferência estética) = 1
  - Confiança: Baixa (sem dados de impacto) = 1
  - Esforço: Baixo (1 semana) = 3
  - **Score: 5**

Priorizar Feature A.

### 2. Alinhamento de Time

**Objetivo**: Todos os times entendem como contribuem para NSM

Criar **map de contribuição**:

```
        North Star: Nights Booked
                  ↓
    ______________|______________
   |              |              |
Product Team   Growth Team   Ops Team
   |              |              |
Melhorar       Adquirir       Qualidade
Search &       novos          de Hosts
Booking UX     travelers      & Suporte
   ↓              ↓              ↓
Input:         Input:         Input:
Conversion     New Bookers    Booking
Rate                          Completion
```

Cada time tem **Input Metric** sob sua responsabilidade.

### 3. Revisões e Retrospectivas

**Formato de Sprint Review/QBR**:

1. **NSM Performance**: Meta vs. Atual vs. Anterior
2. **Input Metrics Breakdown**: O que moveu? O que travou?
3. **Iniciativas Entregues**: Qual foi o impacto esperado vs. real?
4. **Learnings**: O que aprendemos sobre o que move a NSM?
5. **Next Actions**: O que vamos testar no próximo ciclo?

### 4. Experimentos

**Framework de hipóteses**:

"Acreditamos que **[intervenção]** vai aumentar **[input metric]** porque **[rationale]**, o que levará a **[X% aumento na NSM]**."

Exemplo:
"Acreditamos que **adicionar social proof (X avaliações)** na listing page vai aumentar **booking conversion rate** porque **reduz ansiedade de confiança**, o que levará a **+5% em Nights Booked**."

**Métricas do experimento**:
- **Primary**: Input Metric (booking conversion)
- **Secondary**: NSM (nights booked)
- **Guardrail**: Métricas que não podem piorar (ex: cancellation rate)

## Evolução da North Star

### Quando Mudar a North Star

North Star **não é imutável**. Considere mudança quando:

1. **Mudança de estágio**:
   - Pre-PMF → Post-PMF: De usage genérico para core value
   - Early → Growth: De ativação para retenção/monetização
   - Growth → Scale: De growth puro para eficiência

2. **Pivô de produto**:
   - Produto muda significativamente
   - ICP muda (ex: B2C → B2B)
   - Modelo de negócio muda (ex: ads → subscription)

3. **Métrica atual é gamed ou mal-aligned**:
   - Time está otimizando para métrica mas não para valor real
   - Ex: "Contas criadas" mas sem ativação

### Exemplos de Evolução

**Instagram**
- **Pre-2013**: DAU (crescimento puro)
- **2013-2016**: Stories Created (engagement depth)
- **2016-2020**: Time Spent in App (ads revenue optimization)
- **2020+**: ? (Reels engagement? Shopping actions?)

**LinkedIn**
- **Early**: Profiles Created (network size)
- **Growth**: Connections Made (network density)
- **Mature**: Weekly Active Users (engagement sustentável)

**Notion**
- **Pre-2019**: Users Signed Up (aquisição)
- **2019-2021**: Collaborative Docs Created (PMF, viral loops)
- **2022+**: Weekly Active Workspaces (retenção, B2B expansion)

## Erros Comuns

### ❌ Erro 1: North Star é métrica de vaidade

**Problema**: "Total Users" sem distinção de ativos vs. inativos

**Exemplo ruim**: Zoom tem 300M "users" mas 80% nunca abriram o app

**Fix**: Adicionar qualificador de atividade
- ❌ Total Users
- ✅ Weekly Active Users
- ✅✅ Weekly Active Meeting Hosts (melhor: captura core value)

### ❌ Erro 2: North Star é métrica lagging (receita)

**Problema**: MRR é outcome, não input. Não é acionável.

**Exemplo ruim**: "Nossa NSM é MRR Growth"

**Fix**: Identificar o que impulsiona MRR
- ❌ MRR Growth
- ✅ Active Subscriptions × ARPU
- ✅✅ Weekly Active Power Users (prediz upsell e retention)

### ❌ Erro 3: Múltiplas North Stars

**Problema**: "Nossa NSM é DAU, NPS, e Revenue"

**Fix**: Escolher UMA que melhor captura valor. Outras são inputs ou outcomes.

**Correto**:
- **North Star**: DAU (leading indicator de tudo)
- **Inputs**: New Users, Retained Users, Resurrected Users
- **Outcomes**: Revenue, NPS (consequências de DAU saudável)

### ❌ Erro 4: North Star sem Input Metrics

**Problema**: NSM sozinha não dá direção de onde atuar

**Exemplo ruim**: "Vamos aumentar Nights Booked" (como?)

**Fix**: Decompor em inputs acionáveis
- Aumentar Active Bookers (aquisição)
- Aumentar Booking Frequency (engagement, reativação)
- Aumentar Nights per Booking (incentivos, supply)

### ❌ Erro 5: North Star nunca evolui

**Problema**: Manter mesma NSM quando contexto muda

**Exemplo ruim**: Startup Series B ainda focando em "Sign Ups" (métrica de early stage)

**Fix**: Revisar NSM a cada mudança significativa de estágio ou estratégia

## Templates e Ferramentas

### North Star Canvas

Use o canvas em `assets/north-star-canvas.md` para definir sua NSM:

**Seções do canvas**:
1. Proposta de valor core
2. Momentos de valor
3. Candidatas a North Star (com scores)
4. North Star selecionada
5. Input Metrics (nível 1 e 2)
6. Como cada time contribui

### Dashboard de North Star

**Estrutura recomendada** (Looker, Tableau, Amplitude, Mixpanel):

**Seção 1: North Star Performance**
- Gráfico de linha: NSM ao longo do tempo (12 meses)
- Meta vs. Atual
- % change MoM, QoQ

**Seção 2: Input Metrics Breakdown**
- Gráfico de barras/área empilhada: Contribuição de cada input
- Tabela: Cada input metric com trend

**Seção 3: Cohort Analysis**
- NSM por cohort (mês de entrada)
- Permite ver se novos usuários estão melhores/piores

**Seção 4: Segmentação**
- NSM por segmento (ICP, região, canal, etc.)
- Identifica onde focar

**Seção 5: Impacto de Iniciativas**
- Lista de features/experimentos lançados
- Before/After da NSM e input metrics

## Recursos Complementares

### Leitura Recomendada

**Artigos Fundacionais**:
- Amplitude: "The North Star Metric" (2016)
- Lenny Rachitsky: "How to Find Your North Star Metric" (2021)
- Sean Ellis: "The One Metric That Matters" (2010)

**Case Studies**:
- Airbnb: From GMV to Nights Booked
- HubSpot: Weekly Active Contacts
- Slack: Messages Sent
- Spotify: Time Listening

### Comunidades

- Reforge (Growth Series alumni)
- Lenny's Newsletter (community)
- #growth channels em Slack communities

## Checklist de Implementação

Use este checklist ao implementar North Star:

**Fase 1: Definição (Semana 1-2)**
- [ ] Articular proposta de valor core
- [ ] Listar 5-10 momentos de valor
- [ ] Identificar 3-5 candidatas a NSM
- [ ] Avaliar com framework (Value, Breadth, Leading)
- [ ] Validar com stakeholders (Product, Eng, Growth, Leadership)
- [ ] Escolher NSM final

**Fase 2: Input Metrics (Semana 2-3)**
- [ ] Identificar 3-5 Input Metrics (nível 1)
- [ ] Decompor em Sub-inputs (nível 2)
- [ ] Mapear responsabilidade por time
- [ ] Validar que inputs movem NSM (correlação histórica)

**Fase 3: Instrumentação (Semana 3-4)**
- [ ] Garantir que NSM pode ser rastreada (eng/analytics)
- [ ] Instrumentar Input Metrics
- [ ] Criar dashboard automatizado
- [ ] Definir frequência de revisão (semanal, mensal)

**Fase 4: Socialização (Semana 4-6)**
- [ ] Apresentar NSM para toda empresa (all-hands)
- [ ] Treinar times em como NSM funciona
- [ ] Criar map de contribuição (como cada time afeta NSM)
- [ ] Incorporar NSM em rituais (sprint planning, QBR)

**Fase 5: Aplicação (Ongoing)**
- [ ] Usar NSM para priorizar roadmap
- [ ] Estruturar experimentos em função de inputs
- [ ] Revisar NSM em retros e reviews
- [ ] Iterar e refinar conforme aprende

---

**North Star Framework é sobre foco e alinhamento. Uma métrica, um time, um propósito.** 🌟
