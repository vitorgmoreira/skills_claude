# Comunicação e Transparência em Equity

Como explicar equity para colaboradores, criar transparência e evitar mal-entendidos.

---

## 🎯 O Problema: Colaboradores Não Entendem Equity

**Realidade**: 80%+ dos colaboradores com equity não entendem completamente:
- Quanto equity vale hoje
- O que é diluição
- Quando podem vender (liquidez)
- Diferença entre stock options e phantom shares
- Impostos que vão pagar

**Consequência**: Frustração, sensação de "enganação", saídas prematuras

---

## 📚 Educação é Crítica

### Onboarding de Equity (Primeira Vez)

**Quando oferecer equity** (offer letter), incluir:

**1. Explicação Básica**:
```
"Você receberá 10.000 stock options com strike price de R$1,00.

O que isso significa:
- Você terá o DIREITO de comprar 10.000 ações por R$1,00 cada
- Hoje, cada ação vale R$10,00 (valuation atual)
- Se você exercer hoje, pagaria R$10.000 e receberia ações que valem R$100.000

Vesting:
- Você "ganha" essas options ao longo de 4 anos
- Cliff de 1 ano: se sair antes de 1 ano, perde tudo
- Após 1 ano: 25% veste, depois 1/48 avos por mês

Liquidez:
- Você só pode vender essas ações em um "exit" (M&A, IPO)
- Pode levar 5-10 anos para ter liquidez
- Não é dinheiro hoje, é potencial de ganho no futuro
```

**2. Cenários de Exit**:
```
Cenário Conservador (empresa vale R$100M no exit):
- Suas 10.000 ações = 0.1% da empresa
- Valor: R$100k
- Menos strike (R$10k) e impostos (~R$20k)
- Líquido: ~R$70k

Cenário Base (R$500M):
- Valor: R$500k
- Líquido: ~R$400k

Cenário Otimista (R$1B - unicórnio):
- Valor: R$1M
- Líquido: ~R$800k

Cenário Realista:
- 50% das startups falham (equity = R$0)
- 30% têm exit pequeno (abaixo do investido)
- 15% têm exit médio (2-5x retorno)
- 5% têm exit grande (10x+ retorno)
```

**3. FAQ Antecipado**:
- "O que é vesting?"
- "Quando posso vender?"
- "O que acontece se a empresa não der exit?"
- "Quanto vou pagar de imposto?"

---

## 🔍 Transparência: Quanto Compartilhar?

### Opção 1: Transparência Total (Recomendado para Seed+)

**Compartilhar com todos colaboradores**:
- ✅ Valuation atual da empresa
- ✅ Cap table simplificado (% de cada stakeholder)
- ✅ Equity pool restante
- ✅ Histórico de diluição
- ✅ Plano de futuras rodadas

**Vantagens**:
- Confiança e engajamento
- Colaboradores entendem contexto
- Decisões melhores (todos sabem o "porquê")

**Exemplo (Buffer, Gitlab)**: Cap table 100% público

---

### Opção 2: Transparência Limitada

**Compartilhar apenas**:
- ✅ % de equity individual
- ✅ Valuation atual
- ❌ Cap table completo
- ❌ Equity de outros colaboradores

**Vantagens**:
- Menos comparação entre colaboradores
- Privacidade

---

### Opção 3: Opacidade (Não Recomendado)

**Não compartilhar quase nada**:
- ❌ Valuation
- ❌ Cap table
- ❌ Contexto de diluição

**Problema**: Gera desconfiança, especulação, frustração

**Quando é comum**: Pre-seed muito early (ainda validando)

---

## 💬 Comunicando Diluição

### O Que É Diluição?

**Definição**: Seu % da empresa diminui quando novos investidores entram

**Exemplo**:
```
Situação inicial:
- Você: 1% da empresa (10.000 ações de 1.000.000 total)
- Empresa vale: R$10M

Series A (investidor compra 20%):
- Total de ações aumenta para 1.250.000
- Você ainda tem 10.000 ações
- Seu %: 10.000 / 1.250.000 = 0.8%
- Diluição: De 1% para 0.8% (20% de diluição)

MAS:
- Valuation pós-money: R$50M
- Seu equity: 0.8% × R$50M = R$400k
- Antes era: 1% × R$10M = R$100k

Você foi diluído, mas seu equity VALEU MAIS (R$100k → R$400k)
```

---

### Como Comunicar

**Mensagem ao time após rodada**:
```
Subject: Series A Fechada - Update de Equity

Time,

Fechamos nossa Series A de R$20M com valuation pós-money de R$100M.

Impacto no seu equity:

1. Diluição:
   - Todos foram diluídos em ~20% (padrão em Series A)
   - Se você tinha 1%, agora tem 0.8%

2. Valor:
   - Apesar da diluição, seu equity VALEU MAIS
   - Valuation subiu 10x (R$10M → R$100M)
   - Seu equity: 0.8% × R$100M = R$800k (antes: R$100k)

3. Equity Pool:
   - Refresh do pool para 15% (para futuras contratações)
   - Esse refresh também dilui todos (incluindo founders)

Próximos passos:
- Usaremos R$20M para crescer time, produto, vendas
- Meta: Chegar em R$10M ARR em 18 meses
- Próxima rodada (Series B): Projetamos valuation de R$300-500M

Dúvidas? Estou disponível para 1:1.

[CEO Name]
```

---

## 🧮 Tools de Visualização

### Cap Table Tools

**Recomendados**:
1. **Carta** (mais usado globalmente)
   - Dashboard para colaboradores
   - Cenários de exit
   - Tracking automático de vesting

2. **Pulley** (startup-friendly)
   - Visualização clara
   - Onboarding de optionholders
   - Mais barato que Carta

3. **Capboard** (Brasil)
   - Focado em BR
   - Integração com contabilidade BR

---

### Equity Calculators

**Criar calculadora interna** para colaboradores:
```
Inputs:
- Número de options: [10.000]
- Strike price: [R$1,00]
- Valuation atual: [R$100M]
- % de equity: [0.1%]

Outputs:
Cenário exit R$500M:
- Valor bruto: R$500k
- Strike pago: R$10k
- IR (~23%): R$113k
- Líquido: ~R$377k
```

**Exemplo de ferramenta**: [Figura interativa no Notion/Confluence]

---

## 📅 Rituais de Comunicação

### Onboarding (Ao dar equity)

**Checklist**:
- [ ] Explicar o que é equity (options vs phantom vs RSU)
- [ ] Explicar vesting e cliff
- [ ] Cenários de exit (conservador, base, otimista)
- [ ] Mostrar cálculo de impostos
- [ ] Dar FAQ escrito
- [ ] Oferecer 1:1 para dúvidas

---

### Anual (Company All-Hands)

**Update de equity**:
- Valuation atual
- Diluição no ano (se teve rodada)
- Progresso rumo a exit (métricas chave)
- Recap de equity pool (quanto usado, quanto resta)

---

### Pós-Rodada (Dentro de 1 semana)

**Email + All-Hands**:
- Valuation pós-money
- Quanto foi investido
- Diluição %
- Impacto no equity individual (valor absoluto aumentou)
- Próximos passos da empresa

---

## ❓ FAQ Comum de Colaboradores

### "Quanto meu equity vale hoje?"

**Resposta**:
```
"Seu equity 'vale' X no papel (baseado no valuation da última rodada).

MAS: Esse valor é ilusório até ter liquidez (exit).

Cenários:
- Empresa falha: Vale R$0
- Exit pequeno: Vale menos que no papel
- Exit grande: Vale mais que no papel

Pense em equity como loteria high-probability:
- Não conte com esse dinheiro para despesas de curto prazo
- É upside de longo prazo (5-10 anos)
```

---

### "Quando posso vender?"

**Resposta**:
```
"Você poderá vender em um 'exit':
- M&A (empresa vendida)
- IPO (empresa abre capital)
- Mercado secundário (raro, Series B+)

Timeline típico:
- Startup leva 7-10 anos para exit (mediana)
- 50% das startups nunca tem exit

Paciência é crítica."
```

---

### "O que acontece se eu sair antes do exit?"

**Resposta**:
```
"Depende de quando você sair:

Antes do cliff (1 ano):
- Perde todo equity (0%)

Após cliff, mas antes de 4 anos:
- Mantém equity vestido até data de saída
- Perde equity não-vestido
- Tem 90 dias para EXERCER options (pagar strike price)

Após 4 anos (fully vested):
- Mantém tudo
- Tem 90 dias para exercer

Importante: Exercer custa dinheiro (strike price × quantity)
Ex: 10.000 options, strike R$1 = R$10k out-of-pocket"
```

---

### "Vou pagar quanto de imposto?"

**Resposta**:
```
"Impostos acontecem em 2 momentos:

1. Exercício (quando você compra as ações):
   - IR: Até 27,5% sobre (FMV - strike)
   - Exemplo: Ganho de R$90k → IR de ~R$24k

2. Venda (exit):
   - IR ganho de capital: 15-22,5% sobre lucro
   - Exemplo: Venda R$500k, comprou R$10k → IR ~R$74k

Total: ~20-30% do ganho líquido vai para impostos"
```

---

## ⚠️ Armadilhas de Comunicação

**Erro #1**: Prometer muito
```
Ruim: "Esse equity vai te fazer milionário!"
Bom: "Esse equity tem potencial de upside significativo, mas é risco alto"
```

**Erro #2**: Não explicar vesting
```
Problema: Pessoa acha que equity é dele 100% desde dia 1
Solução: Explicar cliff e vesting na offer letter
```

**Erro #3**: Comparar com outros
```
Ruim: "Você tem mais equity que João"
Bom: "Seu equity foi determinado baseado em role, seniority, timing"
```

**Erro #4**: Esconder diluição
```
Problema: Colaborador descobre que foi diluído, sente-se enganado
Solução: Comunicar diluição proativamente após cada rodada
```

---

## 🎯 Templates de Comunicação

Ver em `assets/`:
- `equity-offer-letter.md`: Carta de oferta com equity
- `equity-faq-collaborators.md`: FAQ completo para colaboradores
- `post-round-email-template.md`: Email pós-rodada explicando diluição

---

**Próximo guia**: [cap-table-management.md](cap-table-management.md)
