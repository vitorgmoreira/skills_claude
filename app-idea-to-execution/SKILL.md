---
name: app-idea-to-execution
description: Transforms app ideas into professionally structured, executable projects with comprehensive planning (PRD, architecture, roadmap) and phased implementation guidance. Use when users want to build an app from an idea, need help structuring a project, or want to transform a concept into a development roadmap.
---

# App Idea to Execution

## Overview

This skill transforms app ideas into professionally structured, executable projects through a systematic workflow that covers validation, planning, architecture, and phased implementation. It combines proven product management frameworks (Lean Startup, JTBD, AARRR) with software engineering best practices to ensure projects are well-planned, prioritized, and executed incrementally.

The skill is designed for developers (solo or small teams) building fullstack web applications who need structure to avoid getting lost in complexity, want to follow professional standards, and need guidance on breaking down projects into manageable phases.

## Core Philosophy

### Framework-Driven, Not Generic
Use validated frameworks for each stage (Problem-Solution Fit, ICE/RICE prioritization, AARRR breakdown) rather than ad-hoc advice. Every recommendation should be grounded in established methodology.

### Context-First Approach
ALWAYS collect comprehensive context before recommending solutions. Understand the app idea, user's technical level, project constraints, and goals before proceeding.

### Phased and Iterative
Break projects into realistic phases (Foundation → Growth → Scale) with clear validation checkpoints. Avoid big-bang development - build incrementally with frequent validation.

### Actionable Over Theoretical
Provide specific action items, timelines, and metrics rather than abstract concepts. Every output should enable immediate next steps.

### Professional Standards
Follow industry best practices for documentation (PRD, architecture docs), planning (OKRs, roadmaps), and execution (sprints, metrics tracking).

## When to Use This Skill

Use this skill when:
- User wants to build a web app from an idea
- User has a concept but doesn't know how to start structuring the project
- User needs help creating a PRD, architecture, or roadmap
- User wants to break down a complex project into phases
- User asks about project planning, prioritization, or execution strategies
- User mentions feeling lost or overwhelmed with project scope

Do NOT use for:
- Simple bug fixes or small features in existing projects
- Pure research or documentation tasks
- Non-web applications (though principles may adapt)

## Workflow

Follow this 5-step workflow sequentially. Each step builds on the previous one.

### Step 1: Elicitação da Ideia (Context Gathering)

**Objetivo:** Understand the app idea, user context, and constraints comprehensively before any recommendations.

**Questions to Ask:**

1. **Sobre a Ideia:**
   - Descreva sua ideia de app em 2-3 frases
   - Que problema específico ele resolve?
   - Quem é o usuário-alvo?
   - Já existe algo similar? O que faria seu app diferente?

2. **Contexto Técnico:**
   - Qual seu nível de experiência? (iniciante / intermediário / avançado)
   - Tem preferências de tech stack? (React, Vue, Node, Python, etc.)
   - Pretende hospedar onde? (Vercel, AWS, outro?)
   - Vai trabalhar sozinho ou em equipe?

3. **Objetivos e Constraints:**
   - Prazo esperado para ter algo funcionando?
   - Pretende monetizar? Como?
   - Já tem usuários em mente para validar?
   - Alguma limitação de tempo/recursos?

**Output:** Summary document com todas as informações coletadas para referência nas próximas etapas.

### Step 2: Validação da Ideia (Problem-Solution Fit)

**Objetivo:** Validar se a ideia resolve um problema real e definir o escopo mínimo viável.

**Atividades:**

1. **Problem Definition usando Jobs-to-be-Done (JTBD):**
   - Quando o usuário "contrata" este app? (situação específica)
   - O que ele está tentando alcançar? (progresso desejado)
   - O que ele usa hoje? (alternativas atuais)
   - Por que as alternativas não satisfazem? (custo do problema)

2. **Solution Hypothesis:**
   - Core value proposition em 1 frase
   - "Aha moment" - momento em que usuário percebe o valor
   - 3-5 features essenciais para entregar esse valor
   - O que NÃO fazer na v1 (scope control)

3. **MVP Definition:**
   - Qual a versão mais simples que entrega o "aha moment"?
   - O que pode ser manual/fake backend inicialmente?
   - Como validar se funciona? (métricas qualitativas)

**Refer to:** `references/idea-validation.md` for detailed frameworks (Lean Startup, Mom Test, JTBD)

**Output:**
- Problem statement claro
- MVP scope definido (3-5 features core)
- Validation plan (como testar com primeiros usuários)

### Step 3: Planejamento Completo (PRD + Architecture + Priorities)

**Objetivo:** Criar documentação profissional completa que serve como guia para toda implementação.

**3.1 Product Requirements Document (PRD)**

Create comprehensive PRD using template in `assets/prd-template.md`:

- **Product Vision & Strategy:**
  - North Star Metric (métrica principal de sucesso)
  - Input Metrics (o que impulsiona a NSM)
  - Product Strategy Stack (Vision → Strategy → Roadmap)

- **User Stories & Features:**
  - User personas
  - User stories no formato: "Como [persona], eu quero [ação] para [benefício]"
  - Acceptance criteria para cada feature

- **Success Metrics:**
  - Métricas quantitativas (uso semanal, retenção, etc.)
  - Métricas qualitativas (feedback, NPS)
  - Definir targets realistas

**3.2 Technical Architecture**

Design fullstack architecture using template in `assets/architecture-doc-template.md`:

- **System Architecture:**
  - Diagrama de componentes (Frontend, Backend, Database, APIs)
  - Tech stack justificado (por que cada escolha)
  - Architectural Decision Records (ADRs) para decisões importantes

- **Data Model:**
  - Entidades principais e relacionamentos
  - Schema de banco de dados
  - Fluxo de dados na aplicação

- **API Design:**
  - Principais endpoints (RESTful ou GraphQL)
  - Autenticação/autorização strategy
  - Rate limiting e segurança

- **Infrastructure & DevOps:**
  - Ambientes (dev, staging, production)
  - Deploy strategy e CI/CD
  - Monitoring, logging, error tracking

**Refer to:** `references/prd-architecture.md` for detailed guidance on fullstack architecture patterns

**3.3 Feature Prioritization**

Use ICE or RICE scoring for each feature:

**ICE Score = (Impact + Confidence + Ease) / 3**
- Impact: Impacto no usuário/negócio (1-10)
- Confidence: Confiança de que funcionará (1-10)
- Ease: Facilidade de implementação (1-10)

**RICE Score = (Reach × Impact × Confidence) / Effort**
- Reach: Quantos usuários afeta por período
- Impact: Quanto impacta (0.25 = mínimo, 3 = massive)
- Confidence: % de confiança (0-100%)
- Effort: Person-weeks de trabalho

Create prioritized backlog ordenado por score.

**Refer to:** `references/project-breakdown.md` for prioritization frameworks

**Output:**
- PRD completo (5-10 páginas)
- Architecture document (3-5 páginas com diagramas)
- Feature backlog priorizado com scores

### Step 4: Breakdown Executável (Roadmap + Sprints + OKRs)

**Objetivo:** Transformar o planejamento em roadmap executável com fases, sprints e métricas claras.

**4.1 Define Project OKRs**

Use template in `assets/okr-project-template.md`:

**Ciclo recomendado:**
- **Mensal** para MVPs e early stage (0-3 meses)
- **Trimestral** para projetos estabelecidos (3+ meses)

**Exemplo:**
```
Objective: Lançar MVP validado com primeiros usuários
  KR1: 5-10 usuários testadores ativos semanalmente
  KR2: Feature principal usada 3x/semana por usuário
  KR3: 80% dos usuários completam onboarding
  KR4: NPS qualitativo > 40
```

**4.2 Phase-Based Roadmap**

Break project into 3 stages usando framework de Stage-Based Development:

**Fase 1: Foundation (0-4 semanas)**
- Objetivo: Validar Problem-Solution Fit com MVP funcional
- Escopo: 3-5 features core do MVP
- Métricas: Qualitativas (feedback), uso semanal por 5-10 testadores
- Entregáveis:
  - Setup inicial (repo, CI/CD, ambientes)
  - Implementação do fluxo principal (happy path)
  - UI básica funcional (não precisa ser bonita)
  - Deploy em staging/production

**Fase 2: Growth (4-12 semanas)**
- Objetivo: Escalar o que funciona, otimizar experiência
- Escopo: Polimento do MVP + features secundárias priorizadas
- Métricas: Engajamento, retenção semanal, time-to-value
- Entregáveis:
  - Onboarding otimizado
  - Top 3-5 features do backlog priorizado
  - Performance e UX melhorados
  - Analytics implementado

**Fase 3: Scale (12+ semanas)**
- Objetivo: Eficiência, automação, crescimento sustentável
- Escopo: Automação, growth loops, monetização
- Métricas: Custo por usuário, LTV, growth rate
- Entregáveis:
  - Processos automatizados
  - Growth features (referral, viral loops)
  - Monetização (se aplicável)
  - Documentation e testes robustos

**4.3 Sprint Planning**

For each phase, break into sprints using `assets/weekly-sprint-template.md`:

**Sprint semanal ou quinzenal:**
- Sprint Goal (objetivo claro em 1 frase)
- Tarefas priorizadas com estimativas
- Definition of Done para cada tarefa
- Retrospective ao final (o que funcionou, o que melhorar)

**Refer to:**
- `references/project-breakdown.md` for AARRR framework, Stage-Based Development
- `references/agile-solo-dev.md` for sprint planning and solo dev practices
- `references/execution-frameworks.md` for OKRs and implementation roadmaps

**Output:**
- Project OKRs definidos
- Roadmap de 3 fases com escopo, métricas e entregáveis
- Sprints da Fase 1 planejados em detalhe
- Weekly planning template pronto para uso

### Step 5: Execução Assistida (Implementation + Validation)

**Objetivo:** Executar o roadmap fase por fase, validando checkpoints e iterando baseado em feedback.

**5.1 Execution Protocol**

For each sprint/phase:

1. **Pre-Sprint Setup:**
   - Review sprint goal and tasks
   - Ensure definition of done is clear
   - Setup tracking (simple kanban: To Do / In Progress / Done)

2. **Durante o Sprint:**
   - Implementar tarefas sequencialmente
   - Commit frequently com mensagens claras
   - Testar continuamente (não deixar testes pro final)
   - Documentar decisões importantes

3. **End of Sprint:**
   - Review: O que foi entregue vs. planejado?
   - Retrospective: O que funcionou? O que melhorar?
   - Demo: Validar funcionalidade com usuário (mesmo que você mesmo)
   - Update roadmap se necessário

**5.2 Validation Checkpoints**

At end of each phase:

**Fase 1 Checkpoint:**
- [ ] MVP deployed e acessível
- [ ] Happy path funciona end-to-end
- [ ] 5-10 usuários testaram
- [ ] Feedback coletado e documentado
- [ ] Decisão: Prosseguir para Fase 2? Pivotar? Iterar mais no MVP?

**Fase 2 Checkpoint:**
- [ ] Features priorizadas implementadas
- [ ] Métricas de engajamento sendo trackeadas
- [ ] Retenção semanal > 40%
- [ ] Performance aceitável (< 3s load time)
- [ ] Decisão: Escalar para Fase 3? Focar em retention?

**Fase 3 Checkpoint:**
- [ ] Growth loops implementados
- [ ] Processos automatizados
- [ ] Documentação completa
- [ ] Testes cobrindo fluxos principais
- [ ] Decisão: Manutenção? Novas features? Pivot?

**5.3 Iteration Protocol**

When issues arise or validation fails:

1. **Diagnose:** O que não funcionou? Por quê?
2. **Repriorize:** Ajustar backlog baseado em aprendizados
3. **Adapt:** Update roadmap, OKRs se necessário
4. **Iterate:** Implementar correções antes de prosseguir

**Refer to:**
- `references/agile-solo-dev.md` for execution best practices
- `references/execution-frameworks.md` for checkpoint templates

**5.4 Continuous Assistance**

Durante execução, Claude deve:
- Implementar código seguindo arquitetura definida
- Sugerir melhorias quando identificar problemas
- Alertar quando scope creep acontecer
- Ajudar a manter foco nos OKRs e sprint goals
- Facilitar retrospectives e ajustes de roadmap

**Output:**
- Projeto implementado fase por fase
- Validação em checkpoints
- Iteração baseada em feedback
- Documentação mantida atualizada

## Best Practices

### For Users

**Do's:**
- Seja honesto sobre seu nível técnico e constraints
- Valide com usuários reais o quanto antes
- Foque no MVP - resista ao scope creep
- Celebre pequenas vitórias (cada sprint completado)
- Documente decisões importantes

**Don'ts:**
- Não pule a fase de validação
- Não adicione features sem priorização (ICE/RICE)
- Não gaste muito tempo em polish antes da validação
- Não ignore métricas - track desde o dia 1
- Não tenha medo de pivotar se validação falhar

### For Claude

**Do's:**
- SEMPRE coletar contexto completo em Step 1
- Usar frameworks estabelecidos, não inventar
- Ser específico e actionable em todas recomendações
- Quebrar projetos grandes em fases realistas
- Validar compreensão antes de prosseguir para próximo step
- Manter documentação atualizada durante execução
- Alertar sobre scope creep ou riscos

**Don'ts:**
- Não pular steps do workflow
- Não dar soluções genéricas sem contexto
- Não recomendar big-bang launches
- Não adicionar complexidade desnecessária
- Não esquecer de definir métricas de sucesso
- Não proceder para código antes de ter PRD + arquitetura

## Resources

### references/
Detailed framework documentation loaded as needed:

- **idea-validation.md** - Lean Startup, Mom Test, Jobs-to-be-Done frameworks
- **prd-architecture.md** - PRD templates, fullstack architecture patterns, tech stack decisions
- **project-breakdown.md** - AARRR (Pirate Metrics), Stage-Based Development, ICE/RICE prioritization
- **agile-solo-dev.md** - Sprint planning, time management, batch creation for solo developers
- **execution-frameworks.md** - OKRs, implementation roadmaps, checkpoint templates, metrics tracking

### assets/
Ready-to-use templates for each project:

- **prd-template.md** - Complete PRD structure to copy and fill
- **architecture-doc-template.md** - Technical architecture documentation template
- **okr-project-template.md** - OKR template with examples for different project stages
- **weekly-sprint-template.md** - Sprint planning and retrospective template

## Examples

### Example 1: Todo App with AI Features

**User Request:** "Quero criar um app de to-do list com features de IA que sugere priorização"

**Step 1 - Context:**
- Fullstack web app (React + Node + PostgreSQL)
- Usuário: desenvolvedores/product managers
- Diferencial: IA sugere priorização baseada em urgência/importância
- Iniciante em IA, intermediário em web dev
- 4-6 semanas para MVP
- Validar com 5 amigos PMs

**Step 2 - Validation:**
- JTBD: Quando PM tem muitas tarefas e não sabe por onde começar
- Aha moment: IA sugere ordem de execução que faz sentido
- MVP: To-do CRUD + AI prioritization + visualização de prioridades
- Não fazer: time tracking, teams, integrations (v2)

**Step 3 - Planning:**
- PRD com North Star: "Tarefas completadas de alta prioridade por semana"
- Architecture: React frontend, Node API, PostgreSQL, OpenAI API
- Prioritização ICE das features

**Step 4 - Roadmap:**
```
Fase 1 (Semanas 1-2): MVP
  Sprint 1: Setup + CRUD básico de tarefas
  Sprint 2: Integração OpenAI + algoritmo de priorização

Fase 2 (Semanas 3-4): Polish + Secondary Features
  Sprint 3: UI/UX melhorado, filtros, categorias
  Sprint 4: Export, notificações, analytics básico

Fase 3 (Semanas 5-6): Growth
  Sprint 5: Onboarding, templates, sharing
  Sprint 6: Feedback loop, otimização IA
```

**Step 5 - Execution:**
- Implementar Sprint 1, validar CRUD funciona
- Implementar Sprint 2, testar com 5 PMs
- Checkpoint Fase 1: 4/5 PMs usaram toda semana → Prosseguir
- Continue fase 2...

### Example 2: SaaS Analytics Dashboard

**User Request:** "Preciso de um dashboard para analisar métricas de produto SaaS"

**Step 1 - Context:**
- Web app (Next.js + Python backend + BigQuery)
- Usuário: PMs de produtos SaaS
- Diferencial: insights automáticos, não só gráficos
- Avançado em frontend, iniciante em data
- 8-12 semanas para produto usável
- Validar com 10 PMs da rede

**Step 2 - Validation:**
- JTBD: Quando PM precisa entender saúde do produto rapidamente
- Aha moment: Ver insights acionáveis sem precisar fazer queries
- MVP: Conectar data source + 5 dashboards essenciais + 1 insight automatizado
- Não fazer: alertas customizados, ML avançado, white-label (v2+)

**Step 3 - Planning:**
- PRD com NSM: "Decisões baseadas em data tomadas por semana"
- Architecture: Next.js SSR, FastAPI backend, BigQuery connector, Chart.js
- Prioritização RICE dos dashboards (Acquisition, Activation, Retention, Revenue, Referral)

**Step 4 - Roadmap:**
```
Fase 1 (Semanas 1-4): Foundation
  Sprint 1-2: Data connectors (BigQuery, Postgres)
  Sprint 3-4: Primeiros 3 dashboards (Acquisition, Activation, Retention)

Fase 2 (Semanas 5-8): Core Product
  Sprint 5-6: Dashboards restantes + drill-downs
  Sprint 7-8: Primeiro insight automático (churn risk detection)

Fase 3 (Semanas 9-12): Growth & Polish
  Sprint 9-10: Onboarding, templates de dashboards
  Sprint 11-12: Performance optimization, caching, real-time updates
```

**Step 5 - Execution:**
- Implementar conectores, validar com dados reais
- Dashboard de Acquisition, testar com 3 PMs
- Checkpoint Fase 1: Dashboards úteis? Dados corretos? → Ajustar queries baseado em feedback
- Continue...

## Conclusion

This skill provides comprehensive structure for transforming app ideas into professionally executed projects. By following the 5-step workflow and leveraging the frameworks in references, users can build fullstack web apps with confidence, avoiding common pitfalls like scope creep, analysis paralysis, and lack of validation.

The phased approach ensures continuous progress with frequent validation, making it suitable for solo developers and small teams working on complex projects.
