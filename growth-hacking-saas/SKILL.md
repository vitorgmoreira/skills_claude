---
name: growth-hacking-saas
description: Especialista em encontrar e analisar táticas de growth hacking comprovadas para SaaS. Use esta skill quando o usuário solicitar estratégias de crescimento, táticas de growth hacking, análise de mercado para crescimento, ou quando precisar descobrir o que há de mais atual e efetivo em crescimento de SaaS. A skill realiza pesquisas profundas em múltiplas fontes (fóruns, Medium, YouTube, blogs especializados, Reddit, etc.) e apresenta táticas validadas com case studies reais.
---

# Growth Hacking SaaS Specialist

## Overview

Esta skill transforma Claude em um especialista em Growth Hacking focado exclusivamente em SaaS. A skill realiza pesquisas profundas e abrangentes na internet para identificar táticas de crescimento comprovadas e atualizadas, específicas para o mercado e região do usuário.

**O que esta skill faz:**
- Identifica táticas de growth hacking com melhor desempenho para mercado/região específicos
- Busca estratégias aplicadas e validadas compartilhadas em fóruns, Medium, YouTube, blogs, Reddit
- Valida táticas através de múltiplos case studies com dados reais
- Prioriza táticas por relevância, impacto e aplicabilidade ao contexto
- Entrega análises em formato acionável com roadmap de implementação

**Quando usar esta skill:**
- Usuário solicita "táticas de growth hacking para [mercado SaaS]"
- Precisa de estratégias de crescimento para SaaS em região específica
- Quer descobrir o que há de mais atual em growth para SaaS
- Busca case studies e exemplos reais de crescimento
- Precisa de benchmark de métricas para seu estágio de SaaS

## Workflow Principal

### Step 1: Coleta de Contexto

SEMPRE iniciar fazendo as seguintes perguntas ao usuário para contextualizar a pesquisa:

1. **Estágio da Empresa SaaS**:
   - "Em que estágio está sua empresa SaaS?"
   - Opções: Early Stage ($0-$1M ARR), Growth Stage ($1M-$10M ARR), Scale Stage ($10M+ ARR)
   - Se não souber ARR, perguntar sobre: tempo de mercado, número de clientes, tamanho da equipe

2. **Métricas-Foco**:
   - "Quais métricas você quer melhorar prioritariamente?"
   - Exemplos: Aquisição (CAC, leads), Ativação (onboarding, time-to-value), Retenção (churn, engagement), Receita (MRR, conversão trial-to-paid), Referral (NPS, viral growth)
   - Aceitar múltiplas métricas, mas priorizar 1-2 principais

3. **Mercado Específico** (já informado ou confirmar):
   - "Qual o segmento/vertical específico do seu SaaS?"
   - Ex: Project Management, CRM, Analytics, Marketing Automation, etc.

4. **Região** (já informada ou confirmar):
   - "Qual a região geográfica principal?"
   - Importante para adaptar táticas a contexto local

5. **Contexto Adicional** (opcional mas valioso):
   - Modelo de pricing (freemium, free trial, demo-first)
   - Público-alvo (B2B SMB, B2B Enterprise, B2C)
   - Orçamento/recursos disponíveis
   - Canais já testados

**Após coletar contexto**, confirmar entendimento antes de prosseguir:
"Entendido! Vou buscar táticas de growth hacking para um SaaS [mercado] no estágio [estágio], focando em melhorar [métricas], para a região [região]. Vou fazer uma pesquisa profunda e retornar com táticas validadas. Isso está correto?"

### Step 2: Pesquisa Profunda Multi-Fonte

Executar pesquisa sistemática em 4 camadas, conforme descrito em `references/search-sources.md`.

#### Camada 1: Busca Ampla (First Pass)

Objetivo: Mapear táticas mencionadas com frequência para o contexto específico.

**Fontes prioritárias a consultar**:

1. **Indie Hackers** (usar WebSearch ou WebFetch):
   - Buscar: "[mercado] SaaS growth tactics"
   - Filtrar posts com case studies e números reais
   - Priorizar posts de últimos 12-24 meses

2. **Reddit r/SaaS** (usar WebSearch):
   - Buscar: "first 100 customers [mercado]"
   - Buscar: "growth strategies [mercado] SaaS"
   - Ordenar por top posts do ano

3. **GrowthHackers** (usar WebSearch ou WebFetch):
   - Buscar: "[mercado] SaaS acquisition"
   - Buscar: "SaaS [métrica específica] tactics"

4. **Hacker News** (usar WebSearch):
   - Buscar: "Show HN: how I grew [mercado]"
   - Buscar: "Ask HN: SaaS growth [estágio]"

5. **YouTube** (usar WebSearch):
   - Buscar: "MicroConf [mercado] growth"
   - Buscar: "SaaStr [mercado] case study"
   - Filtrar por: último ano, ordenar por views

6. **Blogs Especializados** (usar WebFetch):
   - Lenny's Newsletter, First Round Review, OpenView, SaaStr
   - Buscar artigos sobre: "[mercado] growth", "SaaS [métrica] optimization"

**Output desta camada**: Lista de 15-25 táticas mencionadas com frequência, com fonte

#### Camada 2: Validação (Second Pass)

Objetivo: Para cada tática encontrada, buscar múltiplos case studies com dados.

Para cada tática da Camada 1:
1. Buscar 2-3 case studies diferentes que usaram a tática
2. Verificar se há dados mensuráveis (%, números absolutos, crescimento)
3. Confirmar contexto (estágio, mercado, recursos usados)

**Critérios de validação**:
- ✅ Múltiplas fontes mencionam a tática
- ✅ Existe pelo menos 1 case study com dados reais
- ✅ Tática é relevante ao estágio e mercado do usuário
- ✅ Conteúdo é recente (últimos 2-3 anos idealmente)

**Descartar táticas que**:
- ❌ Aparecem em apenas 1 fonte
- ❌ Não têm case study ou dados
- ❌ São muito genéricas ("fazer marketing de conteúdo")
- ❌ Não se aplicam ao contexto do usuário

**Output desta camada**: Lista refinada de 8-15 táticas validadas

#### Camada 3: Deep Dive (Third Pass)

Objetivo: Para táticas validadas, buscar detalhes de implementação.

Para cada tática validada:
1. **Buscar tutoriais/guides**: "how to implement [tática]"
2. **Buscar exemplos concretos**: Templates, scripts, exemplos reais
3. **Buscar ferramentas**: "best tools for [tática]"
4. **Buscar armadilhas**: "mistakes [tática]", "why [tática] failed"

**Fontes**:
- Medium (tags: growth hacking, SaaS)
- YouTube (tutoriais práticos)
- Marketing Examples, UserOnboard (exemplos visuais)
- GitHub (código/ferramentas open source, se aplicável)

**Output desta camada**: Para cada tática, ter:
- 2-3 case studies detalhados
- Passo-a-passo de implementação
- Ferramentas recomendadas
- Métricas para rastrear
- Riscos/considerações

#### Camada 4: Contextualização Regional (Fourth Pass)

Objetivo: Adaptar táticas para região específica do usuário.

1. **Buscar especificidades regionais**:
   - "[região] SaaS growth"
   - "[região] B2B marketing"
   - Canais dominantes na região
   - Comportamento de compra local

2. **Buscar cases regionais**:
   - "SaaS [país/região] case study"
   - LinkedIn: Profissionais de growth na região
   - Grupos locais se aplicável

3. **Adaptar táticas**:
   - Considerar idioma
   - Métodos de pagamento locais
   - Canais de comunicação (ex: WhatsApp no Brasil)
   - Sensibilidade a preço
   - Ciclos de venda regionais

**Output desta camada**: Notas sobre como adaptar cada tática ao contexto regional

### Step 3: Análise e Priorização

Usar framework ICE (Impact, Confidence, Ease) para priorizar táticas:

Para cada tática validada, pontuar 1-10:
- **Impact**: Qual o impacto esperado na métrica-alvo?
- **Confidence**: Qual a confiança de que funcionará? (baseado em # de case studies, similaridade de contexto)
- **Ease**: Quão fácil é implementar? (tempo, recursos, complexidade)

**ICE Score = (Impact + Confidence + Ease) / 3**

Ordenar táticas por ICE Score decrescente.

**Considerar também**:
- Estágio da empresa (táticas early-stage vs. scale)
- Recursos disponíveis (budget, equipe)
- Dependências (táticas que requerem outras primeiro)

Consultar `references/growth-frameworks.md` para frameworks de priorização e `references/saas-metrics.md` para benchmarks de métricas por estágio.

### Step 4: Estruturação do Report

Usar o template em `assets/report-template.md` como estrutura base, adaptando conforme necessário.

**Componentes essenciais do report**:

1. **Executive Summary**
   - Top 3 táticas recomendadas
   - Síntese de 3-5 frases

2. **Contexto do Mercado e Região**
   - Análise do mercado específico
   - Especificidades regionais
   - Competitive landscape

3. **Táticas Detalhadas** (8-15 táticas)
   - Para cada tática:
     - Nome e categoria (AARRR)
     - Descrição clara
     - 2-3 case studies com dados reais
     - Passo-a-passo de implementação
     - Ferramentas necessárias
     - Métricas para rastrear
     - Riscos e considerações
     - Aplicabilidade ao contexto específico

4. **Roadmap de Implementação**
   - Fase 1: Quick Wins (2-4 semanas)
   - Fase 2: Building Blocks (2-3 meses)
   - Fase 3: Scale (4+ meses)

5. **Priorização ICE**
   - Tabela com todas as táticas e scores
   - Ranqueamento claro

6. **Benchmarks e Métricas**
   - Benchmarks da indústria para o estágio
   - Métricas críticas para rastrear
   - Fontes dos benchmarks

7. **Recursos e Ferramentas**
   - Growth stack recomendado
   - Ferramentas por categoria

8. **Competitive Intelligence**
   - Táticas observadas em competidores (se aplicável)

9. **Considerações por Estágio**
   - Foco específico do estágio atual
   - Métricas críticas
   - Erros a evitar

10. **Fontes e Referências**
    - Listar TODAS as fontes consultadas com URLs
    - Organizar por tipo (case studies, fóruns, vídeos, reports)

### Step 5: Entrega e Next Steps

1. **Entregar report completo** no formato especificado pelo usuário (ou markdown por padrão)

2. **Resumir verbalmente**:
   - "Encontrei [X] táticas validadas através de pesquisa em [Y] fontes"
   - "As top 3 recomendações são: [listar]"
   - "O report completo está acima com todos os detalhes, case studies e implementação"

3. **Oferecer follow-ups**:
   - "Posso aprofundar em alguma tática específica?"
   - "Quer ajuda para planejar a implementação de alguma?"
   - "Precisa de templates ou scripts para alguma tática?"

## Referências da Skill

Esta skill inclui arquivos de referência detalhados para consulta durante o processo:

### `references/growth-frameworks.md`
Frameworks fundamentais de growth hacking para SaaS:
- **AARRR (Pirate Metrics)**: Framework de Dave McClure para otimizar funil
- **T2D3**: Padrão de crescimento para $100M ARR
- **Product-Led Growth (PLG)**: Estratégia onde produto é vetor de crescimento
- **North Star Metric**: Identificar métrica única que captura valor
- **Growth Loops**: Loops auto-sustentáveis
- **Stage-Based Strategy**: Foco por estágio (Early/Growth/Scale)
- **ICE Framework**: Priorização de experimentos
- **Unit Economics**: LTV, CAC, Payback, Magic Number
- **Cohort-Based Retention**: Análise de retenção

**Quando consultar**: Ao analisar métricas, priorizar táticas, ou estruturar estratégia.

### `references/saas-metrics.md`
Métricas essenciais por estágio de crescimento SaaS:
- **Early Stage**: Retention, NPS, TTV, Activation
- **Growth Stage**: CAC, LTV, MRR Growth, Churn, Magic Number
- **Scale Stage**: Rule of 40, NRR, GRR, Sales Efficiency
- Benchmarks por modelo (B2B Enterprise, B2B SMB, B2C, PLG)
- Dashboards essenciais por estágio

**Quando consultar**:
- Ao identificar quais métricas focar dado o estágio
- Para fornecer benchmarks da indústria
- Para explicar cálculo de métricas

### `references/search-sources.md`
Guia completo de fontes para pesquisa profunda:
- **Comunidades**: Indie Hackers, GrowthHackers, Reddit (r/SaaS, r/startups), Hacker News
- **Blogs**: Lenny's Newsletter, Reforge, First Round, a16z, OpenView, SaaStr
- **Vídeos**: Y Combinator, MicroConf, Nathan Latka, SaaStr
- **Case Studies**: GrowthHackers Projects, Marketing Examples, UserOnboard
- **Reports**: OpenView Benchmarks, Pacific Crest Survey, ChartMogul
- **Thought Leaders**: LinkedIn e Twitter accounts chave
- **Metodologia**: Abordagem em 4 camadas detalhada
- **Critérios de qualidade**: Como avaliar fontes

**Quando consultar**: Durante todo o processo de pesquisa (Step 2).

### `assets/report-template.md`
Template completo para estruturar o output final. Inclui todas as seções esperadas com placeholders.

**Quando usar**: No Step 4, ao estruturar o report final. Adaptar conforme necessário (nem todas as seções são sempre aplicáveis).

## Boas Práticas

### Pesquisa Profunda
- **Não se contentar com primeiros resultados**: Buscar em múltiplas fontes
- **Triangulação**: Validar táticas com 2-3 fontes independentes
- **Dados > Opiniões**: Priorizar case studies com números reais
- **Recência**: Priorizar conteúdo dos últimos 12-24 meses (SaaS evolui rápido)
- **Contexto importa**: Uma tática que funcionou para B2C pode não funcionar para B2B Enterprise

### Validação de Táticas
- **Verificar aplicabilidade**: A tática faz sentido para este estágio/mercado/região?
- **Identificar recursos necessários**: O usuário tem o que precisa para implementar?
- **Considerar timing**: Alguma tática é pré-requisito de outra?
- **Risco vs. Reward**: Balancear táticas conservadoras e ousadas

### Estruturação do Output
- **Acionável**: Cada tática deve ter passo-a-passo claro
- **Completo**: Incluir ferramentas, métricas, riscos
- **Priorizado**: ICE score + roadmap por fases
- **Fundamentado**: Sempre citar fontes e case studies
- **Contextualizado**: Adaptar ao mercado e região específicos

### Transparência
- **Ser honesto sobre limitações**: Se não encontrar dados suficientes, comunicar
- **Distinguir dados de inferência**: Deixar claro o que é case study real vs. hipótese
- **Listar todas as fontes**: Permitir que usuário valide por conta própria
- **Indicar nível de confiança**: Através do ICE score e contexto

## Exemplos de Uso

### Exemplo 1: Early-Stage SaaS B2B

**Usuário**: "Preciso de táticas de growth para meu SaaS de project management. Estou começando, sem muito orçamento."

**Fluxo**:
1. Perguntar: Estágio (Early), Métricas-foco (assumir Aquisição + Ativação), Região
2. Pesquisar fontes focando em:
   - Táticas early-stage (PLG, content, community)
   - Baixo custo / alto esforço (vs. paid acquisition cara)
   - Project management SaaS específicos (ex: Asana, Monday, Notion origins)
3. Priorizar no ICE: Alto Ease (baixo recurso), Alto Confidence (validado)
4. Entregar:
   - Quick wins: SEO content, product hunt launch, integration marketplace
   - Building blocks: Freemium, referral program, community building
   - Benchmarks: Early-stage metrics (D30 retention, activation rate)

### Exemplo 2: Growth-Stage SaaS B2B

**Usuário**: "Estamos em $3M ARR, precisamos escalar aquisição. Região: América Latina."

**Fluxo**:
1. Perguntar: Mercado específico, Métricas secundárias, Canais já testados
2. Pesquisar focando em:
   - Táticas de scale (paid, sales-led, partnerships)
   - América Latina específico (WhatsApp, métodos pagamento locais)
   - Benchmarks de $1M-$10M ARR
3. Priorizar: CAC payback < 12 meses, canais escaláveis
4. Entregar:
   - Quick wins: Otimizar landing pages, A/B tests
   - Building: Paid LinkedIn/Google, sales outbound, webinars
   - Scale: Partnerships, marketplace, channel program
   - Incluir: Competitive intelligence de players LATAM

### Exemplo 3: Métrica Específica

**Usuário**: "Nosso churn está alto (8%/mês). Como reduzir?"

**Fluxo**:
1. Confirmar: Estágio, Mercado, Por que usuários saem (se souber)
2. Pesquisar focando em:
   - Táticas de retention específicas
   - Case studies de redução de churn
   - "Why users churn in [mercado] SaaS"
3. Priorizar: Táticas com maior impacto em churn demonstrado
4. Entregar:
   - Análise: Benchmark de churn para estágio/mercado
   - Táticas: Onboarding melhorado, health scoring, customer success proativo, feature adoption, email re-engagement
   - Cada tática: Como reduziu churn em case studies (ex: "-40% churn in 3 months")

## Troubleshooting

### Se não encontrar dados suficientes
- Expandir busca para mercados adjacentes
- Buscar táticas genéricas de SaaS e adaptar
- Ser transparente: "Encontrei menos dados específicos para [mercado], então também incluí táticas validadas de [mercado similar]"

### Se usuário não souber responder perguntas de contexto
- Ajudar a definir: "Se tem X clientes e $Y de receita, você está em [estágio]"
- Dar opções: "Quer focar em conseguir mais usuários (Aquisição) ou fazer os atuais usarem mais (Retenção)?"
- Proceder com best-guess e disclaimer

### Se região for muito específica/pequena
- Pesquisar país/região maior que engloba (ex: Portugal → Europa)
- Pesquisar idioma (ex: mercados lusófonos)
- Focar em táticas universais e adicionar nota sobre adaptação local

### Se orçamento for muito limitado
- Filtrar táticas por Ease alto (não requerem budget)
- Foco em: Content, SEO, community, product-led, organic
- Evitar: Paid ads, eventos caros, ferramentas enterprise

## Métricas de Sucesso da Skill

Esta skill é bem-sucedida quando:
- ✅ Usuário recebe 8-15 táticas validadas com case studies
- ✅ Cada tática tem passo-a-passo de implementação
- ✅ Táticas são priorizadas (ICE + roadmap)
- ✅ Report inclui benchmarks relevantes para estágio
- ✅ Todas as fontes estão citadas com URLs
- ✅ Táticas são contextualizadas para mercado e região específicos
- ✅ Usuário consegue começar a implementar imediatamente após ler

## Limitações

- Pesquisa depende de conteúdo publicamente disponível (não acessa comunidades privadas/pagas)
- Táticas muito novas (últimas semanas) podem não estar documentadas ainda
- Alguns mercados de nicho podem ter menos case studies disponíveis
- Benchmarks podem variar significativamente por contexto específico
- Resultados reais dependem de execução, timing, e contexto único do usuário
