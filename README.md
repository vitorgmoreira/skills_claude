# Claude Skills Collection

Coleção pessoal de skills customizadas para Claude Desktop.

## 📚 Skills Disponíveis

### Growth Hacking SaaS Specialist

Especialista em encontrar e analisar táticas de growth hacking comprovadas para SaaS através de pesquisas profundas na internet.

- **Descrição**: Transforma Claude em um especialista em Growth Hacking focado exclusivamente em SaaS, realizando pesquisas profundas em múltiplas fontes para identificar táticas validadas com case studies reais
- **Capacidades principais**:
  - Pesquisa profunda em 40+ fontes (Indie Hackers, Reddit, GrowthHackers, Hacker News, YouTube, Medium, blogs especializados)
  - Validação com múltiplos case studies e dados mensuráveis
  - Priorização com framework ICE (Impact, Confidence, Ease)
  - Contextualização para mercado e região específicos
  - Reports acionáveis com roadmap de implementação
  - Benchmarks da indústria por estágio de crescimento
- **Recursos inclusos**:
  - 3 guias completos de referência (Frameworks, Métricas, Fontes de Pesquisa)
  - Template profissional de report (12 seções)
  - Metodologia de pesquisa em 4 camadas
  - Benchmarks por estágio (Early/Growth/Scale)
- **Download**: [`growth-hacking-saas.zip`](growth-hacking-saas.zip)

**Exemplos de uso:**
```
"Preciso de táticas de growth para meu SaaS de CRM. Estamos em $2M ARR, região Brasil."
"Nosso churn está em 8%/mês. Quais táticas funcionam para reduzir?"
"Quero escalar aquisição para SaaS de project management em early stage."
"Me mostre estratégias validadas de growth para SaaS B2B na América Latina."
```

---

### B2B SaaS Startup Mentor

Mentor especializado em aceleração de startups B2B SaaS brasileiras em estágio seed/pre-seed.

- **Descrição**: Transforma Claude em um mentor expert de startups, similar aos mentores de aceleradoras como Y Combinator e Endeavor
- **Áreas cobertas**:
  - Product-Market Fit e validação
  - Go-to-Market e estratégias de vendas
  - Métricas e KPIs (MRR, Churn, CAC, LTV, NRR, etc.)
  - Fundraising e pitch para investidores brasileiros
  - Pricing e monetização
  - Growth e estratégias de crescimento
  - OKRs e planejamento estratégico
  - Contexto específico do mercado brasileiro
- **Recursos inclusos**:
  - 8 guias detalhados de referência
  - 4 templates prontos (Pitch Deck, OKRs, One-Pager, Dashboard de Métricas)
- **Download**: [`b2b-saas-startup-mentor.zip`](b2b-saas-startup-mentor.zip)

**Exemplos de uso:**
```
"Analise minhas métricas: tenho R$100k MRR, 30 clientes, 3% churn mensal. Estou pronto para Series A?"
"Me ajude a criar OKRs para o próximo trimestre. Estamos em seed stage."
"Revise meu pitch deck antes de apresentar para investidores."
"Devo focar em SMB ou Enterprise? Meu ACV atual é R$5k/ano."
```

---

### LinkedIn Content Creator

Criador expert de conteúdo para LinkedIn com técnicas avançadas de storytelling e otimização algorítmica.

- **Descrição**: Transforma Claude em um escritor profissional de LinkedIn que cria posts altamente engajadores, prontos para publicar
- **Capacidades principais**:
  - Criação de posts completos do zero
  - Adaptação de conteúdo de outras fontes (artigos, reuniões, experiências)
  - Geração de ideias de conteúdo
  - Otimização para algoritmo do LinkedIn
  - Estruturação de carousels
  - Aplicação de técnicas de copywriting e storytelling
- **Recursos inclusos**:
  - 8 frameworks de conteúdo de alta performance
  - 7 tipos de hooks magnéticos
  - Técnicas de engajamento e triggers psicológicos
  - Templates de posts e carousels
- **Download**: [`linkedin-content-creator.zip`](linkedin-content-creator.zip)

**Exemplos de uso:**
```
"Escreva um post para LinkedIn sobre técnicas de produtividade para founders"
"Transforme este artigo em um post de LinkedIn: [artigo]"
"Acabei de ter um meeting onde aprendi X sobre pricing. Crie conteúdo disso"
"Me ajude a criar conteúdo para LinkedIn sobre minha startup"
```

---

## 🚀 Como Instalar

1. Baixe o arquivo `.zip` da skill desejada
2. Extraia o conteúdo para a pasta de skills do Claude Desktop:
   - **macOS/Linux**: `~/.claude/skills/`
   - **Windows**: `%USERPROFILE%\.claude\skills\`
3. Reinicie o Claude Desktop

## 💡 Como Usar

As skills são ativadas automaticamente quando você faz perguntas relacionadas ao domínio de especialidade delas. Você também pode invocar uma skill explicitamente mencionando-a na sua mensagem.

Cada skill inclui sua própria documentação com exemplos específicos de uso.

---

## 📁 Estrutura do Repositório

```
skills_claude/
├── README.md
│
├── growth-hacking-saas.zip              # Skill: Growth Hacking SaaS
└── growth-hacking-saas/
    ├── SKILL.md                         # 10.000+ palavras de instruções
    ├── references/                      # 3 guias completos
    │   ├── growth-frameworks.md         # AARRR, PLG, ICE, Unit Economics
    │   ├── saas-metrics.md              # Métricas por estágio + benchmarks
    │   └── search-sources.md            # 40+ fontes + metodologia
    └── assets/
        └── report-template.md           # Template com 12 seções
│
├── b2b-saas-startup-mentor.zip          # Skill: Mentoria de Startups
└── b2b-saas-startup-mentor/
    ├── SKILL.md
    ├── references/                      # 8 guias detalhados
    │   ├── product-market-fit.md
    │   ├── metrics-kpis.md
    │   ├── gtm-sales.md
    │   ├── pricing-monetization.md
    │   ├── fundraising-brazil.md
    │   ├── growth-strategies.md
    │   ├── okrs-planning.md
    │   └── brazil-market-context.md
    └── assets/                          # 4 templates
        ├── pitch-deck-template.md
        ├── okr-template.md
        ├── one-pager-template.md
        └── metrics-dashboard-template.md
│
├── linkedin-content-creator.zip         # Skill: Criador de Conteúdo LinkedIn
└── linkedin-content-creator/
    ├── SKILL.md
    ├── references/
    │   ├── engagement-techniques.md
    │   └── content-frameworks.md
    └── assets/
        ├── post-template.txt
        └── carousel-template.txt
```
