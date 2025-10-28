# Checklist Completo de Análise de Retenção

Guia estruturado para diagnosticar lacunas no seu SaaS e identificar oportunidades de melhoria na retenção.

---

## Como Usar Este Checklist

1. **Responda cada pergunta honestamente** (Sim/Não/Parcial)
2. **Anote evidências** (dados, métricas, observações)
3. **Identifique gaps críticos** (Nãos e Parciais)
4. **Priorize** por impacto potencial vs. esforço
5. **Crie plano de ação** para top 5 gaps

---

## PARTE 1: HOOKED FRAMEWORK AUDIT

### 1.1 TRIGGER (Gatilho)

#### Triggers Externos

**Owned Triggers:**
- [ ] Temos notificações push implementadas?
- [ ] Emails de re-engagement são enviados?
- [ ] Notificações são personalizadas (não genéricas)?
- [ ] Frequência de triggers é otimizada (não spam)?
- [ ] Usuário pode controlar preferências de notificação?

**Relationship Triggers:**
- [ ] Produto incentiva convites/compartilhamentos?
- [ ] Há mecanismo de "convide seu time"?
- [ ] Notificações sociais ("João te mencionou")?
- [ ] Network effects ajudam trigger?

**Métricas:**
- Taxa de abertura de emails: ____%
- Engagement rate em notificações push: ____%
- % usuários que convidam outros: ____%

#### Triggers Internos

**Emoção Core:**
- [ ] Identificamos a emoção/dor primária que resolvemos?
- [ ] Essa emoção é sentida frequentemente (diária/semanal)?
- [ ] Usuários pensam no nosso produto quando sentem essa emoção?
- [ ] Temos evidência qualitativa disso (entrevistas, surveys)?

**Perguntas Diagnósticas:**
- Qual emoção/situação faz usuário abrir nosso produto? _____________
- Com que frequência essa emoção ocorre? (Diária/Semanal/Mensal) _____________
- Competidores resolvem mesma emoção? _____________

**Red Flags:**
- [ ] Usuários dizem "só uso quando lembro"
- [ ] Dependemos de email marketing para tráfego
- [ ] Não há associação emocional clara
- [ ] Produto é "nice to have", não "need to have"

---

### 1.2 ACTION (Ação)

#### Facilidade (Ability)

**Time (Tempo):**
- [ ] Usuário consegue completar primeira ação de valor em < 5 min?
- [ ] Onboarding é rápido (não horas)?
- [ ] Login é rápido (SSO disponível)?

**Physical & Mental Effort:**
- [ ] Quantos cliques até primeira ação de valor? (meta: < 5) ____
- [ ] Interface é intuitiva (sem necessidade de manual)?
- [ ] Usamos defaults inteligentes?
- [ ] Reduzimos campos de formulários ao mínimo?

**Money:**
- [ ] Free tier ou trial disponível?
- [ ] Barreira de pagamento não bloqueia teste de valor?

**Progressive Disclosure:**
- [ ] Revelamos features progressivamente (não tudo de uma vez)?
- [ ] Empty states guiam próxima ação?
- [ ] Onboarding é em steps (não uma wall)?

**Móbile:**
- [ ] Temos app móbile? (se faz sentido)
- [ ] Experiência móbile é boa?
- [ ] Action pode ser feita do celular?

**Métricas:**
- Time to first value: ____ minutos
- % usuários que completam onboarding: ____%
- % usuários que fazem segunda ação: ____%

**Red Flags:**
- [ ] Onboarding leva >30min
- [ ] Requer treinamento/demo para usar
- [ ] Usuários ficam perdidos (feedback qualitativo)
- [ ] Alta taxa de drop-off no onboarding

---

#### Motivação

**Core Motivators Usados:**
- [ ] Prazer/Dor: Destacamos prazer de sucesso ou dor de falha?
- [ ] Esperança/Medo: Vendemos esperança de resultado ou medo de perder?
- [ ] Aceitação/Rejeição: Usamos social proof, "todos estão usando"?

**Heurísticas:**
- [ ] Usamos social proof? ("10k empresas confiam")
- [ ] Escassez? ("Oferta limitada") - se relevante
- [ ] Endowed progress? ("Seu perfil está 30% completo")
- [ ] Framing positivo? ("90% de sucesso" vs "10% falha")

**Red Flags:**
- [ ] Valor do produto não é imediatamente óbvio
- [ ] Usuário não vê "o que eu ganho"
- [ ] Sem social proof

---

### 1.3 VARIABLE REWARD (Recompensa Variável)

#### Tipo de Recompensa

**Rewards of the Tribe (Social):**
- [ ] Há elementos sociais? (likes, comments, mentions)
- [ ] Reconhecimento de conquistas?
- [ ] Leaderboards ou rankings? (se aplicável)
- [ ] Badges/status?

**Rewards of the Hunt (Material/Info):**
- [ ] Insights variáveis? (às vezes surpreende, às vezes não)
- [ ] Notificações de oportunidades?
- [ ] Descoberta de informação relevante?
- [ ] Feed ou dashboard com variabilidade?

**Rewards of the Self (Maestria):**
- [ ] Progress bars, completion tracking?
- [ ] Streaks ou usage tracking?
- [ ] Sense of mastery ao usar produto?
- [ ] Achievements por milestones?

#### Variabilidade

**Checklist de Variabilidade:**
- [ ] Experiência varia de uso para uso? (não sempre igual)
- [ ] Há surpresas positivas ocasionais?
- [ ] Algoritmo personaliza experiência?
- [ ] Usuário não consegue prever exatamente o que vai encontrar?

**Evitar:**
- [ ] Experiência é sempre igual (previsível 100%)
- [ ] Relatórios sempre idênticos
- [ ] Nenhuma personalização
- [ ] "Vi uma vez, vi tudo"

**Métricas:**
- % sessões com descoberta de novo insight: ____%
- Variedade de features usadas por sessão: ____
- NPS ou "surprise & delight" feedback: ____

**Red Flags:**
- [ ] Dashboard sempre mostra mesma coisa
- [ ] Sem personalização alguma
- [ ] Usuários dizem "fica boring after a while"
- [ ] Churn depois de primeiras semanas (novidade passa)

---

### 1.4 INVESTMENT (Investimento)

#### Tipos de Investment

**Data:**
- [ ] Usuário adiciona dados que ficam armazenados?
- [ ] Importação de dados é fácil?
- [ ] Dados acumulam valor com tempo?
- [ ] Histórico é relevante e valioso?

**Time:**
- [ ] Usuário investe tempo configurando?
- [ ] Aprende features/workflows?
- [ ] Customiza produto ao seu uso?

**Effort:**
- [ ] Cria conteúdo dentro do produto?
- [ ] Constrói templates, automações?
- [ ] Esforço melhora experiência futura?

**Social Capital:**
- [ ] Convida colegas/time?
- [ ] Cada convite aumenta switching cost?
- [ ] Network effect de convites?

**Money:**
- [ ] Commitment financeiro (anual, por ex.)?
- [ ] Compra de add-ons/seats aumenta investment?

#### Stored Value

**Checklist:**
- [ ] Produto fica melhor/mais valioso com mais uso?
- [ ] Investment de hoje melhora experiência de amanhã?
- [ ] Switching cost aumenta com tempo?
- [ ] Perder o que construiu seria doloroso?

**Métricas:**
- Volume médio de dados por usuário: ____
- Número médio de configurações/customizações: ____
- % usuários que convidaram alguém: ____%
- Tempo médio investido em setup: ____ min

#### Timing

**Checklist:**
- [ ] Pedimos investment APÓS recompensa (não antes)?
- [ ] Investment é fácil de fazer (não fricção)?
- [ ] Comunicamos valor do investment? ("Isso vai deixar próxima vez mais rápida")

**Red Flags:**
- [ ] Produto não melhora com uso
- [ ] Experiência do dia 1 = dia 100 (flat)
- [ ] Nada acumula (sem stored value)
- [ ] Fácil exportar tudo e trocar de ferramenta

---

### 1.5 LOOP (Fechamento)

#### Loop se Fecha?

**Checklist:**
- [ ] Investment de hoje cria trigger de amanhã?
- [ ] Mais dados → Melhores insights → Notificações → Voltar
- [ ] Mais conexões → Mais atividade → Notificações → Voltar
- [ ] Loop é auto-sustentável?

**Frequência:**
- [ ] Loop completo acontece diariamente?
- [ ] Se não diário, pelo menos semanal?
- [ ] Múltiplos loops possíveis?

**Métricas:**
- % usuários que retornam D1: ____%
- % usuários que retornam D7: ____%
- % usuários que retornam D30: ____%
- DAU/MAU ratio: ____%

**Red Flags:**
- [ ] Usuários usam uma vez e esquecem
- [ ] Sem razão natural para retornar
- [ ] Investment não gera novos triggers
- [ ] Retention curve não achata (continua caindo)

---

## PARTE 2: HABIT PSYCHOLOGY AUDIT

### 2.1 Habit Loop (Duhigg)

**Cue:**
- [ ] Identificamos os cues (localização, tempo, emoção, pessoas, ação anterior)?
- [ ] Cues são consistentes e previsíveis?

**Craving:**
- [ ] Usuários antecipam a recompensa?
- [ ] Há desejo/craving pelo uso do produto?
- [ ] Evidência qualitativa de craving?

**Routine:**
- [ ] Rotina é simples e automática?
- [ ] Não requer esforço consciente após hábito formado?

**Reward:**
- [ ] Recompensa satisfaz o craving?
- [ ] Reforça o loop cue-routine?

### 2.2 Dopamina e Antecipação

- [ ] Criamos antecipação (não só realização)?
- [ ] Variabilidade aumenta dopamina?
- [ ] Usuários ficam curiosos sobre "o que vou encontrar"?

### 2.3 Gatilhos Emocionais

- [ ] Identificamos emoção primária?
- [ ] Produto é associado a essa emoção?
- [ ] Emoção ocorre frequentemente?
- [ ] Pesquisa qualitativa confirma?

### 2.4 Fricção Cognitiva

- [ ] Reduzimos paradoxo da escolha (poucos options)?
- [ ] Carga cognitiva é baixa?
- [ ] UI é clara e não sobrecarrega?

### 2.5 Vieses Cognitivos

- [ ] Usamos endowed progress?
- [ ] Aproveitamos Zeigarnik (tarefas incompletas)?
- [ ] Destacamos sunk cost ("você já investiu X")?
- [ ] Social proof presente?
- [ ] Loss aversion (quando relevante)?

### 2.6 Motivação Intrínseca

**Self-Determination Theory:**
- [ ] Autonomy: Usuário sente controle?
- [ ] Competence: Usuário sente que está melhorando?
- [ ] Relatedness: Há conexão social/community?

### 2.7 Flow

- [ ] Desafio e habilidade balanceados?
- [ ] Metas claras?
- [ ] Feedback imediato?
- [ ] Usuários entram em "flow state"?

### 2.8 Timeline de Formação

- [ ] Sabemos quanto tempo leva para formar hábito no nosso produto?
- [ ] Otimizamos primeiros 30-60 dias (críticos)?
- [ ] Curva de retenção achata após período de formação?

---

## PARTE 3: RETENTION PATTERNS AUDIT

### 3.1 Data Moats

**Historical Value:**
- [ ] Valor aumenta com dados históricos?
- [ ] Trends, forecasts requerem histórico?
- [ ] Perder histórico seria doloroso?

**Learning Algorithms:**
- [ ] Sistema aprende com uso?
- [ ] Personalização evolui?
- [ ] Recomeçar em competitor seria regressivo?

**User-Generated Content:**
- [ ] Usuário cria conteúdo valioso?
- [ ] Conteúdo acumula?
- [ ] Exportar ≠ recriar contexto?

### 3.2 Network Effects

**Direct Network:**
- [ ] Mais usuários = mais valor?
- [ ] Impossível sair sem perder rede?

**Data Network:**
- [ ] Mais usuários melhoram produto para todos?

**Marketplace:**
- [ ] Ecossistema de third-party?
- [ ] Two-sided market?

### 3.3 Switching Cost Builders

**Deep Integrations:**
- [ ] Integrado com stack do usuário?
- [ ] Remover quebraria workflows?
- [ ] Custom integrations criadas?

**Customization:**
- [ ] Altamente customizável?
- [ ] Usuário adaptou ao workflow dele?
- [ ] Recriar config em outro produto = work?

**Financial Lock-in:**
- [ ] Commits anuais com desconto?
- [ ] Volume discounts?
- [ ] (Ético: Há valor real, não só lock-in artificial?)

### 3.4 Engagement Loops

**Collaboration:**
- [ ] Ação de A trigga B?
- [ ] Loops infinitos de colaboração?

**Content/Feed:**
- [ ] Feed personalizado evolui?
- [ ] Algoritmo aprende?

**Gamification:**
- [ ] Streaks, badges, leaderboards?
- [ ] (Se usa): É opt-in ou forçado?

### 3.5 Behavioral Change

**Workflow Replacement:**
- [ ] Substitui workflow antigo completamente?
- [ ] Novo workflow é superior?
- [ ] Voltar seria regressão?

**Skill Development:**
- [ ] Usuário desenvolve skill?
- [ ] Skill é valiosa no mercado?
- [ ] Certificações, trainings?

### 3.6 Progressive Investment

**Freemium → Paid:**
- [ ] Free tier permite investment real?
- [ ] Upgrade timing é natural?

**Seat Expansion:**
- [ ] Usuário convida naturalmente outros?
- [ ] Mais stakeholders com tempo?

**Feature Expansion:**
- [ ] Cross-sell natural?
- [ ] Consolidação de ferramentas?

---

## PARTE 4: MÉTRICAS E DADOS

### 4.1 Habit Testing

**Sean Ellis Test:**
- [ ] Perguntamos: "Como se sentiria se não pudesse usar produto?"
- [ ] % "Muito desapontado": ____% (meta: >40%)

### 4.2 Retenção Cohort

- [ ] Rastreamos D1, D7, D30, D90 retention?
- [ ] Curva de retenção achata (hábito formado)?
- [ ] Cohorts recentes retêm melhor? (produto melhorando)

**Dados:**
- D1 retention: ____%
- D7 retention: ____%
- D30 retention: ____%
- D90 retention: ____%

### 4.3 Engajamento

- [ ] DAU/MAU ratio >20%?
- [ ] Frequência de uso está aumentando?
- [ ] Power users crescendo como % de base?

**Dados:**
- DAU/MAU: ____%
- Sessões por usuário por semana: ____
- % power users (diários): ____%

### 4.4 Profundidade de Investment

- [ ] % usuários que fazem ≥1 investment?
- [ ] Investment aumenta com tempo?
- [ ] Correlação entre investment e retention?

**Dados:**
- % usuários com dados armazenados: ____%
- Média de integrações por usuário: ____
- Média de convites enviados: ____

### 4.5 Velocidade dos Loops

- [ ] Sabemos tempo médio de loop completo?
- [ ] Loops por usuário por semana?
- [ ] Loops estão acelerando?

### 4.6 Churn Analysis

- [ ] Sabemos por que usuários saem?
- [ ] Categorizamos razões de churn?
- [ ] Identificamos at-risk users antes de churnar?

**Churn Reasons (top 3):**
1. ________________
2. ________________
3. ________________

---

## PARTE 5: BENCHMARKING COMPETITIVO

### 5.1 Análise de Competidores Retentivos

**Para cada competitor com boa retenção:**

**Competitor 1: ________________**
- Qual trigger interno usam? ________________
- Quão fácil é a action? ________________
- Que tipo de reward oferecem? ________________
- Investment mechanisms: ________________
- Padrões de retenção usados: ________________

**Competitor 2: ________________**
- (Repetir perguntas)

**Competitor 3: ________________**
- (Repetir perguntas)

### 5.2 O que Aprendemos?

- [ ] Quais padrões competitors usam que nós não?
- [ ] Onde eles são mais fortes?
- [ ] Onde podemos diferencial?

---

## PARTE 6: QUESTÕES ÉTICAS

### 6.1 Manipulation Matrix (Nir Eyal)

- [ ] Você usa o próprio produto regularmente?
- [ ] Produto genuinamente melhora vida/trabalho dos usuários?
- [ ] Se sim a ambos → Facilitator ✅
- [ ] Se não ao primeiro mas sim ao segundo → Peddler (cuidado)
- [ ] Se sim ao primeiro mas não ao segundo → Entertainer (questionável)
- [ ] Se não a ambos → Dealer (evitar)

### 6.2 Transparência

- [ ] Somos transparentes sobre como produto funciona?
- [ ] Usuários sabem por que estão sendo triggerados?
- [ ] Facilitamos saída (export, delete)?
- [ ] Respeitamos autonomia do usuário?

### 6.3 Bem-Estar do Usuário

- [ ] Produto ajuda usuário ser mais produtivo/feliz?
- [ ] Ou só vicia sem benefício real?
- [ ] Há controles para usuário gerenciar uso? (ex: pausa, snooze)

---

## PARTE 7: PRIORIZAÇÃO

### 7.1 Gaps Críticos Identificados

Liste todos os "Não" ou "Parcial" do checklist:

1. ________________ (Área: ________)
2. ________________ (Área: ________)
3. ________________ (Área: ________)
4. ________________ (Área: ________)
5. ________________ (Área: ________)
[...]

### 7.2 ICE Scoring

Para cada gap, pontuar 1-10:

| Gap | Impact | Confidence | Ease | ICE Score |
|-----|--------|------------|------|-----------|
| 1.  |        |            |      |           |
| 2.  |        |            |      |           |
| 3.  |        |            |      |           |
| 4.  |        |            |      |           |
| 5.  |        |            |      |           |

### 7.3 Top 5 Prioridades

Baseado em ICE score:

1. ________________ (ICE: ____)
2. ________________ (ICE: ____)
3. ________________ (ICE: ____)
4. ________________ (ICE: ____)
5. ________________ (ICE: ____)

---

## PARTE 8: PLANO DE AÇÃO

### 8.1 Para Cada Prioridade

**Prioridade #1: ________________**

**Problema:**
[Descrever gap específico]

**Hipótese:**
[Como resolver vai melhorar retenção]

**Solução:**
[O que implementar especificamente]

**Métricas de Sucesso:**
- Primária: ________________
- Secundária: ________________
- Meta: ________________

**Timeline:**
- Inicio: ______
- Entrega: ______

**Owner:**
[Quem é responsável]

---

**Prioridade #2: ________________**
[Repetir estrutura]

---

**Prioridade #3: ________________**
[Repetir estrutura]

---

## PARTE 9: REVISÃO E ITERAÇÃO

### 9.1 Cadência de Revisão

- [ ] Revisão semanal de métricas de retenção?
- [ ] Revisão mensal de experimentos?
- [ ] Revisão trimestral completa de hábito/retenção?

### 9.2 Aprendizados

**O que funcionou:**
- ________________
- ________________

**O que não funcionou:**
- ________________
- ________________

**Próximos experimentos:**
- ________________
- ________________

---

## RESUMO EXECUTIVO DO AUDIT

### Pontuação Geral

Total de "Sim": ____ / ____ (____%)
Total de "Não": ____ / ____ (____%)
Total de "Parcial": ____ / ____ (____%)

### Áreas Mais Fortes

1. ________________
2. ________________
3. ________________

### Áreas Mais Fracas (Ação Urgente)

1. ________________
2. ________________
3. ________________

### Recomendação #1 (Quick Win)

[Gap de alto impacto e baixo esforço para resolver primeiro]

### Recomendação #2 (Strategic)

[Gap de alto impacto que leva mais tempo mas é crítico]

### Meta de Retenção

**Atual:**
- D30 retention: ____%
- DAU/MAU: ____%

**Meta (90 dias):**
- D30 retention: ____%
- DAU/MAU: ____%

---

## NOTAS E OBSERVAÇÕES ADICIONAIS

[Espaço para insights qualitativos, feedback de usuários, observações importantes que não se encaixam nas seções acima]

________________
________________
________________
________________
