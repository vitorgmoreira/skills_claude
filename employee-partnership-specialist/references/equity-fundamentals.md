# Fundamentos de Equity para Colaboradores

Guia completo sobre equity compensation para startups brasileiras: conceitos, tipos, quando implementar e benchmarks.

---

## 🎯 O Que É Equity Compensation

**Equity compensation** (ou "participação societária") é quando a empresa compartilha ownership (propriedade) com colaboradores, alinhando interesses e criando incentivos de longo prazo.

### Por Que Dar Equity?

**1. Atrair Talentos**:
- Startups geralmente não podem pagar salários competitivos com grandes empresas
- Equity compensa diferença salarial com potencial de upside exponencial
- "Trade-off": salário menor hoje por equity que pode valer muito no futuro

**2. Retenção**:
- Vesting de 4 anos com cliff de 1 ano mantém pessoas por período longo
- Colaborador que sai antes do cliff perde todo equity
- Após cliff, incentivo continua (quanto mais fica, mais equity acumula)

**3. Alinhamento de Incentivos**:
- Colaborador com equity pensa como dono (não apenas empregado)
- Sucesso da empresa = sucesso pessoal (wealth creation)
- Reduz conflito principal-agente

**4. Cultura de Ownership**:
- Todos são "donos" da empresa
- Decisões de longo prazo (não apenas curto prazo)
- Colaboração cross-functional natural

---

## 📊 Tipos de Equity Compensation

### 1. Stock Options (Opções de Ações)

**O que é**:
- Direito de COMPRAR ações da empresa a um preço fixo (strike price) no futuro
- Não é ownership imediato (é direito de compra)

**Como funciona**:
```
Exemplo:
1. Empresa te dá 10.000 stock options
2. Strike price: R$1,00 por ação
3. Vesting: 4 anos, cliff 1 ano

Após 1 ano (cliff):
- 2.500 options vestidas (25%)
- Você pode EXERCER (comprar) essas 2.500 ações por R$2.500
- Empresa vale R$10,00/ação (FMV)
- Você paga R$2.500, recebe ações que valem R$25.000
- Ganho no exercício: R$22.500

No exit (empresa vendida por R$50/ação):
- Suas 2.500 ações valem R$125.000
- Ganho total: R$125.000 - R$2.500 (o que você pagou) = R$122.500
```

**Requisitos no Brasil**:
- Empresa deve ser **Sociedade Anônima (SA)**
- LTDA **NÃO pode** ter stock options verdadeiras
- Aprovação em Assembleia Geral Extraordinária (AGE)

**Vantagens**:
- ✅ Ownership real da empresa
- ✅ Ganho ilimitado (quanto mais empresa vale, mais você ganha)
- ✅ Tratamento tributário pode ser mais favorável (ganho de capital)

**Desvantagens**:
- ❌ Colaborador precisa PAGAR para exercer (cash out-of-pocket)
- ❌ Sem liquidez até exit (IPO, M&A)
- ❌ Complexidade tributária

---

### 2. Phantom Shares (Ações Fantasma)

**O que é**:
- Direito de receber VALOR equivalente a ações (não ownership real)
- "Simula" equity sem dar ownership legal
- Também chamado: Shadow Stock, Synthetic Equity

**Como funciona**:
```
Exemplo:
1. Empresa te dá 10.000 phantom shares
2. Valor base: R$1,00 por share (valuation atual)
3. Vesting: 4 anos, cliff 1 ano

No exit (empresa vendida, valuation R$50/share):
- Suas 10.000 phantom shares "valem" R$500.000
- Valor base era R$10.000
- Empresa te paga R$490.000 em dinheiro (ou ações reais)
- Você NÃO precisa pagar nada (diferente de stock options)
```

**Requisitos no Brasil**:
- Funciona em **LTDA ou SA**
- Não precisa transformar empresa
- Contrato civil (não societário)

**Vantagens**:
- ✅ Funciona em LTDA (maioria das startups early-stage)
- ✅ Colaborador NÃO precisa pagar para "exercer"
- ✅ Mais simples de implementar
- ✅ Flexibilidade total nas regras

**Desvantagens**:
- ❌ Não é ownership real
- ❌ Tributação como bônus (IR 27.5% + INSS potencialmente)
- ❌ Empresa precisa ter caixa para pagar no exit
- ❌ Não funciona em IPO (só M&A ou distribuição de dividendos)

---

### 3. Restricted Stock Units (RSU)

**O que é**:
- Promessa de dar ações no futuro (após vesting)
- Comum em empresas maduras (BigTechs, pós-IPO)

**Como funciona**:
```
Exemplo:
1. Empresa te dá 1.000 RSUs
2. Vesting: 4 anos, cliff 1 ano

Após 1 ano (cliff):
- 250 RSUs viram 250 ações reais
- Você NÃO paga nada
- Ações são suas (ownership imediato)
- IR devido no vesting (como "renda")
```

**Quando usar**:
- Empresas pós-IPO (ações têm liquidez)
- Empresas maduras com liquidez

**Menos comum em startups BR** (mais comum em US BigTech)

---

### 4. Stock Appreciation Rights (SAR)

**O que é**:
- Similar a phantom shares, mas paga apenas a "valorização"
- Direito de receber diferença entre FMV atual e FMV na concessão

**Como funciona**:
```
Exemplo:
1. SARs concedidas quando empresa vale R$10M (R$1/share)
2. Você tem 10.000 SARs
3. Exit: empresa vale R$50M (R$5/share)
4. Você recebe: (R$5 - R$1) × 10.000 = R$40.000
```

**Menos comum no Brasil** (phantom shares são mais usadas)

---

## 🏢 Estrutura Societária: LTDA vs SA

### LTDA (Sociedade Limitada)

**Características**:
- Maioria das startups early-stage no Brasil
- Mais simples, menos burocracia
- Não pode ter stock options verdadeiras

**Equity Options**:
- ✅ Phantom Shares (mais comum)
- ✅ SARs
- ❌ Stock Options (NÃO permitido)

**Quando usar**:
- Pre-seed, early seed
- Ainda não levantou muito capital
- Quer simplicidade

---

### SA (Sociedade Anônima)

**Características**:
- Necessária para stock options reais
- Mais complexa, mais cara (R$30-80k para transformar)
- Exigida por investidores (geralmente Series A+)

**Equity Options**:
- ✅ Stock Options (principal motivo para virar SA)
- ✅ Phantom Shares
- ✅ RSUs
- ✅ SARs

**Quando transformar**:
- Series A ou quando investidor exigir
- Quer dar ownership real (não phantom)
- Planeja IPO no futuro

**Custo de transformação LTDA → SA**:
- Advogados: R$15-30k
- Contabilidade: R$5-10k
- Taxas/registro: R$10-15k
- **Total: R$30-80k**
- **Tempo: 2-4 meses**

---

## 💰 Equity Pool: Quanto Alocar?

### Benchmarks por Estágio

**Pre-Seed / Seed**:
```
Equity pool típico: 10-15%
- Suficiente para primeiras 10-20 contratações chave
- Reserva para C-level e early team
```

**Series A**:
```
Equity pool típico: 15-20%
- Refresh do pool (diluição na rodada)
- Crescimento de 20 para 50+ pessoas
- Inclui VP-level hires
```

**Series B+**:
```
Equity pool típico: 10-15% (refresh pós-diluição)
- Continua refresh a cada rodada
- Escala de 50 para 200+ pessoas
```

**Regra geral**:
- Pool deve durar **18-24 meses** de contratações
- Refresh a cada rodada de investimento
- Total acumulado ao longo do tempo: **15-25% diluído entre todos colaboradores**

---

## 🎯 Para Quem Dar Equity?

### Por Nível Hierárquico

**Founders**:
```
Equity: 60-80% total (dividido entre co-founders)
Não é "programa de equity", é ownership original
Vesting: Reverse vesting (4 anos, cliff 1 ano)
```

**C-Level (CTO, CFO, CPO, CMO)**:
```
Equity típico: 0.5-3% cada
Vesting: 4 anos, cliff 1 ano
Strike price: FMV na contratação
```

**VP-Level / Heads**:
```
Equity típico: 0.1-0.5% cada
Vesting: 4 anos, cliff 1 ano
```

**Senior IC (Individual Contributors)**:
```
Equity típico: 0.01-0.1% cada
Vesting: 4 anos, cliff 1 ano
```

**Mid-Level / Junior**:
```
Equity típico: 0.001-0.05% cada
Vesting: 4 anos, cliff 1 ano
Comum dar apenas em Series A+ (não em seed)
```

---

### Por Timing de Entrada

**Employee #1-10** (early team):
```
Equity: 0.5-2% cada (senior roles)
Razão: Alto risco, empresa pequena
Desconto no strike price: 30-50% do FMV
```

**Employee #11-50**:
```
Equity: 0.1-0.5% cada
Razão: Ainda early, mas menos risco que #1-10
```

**Employee #51-200**:
```
Equity: 0.01-0.1% cada
Razão: Empresa mais madura, menos risco
```

**Regra**: Quanto mais cedo entra, mais equity (compensa risco maior)

---

## 📈 Cases de Startups Brasileiras

### Nubank

**Estratégia**:
- Stock options para todos funcionários (não apenas leadership)
- Programa agressivo de equity desde cedo
- IPO em 2021: muitos funcionários viraram milionários

**Números públicos**:
- Colaboradores receberam ~R$6 bilhões em equity no IPO
- Mais de 3.000 "nubankers" com equity
- Cases de analytics senior que entrou em 2015 com ~0.1% → ~R$20M no IPO

---

### Stone

**Estratégia**:
- Equity para key roles (C-level, VP-level, Head-level)
- IPO em 2018 (NYSE)

**Números**:
- Early employees com 0.5-1% ganharam R$50-100M+

---

### QuintoAndar / Loft

**Estratégia**:
- Phantom shares (eram LTDA por muito tempo)
- Transformaram em SA antes de Series B/C
- Equity para tech + product + key commercial roles

---

### Lições dos Cases

1. **Equity funciona**: Early employees que acreditaram e ficaram geraram riqueza real
2. **Vesting é crítico**: Quem saiu cedo (antes do cliff) perdeu tudo
3. **Comunicação importa**: Empresas que explicaram bem equity tiveram menos arrependimento
4. **Quantidade varia**: 0.05% em unicórnio = R$5M (em valuation de R$10B)

---

## ⏱️ Quando Implementar Programa de Equity?

### Sinais de que é hora:

✅ **Contratando key roles** (C-level, VP-level) que esperam equity
✅ **Competindo por talentos** com empresas que oferecem equity
✅ **Levantou seed/Series A** (investidores geralmente exigem equity pool)
✅ **Time >10 pessoas** (equity vira diferencial de retenção)
✅ **Planejando crescer rápido** (50+ pessoas em 18 meses)

### Sinais de que ainda é cedo:

❌ **Pre-revenue, validando ideia** (equity sem vesting pode virar problema)
❌ **Time <5 pessoas** (todos são co-founders, não precisa programa formal)
❌ **Alta incerteza de pivot** (difícil justificar equity se produto muda toda hora)

**Timing típico**:
- **Phantom shares**: Seed stage, após validar PMF
- **Stock options**: Series A, quando transforma para SA

---

## 🧮 Calculando Valor de Equity

### Fórmula Básica

```
Valor do equity = (% ownership) × (Valuation da empresa)

Exemplo:
- Você tem 0.1% da empresa
- Empresa levantou Series A, valuation pós-money R$100M
- Seu equity "vale": 0.1% × R$100M = R$100k (no papel)

No exit (M&A por R$500M):
- Seu equity vale: 0.1% × R$500M = R$500k
- Menos: valor pago no exercício (se stock options)
```

### Diluição

**Cada rodada de investimento dilui**:
```
Situação inicial:
- Você: 0.5% da empresa
- Empresa: R$10M valuation

Series A (investidor compra 20%):
- Todos são diluídos em 20%
- Você agora: 0.5% × 80% = 0.4%
- Empresa: R$50M valuation (pós-money)
- Seu equity: 0.4% × R$50M = R$200k

Mesmo com diluição, seu equity VALEU MAIS (R$50k → R$200k)
porque valuation subiu
```

**Regra**: Diluição é ok se valuation sobe proporcionalmente

---

## 📚 Benchmarks de Equity

### Por Role (% da empresa)

| Role | Pre-Seed/Seed | Series A | Series B+ |
|------|---------------|----------|-----------|
| CEO | 20-40% | 15-30% | 10-25% (diluído) |
| CTO (co-founder) | 10-25% | 8-20% | 5-15% (diluído) |
| CTO (hire) | 1-3% | 0.5-2% | 0.3-1% |
| VP Eng | 0.3-1% | 0.2-0.6% | 0.1-0.4% |
| Senior Eng | 0.05-0.2% | 0.03-0.1% | 0.01-0.05% |
| Mid Eng | 0.01-0.05% | 0.005-0.03% | 0.005-0.02% |

### Por Valuation (valor absoluto do equity)

**Series A (R$50M valuation)**:
- VP-level: 0.3% = R$150k
- Senior IC: 0.05% = R$25k
- Mid IC: 0.01% = R$5k

**Series B (R$200M valuation)**:
- VP-level: 0.2% = R$400k
- Senior IC: 0.03% = R$60k

---

## ⚠️ Armadilhas Comuns

### Erro #1: Dar equity sem vesting
```
Problema: Pessoa recebe equity, sai em 3 meses, fica com tudo
Solução: SEMPRE usar vesting (4 anos, cliff 1 ano mínimo)
```

### Erro #2: Prometer equity sem formalizar
```
Problema: "Você vai ter 1% da empresa" verbal, sem contrato
Solução: SEMPRE documentar em contrato formal
```

### Erro #3: Não explicar equity
```
Problema: Colaborador não entende valor, acha que é "bonus"
Solução: Educação + transparência (cenários de exit, diluição)
```

### Erro #4: Strike price errado
```
Problema: Strike price = valuation atual (não há ganho no exercício)
Solução: Strike price deve ser FMV no momento da concessão (ou menor)
```

### Erro #5: Equity para todos sem critério
```
Problema: Dilui demais, equity vira "commodity"
Solução: Equity para key roles (não todos), aumenta conforme seniority
```

---

## 🎯 Resumo Executivo

**O que dar**:
- LTDA: Phantom Shares
- SA: Stock Options

**Quanto dar**:
- Equity pool total: 10-20%
- C-level: 0.5-3%
- VP/Head: 0.1-0.5%
- Senior IC: 0.01-0.1%

**Como estruturar**:
- Vesting: 4 anos
- Cliff: 1 ano
- Strike price: FMV ou desconto para early employees

**Quando implementar**:
- Seed stage (phantom shares)
- Series A (stock options, transformar para SA)

---

**Próximos guias**:
- [legal-structures-brazil.md](legal-structures-brazil.md) - Detalhes de LTDA vs SA
- [contracts-templates.md](contracts-templates.md) - Modelos de contratos
- [taxation-brazil.md](taxation-brazil.md) - Tributação completa
