# Idea Validation Frameworks

Este documento contém frameworks validados para avaliar e validar ideias de produtos antes de começar o desenvolvimento. Use estas metodologias durante o Step 2 do workflow principal.

## Table of Contents

1. [Lean Startup Principles](#lean-startup-principles)
2. [Jobs-to-be-Done (JTBD) Framework](#jobs-to-be-done-jtbd-framework)
3. [Mom Test Framework](#mom-test-framework)
4. [Problem-Solution Fit](#problem-solution-fit)
5. [MVP Definition Strategies](#mvp-definition-strategies)
6. [Validation Metrics](#validation-metrics)

---

## Lean Startup Principles

### Build-Measure-Learn Loop

O ciclo fundamental do Lean Startup:

```
IDEA → BUILD (MVP) → MEASURE (Data) → LEARN (Insights) → IDEA (Pivot/Persevere)
    ↑                                                              ↓
    └──────────────────────────────────────────────────────────────┘
```

**Aplicação prática:**

1. **Build:** Construir a versão mais simples que testa sua hipótese (não o produto completo)
2. **Measure:** Coletar dados de uso real (não opiniões hipotéticas)
3. **Learn:** Interpretar dados para validar ou invalidar hipóteses
4. **Decide:** Pivotar (mudar direção) ou perseverar (continuar caminho)

**Pivots comuns:**
- **Zoom-in pivot:** Um feature vira o produto todo
- **Zoom-out pivot:** O produto vira apenas um feature de algo maior
- **Customer segment pivot:** Produto certo, cliente errado
- **Problem pivot:** Solução certa para problema errado
- **Platform pivot:** App vira plataforma (ou vice-versa)

### Validated Learning

Não assumir - validar com dados reais:

❌ **Assumptions (evitar):**
- "Usuários vão querer X"
- "Se construir, eles virão"
- "Preciso de todas features antes de lançar"

✅ **Validated Learning (preferir):**
- "50% dos testadores usaram feature X 3x na primeira semana"
- "3 de 5 usuários não completaram onboarding - precisamos simplificar"
- "Usuários pedem feature Y, mas dados mostram que não usam features similares"

### Minimum Viable Product (MVP)

**Definição:** A versão de um novo produto que permite coletar o máximo de validated learning com o mínimo de esforço.

**NÃO é:**
- Produto com bugs e mal feito
- Versão "beta" com metade das features
- Desculpa para lançar algo incompleto

**É:**
- Menor experimento para testar hipótese mais arriscada
- Funcional o suficiente para entregar valor ao early adopter
- Completo no que faz, mas faz muito pouco

**Exemplo:**
- ❌ MVP mal definido: "App de to-do com CRUD básico"
- ✅ MVP bem definido: "App que permite criar tarefas e ver sugestão de priorização por IA - valida se usuários confiam e seguem a sugestão"

---

## Jobs-to-be-Done (JTBD) Framework

### Conceito Central

Pessoas não compram produtos - eles "contratam" produtos para fazer um trabalho (job).

**Exemplo clássico:**
- Harvard professor Theodore Levitt: "People don't want to buy a quarter-inch drill. They want a quarter-inch hole."
- Mas na verdade: eles querem pendurar um quadro. Ou decorar a casa. Ou impressionar visitas.

### JTBD Statement Format

```
Quando eu [SITUAÇÃO],
Eu quero [MOTIVAÇÃO],
Para que eu [OUTCOME ESPERADO]
```

**Exemplos:**

**Spotify:**
```
Quando eu estou dirigindo para o trabalho,
Eu quero ouvir música que combina com meu humor sem esforço,
Para que eu chegue energizado e de bom humor
```

**Uber:**
```
Quando eu preciso ir a um lugar e estou sem carro,
Eu quero transporte confiável sem precisar ligar ou negociar,
Para que eu chegue no horário sem stress
```

**Instagram:**
```
Quando eu tiro uma foto legal,
Eu quero compartilhar com amigos e receber validação,
Para que eu me sinta conectado e apreciado
```

### Aplicando JTBD ao seu App

**1. Identificar a Situação (Trigger)**

Quando exatamente o usuário percebe que precisa de seu app?

**Perguntas:**
- Em que momento do dia/semana isso acontece?
- O que o usuário estava fazendo antes?
- Qual evento dispara a necessidade?

**Exemplo (App de finanças pessoais):**
- ❌ Genérico: "Quando preciso controlar finanças"
- ✅ Específico: "Última semana do mês quando percebo que gastei mais do que devia"

**2. Entender a Motivação (Job-to-be-Done)**

O que o usuário realmente quer alcançar?

**Perguntas:**
- Que progresso ele quer fazer?
- O que está impedindo esse progresso hoje?
- Por que as alternativas atuais falham?

**Exemplo:**
- ❌ Superficial: "Quer controlar gastos"
- ✅ Profundo: "Quer ter tranquilidade de que não vai passar aperto no fim do mês"

**3. Definir o Outcome (Resultado Desejado)**

Como o usuário saberá que o job foi bem feito?

**Perguntas:**
- Como o usuário se sentirá?
- O que mudará na vida dele?
- Quanto tempo/dinheiro/esforço ele economizará?

**Exemplo:**
- ❌ Vago: "Ter controle financeiro"
- ✅ Claro: "Dormir tranquilo sabendo exatamente quanto pode gastar sem comprometer contas essenciais"

### Competing Alternatives

O que o usuário usa HOJE para fazer esse job?

**Categorias de alternativas:**

1. **Concorrentes diretos:** Outros apps similares
2. **Concorrentes indiretos:** Soluções diferentes para mesmo problema
3. **DIY (Do-It-Yourself):** Planilhas, papel, memória
4. **Não fazer nada:** Ignorar o problema

**Exemplo (App de meditação):**
- Direto: Headspace, Calm
- Indireto: Academia, terapia, caminhadas
- DIY: Meditação guiada no YouTube, respiração sozinho
- Não fazer: Lidar com stress sem intervir

**Por que mapear alternativas:**
- Seu app não compete só com apps similares
- Precisa ser 10x melhor que a alternativa atual (não 10% melhor)
- Entender por que alternativas falham = entender seu diferencial

### Switching Triggers

O que faria alguém trocar a solução atual pelo seu app?

**Push factors (empurram para longe da solução atual):**
- Frustração com solução atual
- Mudança de vida (novo emprego, casa, filho)
- Falha da solução atual
- Custo alto da solução atual

**Pull factors (atraem para nova solução):**
- Promessa de resultado melhor
- Economia de tempo/dinheiro
- Status / social proof
- Curiosidade / novidade

**Exemplo (Notion):**
- Push: Frustração de ter ferramentas separadas (docs no Google, tasks no Trello, wiki no Confluence)
- Pull: Promessa de "tudo em um lugar" + flexibilidade infinita

---

## Mom Test Framework

### Princípio Central

Nunca pergunte a sua mãe se sua ideia de negócio é boa. Ela vai mentir (para te proteger).

**Autor:** Rob Fitzpatrick - "The Mom Test: How to Talk to Customers and Learn if Your Business is a Good Idea When Everyone is Lying to You"

### Regras do Mom Test

**1. Fale sobre a vida deles, não sobre sua ideia**

❌ Perguntas ruins:
- "Você usaria um app que faz X?"
- "Você acha essa ideia boa?"
- "Quanto você pagaria por isso?"

✅ Perguntas boas:
- "Como você faz X hoje?"
- "Qual a última vez que teve problema Y?"
- "Quanto tempo/dinheiro perde com Z por mês?"

**2. Pergunte sobre comportamento passado, não sobre intenções futuras**

As pessoas são péssimas em prever o que farão no futuro.

❌ Perguntas ruins:
- "Você assinaria nosso app?"
- "Você usaria isso toda semana?"
- "Você indicaria para amigos?"

✅ Perguntas boas:
- "Que apps você usa diariamente hoje?"
- "Quando foi a última vez que assinou um serviço novo?"
- "Como você descobriu a última ferramenta que adotou?"

**3. Fale menos, ouça mais**

Se você está pitchando, não está aprendendo.

❌ Armadilhas:
- Explicar sua solução em detalhes
- Defender sua ideia quando questionada
- Buscar validação ("você gostou?")

✅ Objetivos:
- Entender os problemas reais
- Descobrir workarounds atuais
- Identificar o custo do problema

### Perguntas Poderosas do Mom Test

**Sobre o Problema:**
1. "Conta sobre a última vez que você teve esse problema."
2. "Por que foi difícil/frustrante?"
3. "O que você tentou fazer para resolver?"
4. "Quanto tempo/dinheiro isso custou?"
5. "Se pudesse resolver isso com uma varinha mágica, o que mudaria?"

**Sobre Soluções Atuais:**
1. "Como você lida com isso hoje?"
2. "O que você gosta na solução atual?"
3. "O que te frustra nela?"
4. "Já tentou outras ferramentas? Por que parou de usar?"
5. "O que te impediria de mudar da solução atual?"

**Sobre Prioridades:**
1. "Isso está no seu top 3 de problemas agora?"
2. "Se tivesse uma hora livre hoje, gastaria resolvendo isso?"
3. "Vale a pena pagar para resolver? Quanto já gastou tentando resolver?"

**Sobre Contexto:**
1. "Quem mais tem esse problema na sua empresa/vida?"
2. "Como você descreveria esse problema para um colega?"
3. "Que outras coisas você tenta fazer quando isso acontece?"

### Red Flags (Sinais de Alerta)

**Quando alguém diz:**
- "Eu provavelmente usaria isso" → 🚩 Não quer te magoar
- "Sempre quis algo assim!" → 🚩 Entusiasmo genérico, não validado
- "Você deveria adicionar feature X, Y, Z" → 🚩 Virando designer ao invés de usuário
- "Quanto vai custar?" → 🚩 (Pode ser bom, mas só se vier depois de demonstrar dor real)

**Sinais melhores:**
- "Eu pago $X/mês hoje para resolver algo parecido"
- "Perdi um cliente semana passada por causa desse problema"
- "Gasto 5 horas por semana fazendo isso manualmente"
- "Quando fica pronto? Quero testar ASAP"

### Como Conduzir Entrevistas do Mom Test

**Preparação:**
1. Liste suas 3 hipóteses mais arriscadas
2. Crie perguntas abertas sobre o problema (não sobre sua solução)
3. Defina critério de sucesso (ex: "5 de 7 pessoas pagam >$50/mês para resolver isso hoje")

**Durante a Conversa:**
1. Comece com contexto deles, não com sua ideia
2. Faça uma pergunta, cale a boca, escute
3. Peça exemplos específicos ("me conta sobre a última vez...")
4. Anote citações literais (palavras deles = copy do seu site)
5. Só apresente solução no final (se pedirem)

**Depois:**
1. Procure padrões (3+ pessoas com mesmo problema = padrão)
2. Categorize: Dor crítica / Nice to have / Não é problema
3. Identifique customer segment com dor mais aguda
4. Decida: construir, pivotar, ou desistir

---

## Problem-Solution Fit

### As 3 Etapas de Fit

```
PROBLEM-SOLUTION FIT → PRODUCT-MARKET FIT → SCALE
        ↓                       ↓                ↓
    Problema existe?     Solução funciona?   Crescimento sustentável?
    Vale a pena resolver?  Usuários pagam?   Custo < Revenue?
```

**Foco agora:** Problem-Solution Fit (antes de escrever código)

### Validando Problem-Solution Fit

**Objetivo:** Ter certeza que o problema existe e vale a pena resolver ANTES de construir.

**Critérios de Validação:**

1. **Problema é frequente**
   - Acontece semanalmente (ou mais)
   - Não é situação rara/edge case

2. **Problema é doloroso**
   - Causa perda de tempo/dinheiro/oportunidade significativa
   - Pessoa já tentou resolver de outras formas
   - Disposta a pagar para resolver

3. **Problema é pervasivo**
   - Muitas pessoas no target segment têm esse problema
   - Não é só você e seus amigos

4. **Você consegue alcançar quem tem o problema**
   - Sabe onde encontrar essas pessoas
   - Consegue comunicar com elas
   - Têm condições de pagar (se for pago)

### Processo de Validação (Sem Código)

**Semana 1-2: Entrevistas (20-30 pessoas)**

Use Mom Test para entrevistar pessoas do target segment.

**Meta:** Encontrar padrões consistentes de problema.

**Sucesso:**
- ✅ 70%+ tem o problema regularmente
- ✅ 50%+ considera "muito doloroso" (top 3 problemas)
- ✅ 30%+ já paga solução existente ou tentou resolver

**Failure signals:**
- 🚩 "Seria legal ter" mas ninguém paga nada hoje
- 🚩 Problema acontece raramente (<1x mês)
- 🚩 Cada pessoa descreve problema diferente (não há padrão)

**Semana 3-4: Landing Page + Waitlist**

Crie landing page explicando solução (sem construir produto).

**Elementos essenciais:**
- Headline clara do problema que resolve
- 3-5 benefícios principais
- Call-to-action: "Join waitlist" ou "Request early access"
- (Opcional) Preço indicativo

**Meta:** Medir interesse real.

**Tráfego:**
- Compartilhe em comunidades onde target segment está
- Ads pequenos ($100-200) em Google/Facebook
- Outreach direto para pessoas entrevistadas

**Sucesso:**
- ✅ 5-10% dos visitantes deixam email
- ✅ Pessoas perguntando "quando fica pronto?"
- ✅ Voluntários para testar versão beta

**Failure signals:**
- 🚩 <1% conversion (copy ruim OU problema não ressoa)
- 🚩 Tráfego não qualificado (pessoas fora do target)
- 🚩 Muitos acessos mas ninguém deixa email

### Problem Statement Template

Depois da validação, documente o problema claramente:

```markdown
## Problem Statement

**Who:** [Target segment específico, não "qualquer pessoa"]

**What:** [Problema específico, não vago]

**When:** [Situação/contexto em que problema acontece]

**Why it matters:** [Custo do problema - tempo/dinheiro/oportunidade perdido]

**Current alternatives:** [O que pessoas fazem hoje]

**Why alternatives fail:** [Por que soluções atuais não satisfazem]

**Evidence:** [Dados das entrevistas/testes]
- X% tem problema regularmente
- Y% considera muito doloroso
- Z% já tentou resolver pagando ou com workaround
```

**Exemplo:**

```markdown
## Problem Statement - App de Finanças Pessoais

**Who:** Profissionais millennials (25-35 anos) com renda média, sem dependentes

**What:** Ansiedade de não saber se podem fazer compras não-essenciais sem comprometer contas do mês

**When:** Última semana do mês, ao considerar compras >$50 (jantar fora, roupas, gadgets)

**Why it matters:**
- Gastam 2-3h por semana fazendo contas mentais
- 40% já passou aperto no fim do mês pelo menos 1x
- Sentem culpa/stress ao gastar mesmo tendo dinheiro

**Current alternatives:**
- Planilhas (20%) - trabalhoso manter atualizado
- Apps de controle (30%) - mostram gastos mas não dizem "pode gastar X hoje"
- "Feeling" (50%) - chutam e às vezes erram

**Why alternatives fail:**
- Planilhas: trabalho manual, sempre desatualizado
- Apps: mostram o passado, não ajudam decisão presente
- Feeling: insegurança constante, erros custam caro

**Evidence:**
- Entrevistamos 25 pessoas (LinkedIn, Reddit r/personalfinance)
- 22/25 (88%) têm essa ansiedade semanalmente
- 15/25 (60%) consideram top 3 fontes de stress financeiro
- 8/25 (32%) pagariam $10-20/mês por solução confiável
- Landing page: 320 visitas, 28 emails (8.75% conversion)
```

---

## MVP Definition Strategies

### Princípios para Definir MVP

**1. One Core Value Proposition**

MVP entrega UM valor principal, não "um pouco de tudo".

❌ Ruim: "App de produtividade com to-dos, calendário, notas, e pomodoro"
✅ Bom: "App que bloqueia distrações durante sessões de trabalho focado"

**2. Aha Moment Clarity**

Usuário deve experimentar o valor core em <5 minutos.

**Pergunta-chave:** "Se usuário usar só 1 feature por 5 minutos, qual feature faria ele voltar amanhã?"

**3. Fake It Before You Make It**

O que pode ser manual no MVP e automatizado depois?

**Exemplos:**
- Zapier: Zaps eram executados manualmente nos primeiros meses
- Airbnb: Fundadores tiravam fotos profissionais das casas pessoalmente
- Stripe: Suporte ao vivo em todo onboarding (parecia automático mas era humano)

**4. Narrow Target Segment**

MVP para nicho hiperespecífico, não "todo mundo".

❌ Ruim: "Ferramenta de gestão para qualquer empresa"
✅ Bom: "Ferramenta de sprint planning para squads de produto de 5-10 pessoas em startups de tech"

### MVP Scoping Canvas

Use este canvas para definir escopo:

```markdown
## MVP Scoping Canvas

### 1. Core Value Proposition
[Em 1 frase: O que o usuário consegue fazer que não conseguia antes?]

### 2. Aha Moment
[Quando/como usuário percebe o valor pela primeira vez?]

### 3. Minimum Feature Set
[3-5 features ESSENCIAIS para entregar o aha moment]

Feature 1: [Nome] - [Por que é essencial]
Feature 2: [Nome] - [Por que é essencial]
Feature 3: [Nome] - [Por que é essencial]

### 4. Explicitly OUT of Scope (v1)
[O que NÃO fazer no MVP - lista para resistir scope creep]

- [ ] Feature X - fazer só na v2 se usuários pedirem
- [ ] Feature Y - nice-to-have mas não essencial
- [ ] Feature Z - muito complexo para MVP

### 5. Manual Workarounds
[O que pode ser manual no MVP e automatizado depois?]

- [Processo X]: Manual via [método] → Automatizar na v2
- [Processo Y]: Fake backend com [ferramenta] → Build real depois

### 6. Success Metrics
[Como saberemos que MVP funciona?]

Qualitativo:
- [ ] [Métrica qualitativa 1 - ex: 5/10 usuários dizem "não consigo mais viver sem isso"]
- [ ] [Métrica qualitativa 2]

Quantitativo:
- [ ] [Métrica quantitativa 1 - ex: 50% usam 3x/semana]
- [ ] [Métrica quantitativa 2]

### 7. Validation Timeline
[Quanto tempo para validar?]

- Semana 1-2: [Build MVP]
- Semana 3-4: [Testar com 5-10 usuários]
- Semana 5: [Decidir pivot/persevere baseado em métricas]
```

### MVP Types

**1. Concierge MVP**
Fazer manualmente o serviço que será automatizado.

**Exemplo:** Food on the Table (app de receitas)
- v1: Founder ia pessoalmente na casa de clientes planejar refeições
- Aprendeu o que clientes realmente precisavam
- Depois automatizou

**Quando usar:** Serviços complexos que podem ser manuais inicialmente.

**2. Wizard of Oz MVP**
Parece automático para o usuário, mas é manual por trás.

**Exemplo:** Zapier inicial
- Interface sugeria automação instantânea
- Na verdade, equipe rodava os "zaps" manualmente

**Quando usar:** Testar se usuários valorizam automação antes de construir.

**3. Landing Page MVP**
Página explicando produto + botão de signup (produto não existe ainda).

**Exemplo:** Buffer (social media scheduling)
- Landing page com preços
- Botão "Start free trial" → "Coming soon! Join waitlist"
- Se pessoas tentam pagar, problema validado

**Quando usar:** Validar demanda antes de escrever qualquer código.

**4. Piecemeal MVP**
Juntar ferramentas existentes para simular o produto.

**Exemplo:** Groupon inicial
- WordPress para landing page
- Apple Mail para enviar cupons
- FileMaker para gerar PDFs

**Quando usar:** Validar conceito sem construir infraestrutura.

**5. Single-Feature MVP**
Produto faz 1 coisa excepcionalmente bem.

**Exemplo:** Instagram inicial
- Só fotos com filtros + feed
- Sem Stories, IGTV, Reels, Shopping (vieram depois de validar core)

**Quando usar:** A maioria dos casos - foque em fazer 1 coisa 10x melhor.

---

## Validation Metrics

### Qualitative Metrics (MVP Stage)

No início, métricas qualitativas importam mais que quantitativas.

**1. "I Can't Live Without This" Test**

Pergunte aos usuários beta: "Como você se sentiria se não pudesse mais usar esse produto?"
- "Muito desapontado" → Strong signal (aim for 40%+)
- "Somewhat disappointed" → Meh
- "Not disappointed" → Weak product-market fit

**2. Unprompted Recommendations**

Usuários recomendam sem você pedir?
- Compartilham com colegas/amigos espontaneamente
- Mencionam em redes sociais
- Pedem para convidar outras pessoas

**3. Usage Patterns**

O comportamento real combina com o esperado?
- Usuários usam o jeito que você imaginou?
- Usam features que você considerou core?
- Descobrem valor que você não antecipou?

**4. Emotional Reactions**

Como usuários descrevem o produto?
- ✅ "Finalmente!", "Exactly what I needed", "Game-changer"
- 🚩 "Interesting", "Nice to have", "I'll try it"

### Quantitative Metrics (MVP → Growth)

**Engagement:**
- **DAU/MAU (Daily Active Users / Monthly Active Users)**
  - Benchmark: >20% = bom engajamento
  - <10% = usuários não veem valor frequente

- **Session frequency**
  - Quantas vezes por semana usuário abre o app?
  - Benchmark depende do tipo de app (social: diário, ferramenta: semanal)

- **Session duration**
  - Quanto tempo passa no app por sessão?
  - Mais longo ≠ sempre melhor (depende do job-to-be-done)

**Retention:**
- **D1, D7, D30 retention**
  - D1: % que volta no dia seguinte
  - D7: % que volta na primeira semana
  - D30: % que volta no primeiro mês

- **Benchmarks (varia muito por vertical):**
  - D1: 40%+ = bom
  - D7: 20%+ = bom
  - D30: 10%+ = caminho para PMF

- **Cohort retention curves**
  - Curve flattens (retém % estável depois de drop inicial) = good
  - Curve keeps dropping to 0 = problema de value proposition

**Leading Indicators:**
- **Time to Value (TTV)**
  - Quanto tempo até usuário experimentar o aha moment?
  - Benchmark: <5 minutos para consumer, <1 semana para B2B

- **Activation rate**
  - % de signups que completam onboarding e executam core action
  - Benchmark: >40% = bem estruturado

- **Feature usage**
  - % que usa cada feature core
  - Se feature "essencial" tem <50% usage, talvez não seja essencial

### Validation Checklist (Go/No-Go Decision)

Após 4-6 semanas com 10-20 usuários beta:

**GO (prosseguir para Growth stage):**
- ✅ 40%+ diriam "very disappointed" sem o produto
- ✅ 30%+ usam semanalmente (ou mais)
- ✅ D7 retention >20%
- ✅ Usuários recomendam espontaneamente
- ✅ Consegue articular claramente por que funciona para quem funciona

**NO-GO (pivotar ou desistir):**
- 🚩 <20% diriam "very disappointed"
- 🚩 Uso declina após primeira semana
- 🚩 D7 retention <10%
- 🚩 Feedback é educado mas frio ("nice tool")
- 🚩 Não consegue identificar padrão de quem tem sucesso vs quem abandona

**ITERATE (mais tempo no MVP):**
- 🟡 Métricas medianas mas sinais mistos
- 🟡 Alguns usuários amam, outros indiferentes (refinar target segment?)
- 🟡 Onboarding confuso (TTV >30 minutos)
- 🟡 Feedback claro sobre o que está faltando

---

## Conclusion

Validar ideias antes de construir economiza meses de trabalho em produtos que ninguém quer. Use estes frameworks de forma pragmática:

1. **JTBD** para entender o problema real
2. **Mom Test** para conversar com usuários sem bias
3. **Problem-Solution Fit** para validar antes de código
4. **MVP strategies** para construir o mínimo necessário
5. **Validation metrics** para decidir objetivamente pivot vs persevere

Lembre-se: a meta não é validar que sua ideia é boa. A meta é descobrir a verdade o mais rápido possível - seja ela boa ou ruim. Descobrir que ideia não funciona em 2 semanas de validação é sucesso, não fracasso.
