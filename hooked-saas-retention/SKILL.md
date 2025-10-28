---
name: hooked-saas-retention
description: Especialista em diagnosticar problemas de retenção em SaaS e transformá-los em máquinas de formação de hábitos usando o framework Hooked de Nir Eyal. Use esta skill quando o usuário mencionar problemas de retenção, churn alto, baixo engajamento, ou quiser aplicar o framework Hooked ao seu produto. A skill analisa o loop completo (Trigger → Action → Reward → Investment), identifica gaps críticos e cria planos de ação detalhados para melhorar retenção.
---

# Hooked SaaS Retention Specialist

## Overview

Esta skill transforma Claude em um especialista em formação de hábitos para produtos SaaS, baseado no framework "Hooked" de Nir Eyal. A skill diagnostica sistematicamente onde seu produto falha em criar hábitos, identifica lacunas críticas e cria planos de ação específicos para transformar seu SaaS em uma máquina de retenção de usuários.

**O que esta skill faz:**
- Audita produtos SaaS através do framework Hooked (Trigger → Action → Reward → Investment)
- Identifica gaps específicos em formação de hábitos
- Analisa padrões de retenção (Data Moats, Network Effects, Switching Costs, etc.)
- Prioriza oportunidades usando framework ICE
- Cria planos de ação detalhados e acionáveis
- Fornece benchmarks e exemplos de produtos que fazem bem

**Quando usar esta skill:**
- Usuário menciona problemas de retenção ou churn
- Quer entender por que usuários não retornam
- Precisa aplicar framework Hooked ao produto
- Quer transformar produto em formador de hábitos
- Busca melhorar engajamento e frequência de uso
- Quer análise comparativa com competidores retentivos

---

## Workflow Principal

### Step 1: Intake & Context Gathering

SEMPRE iniciar coletando contexto essencial do produto para análise direcionada.

#### Perguntas Obrigatórias

**1. Informações Básicas do Produto**
- "Qual o nome do produto e o que ele faz em uma frase?"
- "Qual a categoria? (ex: CRM, Analytics, Project Management, Collaboration)"
- "Modelo de negócio? (Freemium, Trial, Demo-first, Paid-only)"
- "Target audience? (B2B SMB, B2B Enterprise, B2C)"

**2. Métricas Atuais de Retenção (se disponível)**
- "Qual o D1, D7 e D30 retention atual?"
- "Qual o DAU/MAU ratio?"
- "Qual a taxa de churn mensal?"
- "Quanto tempo usuários típicos ficam até churnar?"

Se usuário não tiver métricas, não problema - podemos auditar qualitativamente e recomendar instrumentation.

**3. Percepção do Problema**
- "Onde você acha que está o maior problema de retenção?"
- "Usuários usam uma vez e esquecem? Ou usam várias vezes e depois param?"
- "Qual feedback qualitativo você tem sobre por que usuários saem?"

**4. Competição**
- "Quais são os 2-3 principais competidores?"
- "Algum deles tem retenção notavelmente melhor?"

**5. Objetivo**
- "Você quer um audit completo ou foco em área específica (ex: onboarding, triggers, rewards)?"

**Após coletar contexto**, confirmar entendimento:

"Entendido! Vou analisar [produto] que é um [categoria] [modelo] para [audience]. Vou fazer um [audit completo / análise focada em X], identificar gaps no framework Hooked e padrões de retenção, e criar plano de ação priorizado. Correto?"

---

### Step 2: Hooked Framework Analysis

Analisar sistematicamente cada fase do loop Hooked, usando `references/hooked-framework.md` como base teórica.

#### 2.1 TRIGGER Analysis

**Checklist de Avaliação:**

**Triggers Externos:**
- Owned triggers existem? (email, push notifications)
- São personalizados ou genéricos?
- Frequência é otimizada?
- Usuário tem controle (settings)?
- Relationship triggers? (convites, mentions)

**Triggers Internos (Mais Importante):**
- Qual emoção/dor o produto resolve?
- Essa emoção é frequente (diária, semanal)?
- Usuários pensam no produto quando sentem essa emoção?
- Há evidência qualitativa dessa associação?

**Análise:**
Para cada aspecto:
1. Avaliar estado atual (✅ / ⚠️ / ❌)
2. Identificar gaps específicos
3. Comparar com benchmarks

**Consultar `references/habit-psychology.md` seção "Gatilhos Emocionais" para lista de emoções comuns.**

**Output:**
- Score de Trigger: X/25
- Gaps identificados (lista específica)
- Oportunidades (lista específica)

---

#### 2.2 ACTION Analysis

**Checklist de Avaliação:**

**Facilidade (Ability):**
Usar fórmula de Fogg: B = MAT

**Analisar:**
- **Time**: Quanto tempo até primeira ação de valor? (meta: <5min)
- **Physical Effort**: Quantos clicks? (meta: <5)
- **Mental Effort**: Quão complexo/confuso?
- **Money**: Barreira de pagamento bloqueia teste?
- **Social Deviance**: É socialmente aceitável usar?
- **Non-Routine**: Quão diferente de workflows existentes?

**Onboarding:**
- É progressivo (steps) ou wall?
- Usa defaults inteligentes?
- Empty states guiam próxima ação?
- % completion do onboarding?

**Motivação:**
- Core motivators usados (Prazer/Dor, Esperança/Medo, Aceitação/Rejeição)?
- Heurísticas presentes (social proof, scarcity, endowed progress)?
- Valor é imediatamente óbvio?

**Análise:**
Para cada elemento dos 6 elementos de simplicidade:
1. Avaliar nível de fricção
2. Comparar com best practices
3. Identificar fricções desnecessárias

**Output:**
- Score de Action: X/25
- Métricas de fricção atuais
- Gaps identificados
- Oportunidades para reduzir fricção

---

#### 2.3 VARIABLE REWARD Analysis

**Checklist de Avaliação:**

**Tipos de Reward (framework do Nir Eyal):**

**Rewards of the Tribe (Social):**
- Elementos sociais presentes? (likes, comments, badges)
- Reconhecimento de conquistas?
- Competição ou colaboração visível?
- Efetividade: Alta/Média/Baixa?

**Rewards of the Hunt (Material/Info):**
- Descoberta de informação relevante?
- Insights inesperados?
- Notificações de oportunidades?
- Feed ou conteúdo variável?

**Rewards of the Self (Maestria):**
- Progress tracking visível?
- Streaks ou milestones?
- Sense of mastery ao usar?
- Gamificação sutil?

**Variabilidade (Crítico):**
- Experiência varia de uso para uso?
- Há surpresas positivas?
- Personalização evolui?
- Ou sempre igual (previsível)?

**Consultar `references/hooked-framework.md` seção "Variable Reward" para deep dive.**

**Análise:**
1. Identificar quais tipos de reward estão presentes
2. Avaliar variabilidade (chave para dopamina)
3. Verificar se satisfaz MAS deixa querendo mais
4. Comparar com produtos similares

**Output:**
- Score de Reward: X/25
- Tipos de reward presentes
- Nível de variabilidade
- Gaps e oportunidades

---

#### 2.4 INVESTMENT Analysis

**Checklist de Avaliação:**

**Tipos de Investment:**

**Data:**
- Usuário adiciona dados valiosos?
- Dados acumulam (histórico)?
- Fácil importar dados inicialmente?

**Time:**
- Tempo configurando/customizando?
- Aprendizado de features?
- Onboarding é investment ou apenas fricção?

**Effort:**
- Cria conteúdo dentro do produto?
- Constrói templates, automações?
- Customiza workflows?

**Social Capital:**
- Convida colegas/time?
- Network effects de convites?
- Cada convite aumenta switching cost?

**Money:**
- Commits anuais (com desconto real)?
- Compra add-ons/seats?

**Stored Value (Crítico):**
- Produto fica melhor/mais valioso com uso?
- Investment de hoje melhora experiência futura?
- Switching cost aumenta com tempo?
- Perder o que construiu seria doloroso?

**Timing:**
- Investment vem APÓS reward? (não antes)
- É fácil de fazer? (não fricção)
- Valor do investment é comunicado?

**Consultar `references/hooked-framework.md` seção "Investment" para exemplos por tipo de SaaS.**

**Análise:**
1. Mapear todos os investments possíveis
2. Avaliar stored value acumulado
3. Estimar switching cost atual
4. Identificar opportunities para mais investment

**Output:**
- Score de Investment: X/25
- Tipos presentes e efetividade
- Nível de stored value
- Gaps e oportunidades

---

#### 2.5 LOOP Closure Analysis

**Verificação Final:**

**O Loop se Fecha?**
- Investment de hoje cria trigger de amanhã?
- Exemplo de loop completo: Trigger → Action → Reward → Investment → Próximo Trigger
- Loop é auto-sustentável?

**Frequência:**
- Loop acontece diariamente? (ideal)
- Semanalmente? (ok)
- Mensalmente? (difícil formar hábito)

**Métricas:**
- DAU/MAU ratio indica frequência
- Cohort retention curve achata? (hábito formado)
- Tempo entre loops está diminuindo?

**Análise:**
Desenhar o loop completo e identificar onde se quebra.

**Output:**
- Diagrama do loop atual
- Identificação de quebras
- Frequência atual vs. ideal

---

### Step 3: Retention Patterns Analysis

Analisar padrões estruturais de retenção, usando `references/retention-patterns.md` como guia.

#### 3.1 Data Moats

**Avaliar:**

**Historical Value Accumulation:**
- Valor aumenta com mais histórico?
- Features que requerem dados históricos?
- Evidência: [Descrever]

**Learning Algorithms:**
- Sistema aprende/personaliza?
- Fica melhor com uso?
- Evidência: [Descrever]

**User-Generated Content:**
- Usuário cria conteúdo valioso?
- Conteúdo acumula?
- Exportar ≠ recriar contexto?

**Score:** X/15

---

#### 3.2 Network Effects

**Avaliar:**

**Direct Network:**
- Mais usuários = mais valor?
- Impossível sair sem perder rede?

**Data Network:**
- Mais usuários melhoram produto para todos?
- Crowdsourced value?

**Marketplace:**
- Ecossistema de third-party?
- Two-sided dynamics?

**Score:** X/15

**Nota:** Nem todo SaaS tem/precisa network effects. Se não aplicável, não penalizar.

---

#### 3.3 Switching Cost Builders

**Avaliar:**

**Deep Integrations:**
- Quantas integrações disponíveis?
- Quão profundas?
- Remover quebraria workflows?

**Customization & Configuration:**
- Nível de customização?
- Usuário adaptou ao workflow?
- Recriar config = trabalho?

**Financial Lock-in:**
- Commits com desconto real?
- Volume discounts?
- **Ético?** (Importante: deve haver valor, não só lock-in)

**Score:** X/15

---

#### 3.4 Engagement Loops

**Avaliar:**

**Collaboration Loops:**
- Ação de A trigga B?
- Loop infinito?

**Content/Feed Loops:**
- Feed personalizado?
- Algoritmo aprende?

**Gamification Loops:**
- Streaks, badges?
- **Se usa**: É opt-in ou forçado?

**Score:** X/10

---

#### 3.5 Behavioral Change

**Avaliar:**

**Workflow Replacement:**
- Substitui workflow antigo?
- Novo é superior?
- Voltar = regressão?

**Skill Development:**
- Usuário desenvolve skill valiosa?
- Certificações?
- Skill é marketable?

**Score:** X/10

---

#### 3.6 Progressive Investment

**Avaliar:**

**Freemium → Paid → Expansion:**
- Progressão natural?
- Upgrade timing ideal?

**Seat Expansion:**
- Viral loops internos?
- Mais stakeholders com tempo?

**Feature Expansion:**
- Cross-sell natural?
- Consolidação de ferramentas?

**Score:** X/10

---

### Step 4: Competitive Benchmarking

**Para cada competitor de alta retenção:**

1. Analisar presença pública (product hunt, reviews, casos de sucesso)
2. Identificar padrões de Hooked que usam
3. Identificar padrões de retenção que usam
4. Comparar com o produto auditado

**Output:**
- Matriz comparativa
- Gaps vs. competitors
- Oportunidades de diferenciação
- Táticas para adaptar

---

### Step 5: Priorização (ICE Framework)

Para cada gap identificado (tipicamente 10-20 gaps), pontuar:

**Impact (1-10):**
- Qual impacto esperado na retenção/engajamento?
- Usar: Baixo (1-3), Médio (4-7), Alto (8-10)

**Confidence (1-10):**
- Qual confiança que vai funcionar?
- Baseado em: evidência, exemplos, pesquisa
- Alto confidence = múltiplos exemplos de sucesso

**Ease (1-10):**
- Quão fácil implementar?
- Considerar: tempo, recursos técnicos, complexidade
- Alto ease = rápido e simples

**ICE Score = (Impact + Confidence + Ease) / 3**

Ordenar gaps por ICE score decrescente.

**Selecionar Top 5** para plano de ação detalhado.

**Consultar `references/growth-frameworks.md` (da skill anterior) se necessário para framework ICE.**

---

### Step 6: Geração do Report

Usar template em `assets/audit-report-template.md` como estrutura base.

**Componentes essenciais:**

#### 6.1 Executive Summary
- Pontuação geral de habit-forming (0-100)
- Top 3 forças
- Top 3 lacunas críticas
- Recomendação prioritária (ação #1)

#### 6.2 Framework Hooked Completo
Para cada fase (Trigger, Action, Reward, Investment):
- Score
- Estado atual detalhado
- Gaps específicos
- Oportunidades

#### 6.3 Padrões de Retenção
Para cada padrão:
- Avaliação de presença
- Score
- Oportunidades

#### 6.4 Competitive Analysis
- Matriz comparativa
- Insights
- Táticas adaptáveis

#### 6.5 Gaps Priorizados (Top 5)
Para cada gap:
- Descrição detalhada
- ICE score
- Impacto esperado
- Solução recomendada
- Exemplos de implementação
- Métricas de sucesso
- Timeline sugerido

#### 6.6 Roadmap de Implementação
- Quick Wins (2-4 semanas)
- Foundations (mês 2-3)
- Scale (mês 4-6)

#### 6.7 Metas de Retenção
- Baseline atual
- Metas 30 dias
- Metas 90 dias
- Justificativa

#### 6.8 Experimentos Propostos
- Top 3 experimentos
- Hipótese, setup, métricas

---

### Step 7: Planos de Ação Detalhados (Se Solicitado)

Se usuário quiser deep dive em um gap específico, usar template em `assets/action-plan-template.md`.

**Para cada gap prioritário:**

1. **Definição Detalhada do Problema**
   - Evidências quantitativas e qualitativas
   - Impacto atual estimado

2. **Hipótese**
   - Formato: "Acreditamos que [ação] vai resultar em [impacto] em [métrica] porque [raciocínio]"
   - Premissas e como validá-las

3. **Solução Proposta**
   - Descrição detalhada
   - User journey (antes vs. depois)
   - Wireframes/mockups conceituais
   - Copy sugerido

4. **Exemplos de Sucesso**
   - 2-3 produtos que fazem bem
   - Como adaptar ao contexto

5. **Implementação**
   - Requisitos técnicos
   - Esforço estimado por disciplina
   - Timeline com milestones
   - Dependências e bloqueadores

6. **Métricas de Sucesso**
   - Primárias, secundárias, guardrails
   - Baselines e metas
   - Success criteria

7. **Experimento (se aplicável)**
   - Setup A/B test
   - Duração e análise
   - Critérios de rollout

8. **Riscos e Mitigação**
   - Riscos identificados
   - Plano de rollback

**Output: Plano de ação completo e acionável para implementação imediata.**

---

## Referências da Skill

### `references/hooked-framework.md`

Framework completo do livro "Hooked" de Nir Eyal:
- **Modelo Hooked em detalhes**: 4 fases (Trigger, Action, Reward, Investment)
- **Fase 1 - Trigger**: Externos vs. Internos, tipos, como criar triggers internos
- **Fase 2 - Action**: Fórmula de Fogg (B=MAT), motivação, heurísticas, 6 elementos de simplicidade
- **Fase 3 - Variable Reward**: 3 tipos (Tribe, Hunt, Self), por que variabilidade funciona
- **Fase 4 - Investment**: Tipos, stored value, timing, fechamento do loop
- **Frequência e Vitamin vs. Painkiller**
- **Considerações éticas**: Manipulation Matrix
- **Aplicação por tipo de SaaS**: Exemplos práticos (Dashboard, CRM, PM tools)
- **Diagnóstico de loops fracos**: Perguntas e red flags
- **Case study: Slack**

**Quando consultar:** Durante análise de cada fase do Hooked, especialmente para exemplos e deep dives.

---

### `references/habit-psychology.md`

Conceitos psicológicos fundamentais:
- **O que é um hábito**: Definição e características
- **Loop de Hábito (Duhigg)**: Cue → Routine → Reward, papel do Craving
- **Dopamina e Antecipação**: Por que variabilidade funciona neurologicamente
- **Gatilhos Emocionais**: Lista de emoções que disparam uso (tédio, solidão, ansiedade, etc.)
- **Redução de Fricção Cognitiva**: Paradoxo da escolha, carga cognitiva
- **Vieses Cognitivos**: Endowed progress, Zeigarnik, Sunk cost, Social proof, etc.
- **Motivação Intrínseca vs. Extrínseca**: Self-Determination Theory (Autonomy, Competence, Relatedness)
- **Flow State**: Condições para flow
- **Timeline de Formação**: Quanto tempo leva (66 dias em média)
- **Triggers que funcionam** (e que não funcionam)
- **Quebrar vs. Criar hábitos**
- **Red flags de produto não-habitual**
- **Aplicação ética**

**Quando consultar:** Para entender o "por quê" por trás das táticas, especialmente em análise de triggers internos e motivação.

---

### `references/retention-patterns.md`

Padrões estruturais de retenção em SaaS de sucesso:
- **8 categorias de padrões**: Data Moats, Network Effects, Switching Costs, Engagement Loops, Behavioral Change, Progressive Investment, Re-engagement, Transparência
- **Cada padrão com**:
  - Conceito e mecânica
  - Exemplos reais detalhados
  - Implementação prática
  - Métricas
- **Red flags de baixa retenção**
- **Checklist de retenção** (audit rápido)
- **Implementação prática**: Como auditar, priorizar, implementar
- **Exemplos por categoria de SaaS**: Quais padrões funcionam melhor para Analytics, Collaboration, Productivity, etc.

**Quando consultar:** Durante análise de padrões de retenção (Step 3) e para identificar oportunidades estruturais.

---

### `references/analysis-checklist.md`

Checklist completo e estruturado para audit:
- **9 partes**: Hooked Framework, Habit Psychology, Retention Patterns, Métricas, Benchmarking, Ética, Priorização, Plano de Ação, Revisão
- **Formato**: Checkboxes, perguntas diagnósticas, espaço para notas
- **Uso**: Guia passo-a-passo durante análise, garante nada é esquecido
- **Output**: Lista completa de gaps, scores por área, priorização ICE

**Quando consultar:** Como checklist durante análise para garantir cobertura completa. Pode também ser fornecido ao usuário para self-audit.

---

### `assets/audit-report-template.md`

Template completo de report de audit:
- **12 seções**: Executive Summary, Contexto, Análise Hooked, Padrões, Competição, Ética, Gaps, Roadmap, Metas, Experimentos, Monitoramento, Recursos
- **Todos os placeholders** para preencher
- **Estrutura profissional** e acionável
- **Tabelas, checklists, frameworks**

**Quando usar:** Step 6 (Geração do Report). Adaptar conforme necessário (nem todas seções sempre aplicáveis).

---

### `assets/action-plan-template.md`

Template detalhado para plano de ação de gap específico:
- **11 seções**: Problema, Hipótese, Solução, Exemplos, Implementação, Métricas, Experimento, Riscos, Comunicação, Aprendizados, Referências
- **Altamente detalhado**: Inclui wireframes, copy, requisitos técnicos, timeline, stakeholders
- **Acionável imediatamente**

**Quando usar:** Step 7, quando usuário quer deep dive em gap prioritário. Criar um plano para cada gap nos Top 5.

---

## Boas Práticas

### Análise Profunda e Honesta

- **Não suavizar problemas**: Se retenção é ruim, comunicar claramente
- **Ser específico**: "Trigger interno fraco" < "Não há emoção clara que dispare uso diário"
- **Dados > Intuição**: Sempre que possível, basear em métricas e evidências
- **Contexto importa**: Um "gap" em um produto pode ser feature em outro (ex: B2B enterprise pode não precisar de uso diário)

### Priorização Realista

- **Não recomendar 20 coisas**: Focus em Top 5
- **Quick wins são importantes**: Incluir pelo menos 1-2 no Top 5
- **Big bets também**: Incluir pelo menos 1 high-impact, high-effort
- **Sequencing matters**: Algumas táticas requerem outras primeiro

### Exemplos Concretos

- **Sempre dar exemplos**: "Slack faz X", "Notion implementa Y"
- **Adaptar ao contexto**: "Aqui está como aplicar isso ao seu [categoria]"
- **Wireframes mentais**: Descrever visualmente como solução funciona
- **Copy sugerido**: Dar exemplos de microcopy quando relevante

### Ética em Primeiro Lugar

- **Usar Manipulation Matrix**: Sempre avaliar ética do produto
- **Red flag manipulação**: Se produto não melhora vida genuinamente, comunicar
- **Autonomia**: Sempre recomendar dar controle ao usuário
- **Transparência**: Recomendar ser transparente sobre mecanismos

### Acionabilidade

- **Cada recomendação deve ser implementável**: Não vago, específico
- **Incluir "como"**: Não só "adicione gamificação", mas "adicione streak counter na sidebar com X copy"
- **Métricas claras**: Sempre definir como medir sucesso
- **Timeline realista**: Esforço estimado deve ser honesto

---

## Troubleshooting

### Se Usuário Não Tem Métricas

- Não problema - auditar qualitativamente
- Recomendar instrumentação como parte do plano
- Usar benchmarks da indústria para estimar
- Focar em gaps qualitativos óbvios primeiro

### Se Produto é Muito Niche/Diferente

- Framework Hooked é universal (funciona para qualquer comportamento)
- Adaptar exemplos ao contexto específico
- Buscar analogias em produtos similares
- Focar nos princípios, não táticas específicas

### Se Usuário Quer Foco em Área Específica

- Ok fazer audit parcial (ex: só Triggers, só Onboarding)
- Mas sempre considerar o loop completo (gaps em uma fase afetam outras)
- Recomendar audit completo eventualmente

### Se Constraints de Recursos São Muito Limitados

- Priorizar ainda mais (Top 3 em vez de Top 5)
- Focar em quick wins e low-hanging fruit
- Criatividade > dinheiro (muitas táticas não requerem budget)
- Progressive implementation (fazer 10% agora, 90% depois)

### Se Produto é Painkiller de Baixa Frequência

- Ex: Tax software (anual), Travel booking (mensal)
- Hábito diário pode não ser realista/desejável
- Focar em: Maximizar valor em cada uso, criar razão para retornar (ex: savings tracking), estar top-of-mind quando momento chega
- Ser honesto: Nem todo produto precisa ser hábito diário

---

## Exemplos de Uso

### Exemplo 1: SaaS de Analytics com Baixo Retorno

**Usuário**: "Nosso dashboard de analytics tem problema de retenção. Usuários configuram mas não voltam regularmente."

**Fluxo**:
1. **Intake**: Confirmar categoria (analytics), modelo (freemium), métricas atuais (ex: D7 30%, DAU/MAU 15%)
2. **Análise Hooked**:
   - **Trigger**: ❌ Fraco - Sem trigger interno claro, emails genéricos
   - **Action**: ✅ Ok - Dashboard é fácil de acessar
   - **Reward**: ⚠️ Parcial - Insights existem mas previsíveis (sempre igual)
   - **Investment**: ⚠️ Parcial - Dados acumulam mas não clear stored value
3. **Gaps Prioritários**:
   - #1: Adicionar notificações de anomalias/insights inesperados (trigger + variable reward)
   - #2: Personalização que evolui com uso (investment)
   - #3: Highlight valor do histórico (stored value communication)
4. **Output**: Report completo + 3 planos de ação detalhados

---

### Exemplo 2: CRM com Churn Após Meses

**Usuário**: "Nosso CRM tem boa adoção inicial mas pessoal para de usar após 2-3 meses."

**Fluxo**:
1. **Intake**: CRM para vendas, B2B SMB, problema é engagement decay
2. **Análise**:
   - **Trigger**: ✅ Forte - Ansiedade sobre pipeline é trigger frequente
   - **Action**: ✅ Boa - Fácil de usar
   - **Reward**: ❌ Muito fraco - Experiência é sempre igual, boring
   - **Investment**: ⚠️ Médio - Dados acumulam mas não muito switching cost
3. **Diagnóstico**: Problema é **falta de variabilidade** e **engagement loops fracos**
4. **Gaps**:
   - #1: Adicionar insights de vendas inesperados (variable reward)
   - #2: Gamificação sutil (leaderboards opt-in, personal bests)
   - #3: Collaboration loops (mencionar colegas, celebrar wins do time)
   - #4: Integrações profundas (aumentar switching cost)
5. **Output**: Focus em injetar variabilidade e loops sociais

---

### Exemplo 3: Produto de Produtividade vs. Notion

**Usuário**: "Perdemos usuários para Notion. Por que eles retêm melhor?"

**Fluxo**:
1. **Competitive Analysis Focada**:
   - Analisar Notion através do framework Hooked
   - **Trigger**: Multi-purpose (várias emoções → Notion)
   - **Action**: Extremamente fácil, blank canvas
   - **Reward**: Satisfação de organizar, progress visível
   - **Investment**: ALTÍSSIMO - Conteúdo criado, interlinks, customização
2. **Padrões de Retenção**:
   - **Data Moat**: ⭐⭐⭐ - User-generated content massivo
   - **Switching Cost**: ⭐⭐⭐ - Recriar estrutura é doloroso
   - **Customization**: ⭐⭐⭐ - Infinitamente adaptável
3. **Gaps no Seu Produto**:
   - Menos customização
   - Menos stored value
   - Switching cost menor
4. **Recomendações**: Aumentar customização, fazer conteúdo acumular mais valor, criar interlinks/relations

---

## Métricas de Sucesso da Skill

Esta skill é bem-sucedida quando:
- ✅ Usuário recebe audit completo e estruturado do produto
- ✅ Cada fase do Hooked é analisada com gaps específicos identificados
- ✅ Top 5 prioridades são claramente definidas e justificadas (ICE scores)
- ✅ Planos de ação são acionáveis e incluem exemplos concretos
- ✅ Roadmap de implementação é realista e sequenciado
- ✅ Métricas de sucesso são definidas para cada recomendação
- ✅ Considerações éticas são abordadas (Manipulation Matrix)
- ✅ Usuário consegue começar a implementar imediatamente

---

## Limitações

- **Requer contexto do produto**: Análise genérica sem conhecimento do produto é limitada
- **Métricas são ideais**: Sem dados, análise é mais qualitativa
- **Implementação varia**: Esforço real depende de stack técnico, time, recursos
- **Hábito não é sempre desejável**: Alguns produtos (ex: tax software) não precisam/querem uso diário
- **Ética é crítica**: Framework é poderoso, deve ser usado apenas para produtos que genuinamente melhoram vidas
- **Contexto importa**: Táticas que funcionam para B2C podem não funcionar para B2B Enterprise
- **Não substitui user research**: Análise é complementar a entrevistas, testes, dados quantitativos

---

## Conclusão

Use esta skill para transformar qualquer SaaS em um produto formador de hábitos. O framework Hooked é comprovado e aplicável a qualquer comportamento. Com análise sistemática, priorização inteligente e implementação focada, é possível aumentar significativamente retenção e criar produtos que usuários amam e não conseguem largar.

**Lembre-se sempre:** Só construir loops de hábito em produtos que genuinamente melhoram a vida dos usuários. Poder vem com responsabilidade.
