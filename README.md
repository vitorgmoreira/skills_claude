# Claude Skills Collection

Coleção pessoal de skills customizadas para Claude Desktop.

## 📚 Skills Disponíveis

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
├── b2b-saas-startup-mentor.zip          # Skill empacotada (pronta para instalar)
└── b2b-saas-startup-mentor/             # Código fonte da skill
    ├── SKILL.md                         # Configuração principal
    ├── references/                      # 8 guias detalhados
    │   ├── product-market-fit.md
    │   ├── metrics-kpis.md
    │   ├── gtm-sales.md
    │   ├── pricing-monetization.md
    │   ├── fundraising-brazil.md
    │   ├── growth-strategies.md
    │   ├── okrs-planning.md
    │   └── brazil-market-context.md
    └── assets/                          # 4 templates prontos
        ├── pitch-deck-template.md
        ├── okr-template.md
        ├── one-pager-template.md
        └── metrics-dashboard-template.md
```
