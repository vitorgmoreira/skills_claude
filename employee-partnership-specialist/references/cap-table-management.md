# Cap Table Management

Guia sobre gestão de cap table, tracking de vesting, diluição e ferramentas.

---

## 📊 O Que É Cap Table?

**Capitalization Table** = Planilha que mostra ownership da empresa

**Informações incluídas**:
- Quem são os shareholders (fundadores, investidores, colaboradores)
- Quantas ações cada um possui
- % de ownership
- Tipo de ações (common, preferred, options)
- Vesting status

---

## 🏗️ Estrutura Básica

```
SHAREHOLDERS:
├─ Founders: 60% (com reverse vesting)
├─ Investors: 25% (Series A preferred stock)
├─ Equity Pool: 15%
    ├─ Options concedidas: 8%
    │   ├─ Vestidas: 4%
    │   └─ Não-vestidas: 4%
    └─ Options disponíveis: 7%
```

---

## 🔧 Ferramentas de Cap Table

**Carta** (mais usado):
- Dashboard para colaboradores
- Tracking automático de vesting
- Cenários de exit
- Custo: ~$2k-10k/ano

**Pulley** (startup-friendly):
- Mais barato que Carta
- Interface simples
- Custo: ~$500-2k/ano

**Capboard** (Brasil):
- Focado em startups BR
- Integração com contabilidade
- Custo: ~R$200-800/mês

**Planilha Excel/Google Sheets** (early-stage):
- Grátis
- Requer manutenção manual
- Template disponível em `assets/`

---

## 📋 Tracking de Vesting

**Informações a trackear**:
- Data de início do vesting (start date)
- Vesting schedule (4 anos, cliff 1 ano)
- Equity vestido até hoje (quantidade)
- Próximo vesting milestone

**Automação recomendada**: Software de cap table (Carta, Pulley)

---

## 📉 Diluição e Atualizações

**Após cada rodada**:
1. Atualizar valuation
2. Recalcular % de todos (com diluição)
3. Comunicar impacto para colaboradores
4. Refresh equity pool (se necessário)

**Exemplo de update pós-Series A**:
```
PRÉ-SERIES A:
- Founder: 70% (7M shares)
- Employee pool: 30% (3M shares)
- Total: 10M shares

PÓS-SERIES A (investidor compra 20%):
- Total shares: 12.5M (10M / 0.8)
- Founder: 7M / 12.5M = 56% (diluído de 70%)
- Employee pool: 3M / 12.5M = 24% (diluído de 30%)
- Investor: 2.5M / 12.5M = 20%
```

---

## ⚠️ Erros Comuns

**Erro #1**: Cap table desatualizado
- Problema: Decisões baseadas em dados errados
- Solução: Atualizar mensalmente

**Erro #2**: Não trackear vesting
- Problema: Confusão sobre quanto equity está vestido
- Solução: Usar software ou planilha automatizada

**Erro #3**: Esquecer de documentar concessões
- Problema: Disputa legal (colaborador diz que tem equity, empresa não acha)
- Solução: SEMPRE documentar em contrato assinado

---

**Templates**: Ver `cap-table-template-reference.md` em `assets/`
