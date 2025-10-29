# Tributação de Equity no Brasil

Guia completo sobre IR, INSS, ganho de capital e otimização fiscal em programas de equity.

---

## 🎯 Visão Geral Tributária

### Regra Fundamental

**Equity é tributado em 2 momentos**:
1. **Exercício** (stock options) ou **Recebimento** (phantom shares)
2. **Venda** (ganho de capital)

---

## 📊 Stock Options: Tributação Completa

### Momento 1: Exercício das Options

**Fato gerador**: Colaborador exerce options (compra ações abaixo do FMV)

**Base de cálculo**:
```
Ganho no exercício = (FMV atual - Strike price) × Quantidade

Exemplo:
- 10.000 options, strike price R$1,00
- FMV atual: R$10,00
- Ganho = (R$10 - R$1) × 10.000 = R$90.000
```

**Tributação**:
- **IR**: Tabela progressiva (até 27,5%)
- **INSS**: Geralmente NÃO incide (se bem estruturado)
- **DARF**: Colaborador paga individualmente

**Tabela IR 2024**:
| Base de Cálculo | Alíquota | Parcela a Deduzir |
|-----------------|----------|-------------------|
| Até R$2.112 | Isento | - |
| R$2.112 a R$2.826 | 7,5% | R$158,40 |
| R$2.826 a R$3.751 | 15% | R$370,40 |
| R$3.751 a R$4.664 | 22,5% | R$651,73 |
| Acima R$4.664 | 27,5% | R$884,96 |

**No exemplo** (ganho de R$90k):
- IR = R$90.000 × 27,5% - R$884,96 = R$23.865,04

---

### Momento 2: Venda das Ações (Ganho de Capital)

**Fato gerador**: Colaborador vende ações (exit, IPO, mercado secundário)

**Base de cálculo**:
```
Ganho de capital = (Preço de venda - Custo de aquisição)

Custo de aquisição = Strike price + IR pago no exercício

Exemplo (continuando):
- Comprou por R$1 + pagou R$23.865 de IR no exercício
- Vende por R$50,00/ação
- Ganho = (R$50 - R$1) × 10.000 = R$490.000
- IR no ganho de capital: R$490.000 × 15% = R$73.500
```

**Alíquotas de Ganho de Capital**:
| Ganho | Alíquota |
|-------|----------|
| Até R$5 milhões | 15% |
| R$5M a R$10M | 17,5% |
| R$10M a R$30M | 20% |
| Acima R$30M | 22,5% |

**Importante**: 
- Colaborador paga via DARF até último dia do mês seguinte à venda
- Declarar em IRPF (Ganhos de Capital)

---

### Caso Completo: Stock Options

```
CONCESSÃO (Dia 0):
- 10.000 options, strike R$1,00
- Impostos: R$0 (nada devido)

EXERCÍCIO (Após vesting):
- FMV: R$10,00
- Colaborador paga: R$10.000 (strike)
- Ganho tributável: R$90.000
- IR devido: R$23.865
- Custo total: R$33.865

VENDA (Exit, R$50/ação):
- Recebe: R$500.000
- Ganho de capital: R$490.000
- IR devido: R$73.500
- Líquido final: R$426.500

Resumo tributário total: R$97.365 (23%)
```

---

## 👻 Phantom Shares: Tributação Completa

### Natureza Tributária

**Phantom shares são tributadas como rendimento do trabalho** (não ganho de capital)

**Por quê?**: Não há ownership real, é bônus/PLR contratual

---

### Momento do Pagamento (Exit, Distribuição)

**Fato gerador**: Empresa paga phantom shares (exit, dividendos)

**Tributação**:
- **IR**: 27,5% (fonte - IRRF)
- **INSS**: Potencialmente sim (depende de estruturação)
- **Empresa retém e recolhe IR**

**Exemplo**:
```
PHANTOM SHARES:
- 10.000 phantom shares
- Valor base: R$1,00
- Exit: R$50,00/share
- Ganho: (R$50 - R$1) × 10.000 = R$490.000

Tributação:
- IR (27,5%): R$134.750
- INSS (11% até teto de ~R$7.5k): R$825 (se incidir)
- Líquido: ~R$354.425

Empresa paga colaborador: R$354.425 líquido
Empresa recolhe aos cofres públicos: R$135.575
```

---

### Comparação: Stock Options vs Phantom Shares

**Mesmo ganho de R$490k**:

| Item | Stock Options | Phantom Shares |
|------|---------------|----------------|
| IR total | ~R$97k (23%) | R$135k (27,5%) |
| INSS | Geralmente não | Potencial R$825 |
| Quem paga IR | Colaborador (DARF) | Empresa (IRRF) |
| Liquidez | Colaborador paga exercício | Empresa paga tudo |
| **Líquido final** | **R$426k** | **R$354k** |

**Diferença**: R$72k a menos em phantom shares (tributação mais pesada)

---

## 🏢 Obrigações da Empresa

### DIRF (Declaração de IR Retido na Fonte)

**Quando**: Anualmente (fevereiro do ano seguinte)

**O que declarar**:
- Phantom shares pagas no ano
- IR retido (IRRF)
- Dados do beneficiário (CPF, valor bruto, IR retido)

---

### DARF (Recolhimento)

**Phantom shares**:
- Empresa recolhe IRRF até 20º dia do mês seguinte ao pagamento
- Código DARF: 0561

**Stock options**:
- Colaborador recolhe individualmente (não é obrigação da empresa)
- Empresa pode ajudar educando colaborador

---

### Informações em Recibo de Pagamento

**Phantom shares** (quando pagar):
```
RECIBO DE PAGAMENTO

Beneficiário: João da Silva
CPF: XXX.XXX.XXX-XX

Phantom Shares:
Quantidade: 10.000
Valor por share: R$50,00
Valor total bruto: R$500.000,00

Tributos:
IRRF (27,5%): R$137.500,00
INSS (se aplicável): R$825,00

Valor líquido: R$361.675,00
```

---

## 💡 Estratégias de Otimização Fiscal

### 1. Estrutura Offshore (Cayman)

**Como funciona**:
- Colaborador tem stock options da Cayman Holdco (não empresa BR)
- Cayman: 0% imposto corporativo
- Ganho de capital em venda de ações Cayman pode ter tratamento diferenciado

**Benefícios potenciais**:
- Adiamento de tributação (até venda)
- Possível redução de alíquota (depende de estrutura e tratado)

**Custos**:
- Setup: R$50-150k
- Manutenção: R$20-50k/ano
- Só vale a pena em Series A+ com ganhos grandes

---

### 2. Timing do Exercício

**Stock options**: Colaborador controla quando exercer

**Estratégia**:
- Exercer em ano de renda menor (menor alíquota progressiva)
- Evitar exercer tudo de uma vez (pode pular para 27,5%)
- Parcelar exercício ao longo de meses/anos

**Exemplo**:
```
Ruim: Exercer 100k options de uma vez
- Ganho de R$1M de uma vez
- IR: 27,5% = R$275k

Melhor: Exercer 25k options por ano (4 anos)
- Ganho de R$250k/ano
- IR: 27,5% mas distribuído = R$275k total
- Vantagem: Fluxo de caixa melhor, possível dedução de dependentes
```

---

### 3. Deduções no IRPF

**Colaborador pode deduzir**:
- Dependentes (R$2.275,08 por dependente/ano em 2024)
- Gastos com educação (até R$3.561,50 por pessoa)
- Gastos com saúde (sem limite)
- Previdência privada (PGBL - até 12% da renda)

**Impacto**: Pode reduzir alíquota efetiva de 27,5% para ~20-25%

---

### 4. Pessoa Jurídica (PJ)

**Polêmica**: Alguns tentam receber equity via PJ

**Riscos**:
- Receita Federal pode considerar "pejotização" (fraude)
- Se caracterizar relação de emprego, multas pesadas
- Jurisprudência desfavorável

**Quando pode funcionar**:
- Consultores externos (não funcionários CLT)
- Equity como parte de honorários de consultoria
- Relação claramente não-empregatícia

**Não recomendado** para funcionários CLT tentando "virar PJ" apenas para equity

---

## 🌍 Casos Especiais

### Colaborador Estrangeiro no Brasil

**Residente fiscal no Brasil**:
- Tributação igual a brasileiro
- IR brasileiro incide normalmente

**Não-residente**:
- Retenção de 15% (IRRF) na fonte
- Possível tratado de dupla tributação (depende do país)

---

### Colaborador Brasileiro no Exterior

**Trabalha remoto de fora do Brasil**:
- Pode perder residência fiscal BR (após 12 meses fora)
- Equity pode ser tributado no país de residência
- Obrigação de declarar bens no exterior (se >US$100k)

---

## ⚠️ Erros Tributários Comuns

### Erro #1: Não pagar IR no exercício

```
Problema: Colaborador exerce options, não paga IR
Consequência: Multa de 75-150% + juros Selic
Solução: Educar colaborador, avisar sobre DARF
```

### Erro #2: Empresa não reter IRRF (phantom shares)

```
Problema: Empresa paga phantom shares sem reter IR
Consequência: Empresa é responsável solidária, multa pesada
Solução: Sempre reter 27,5% na fonte
```

### Erro #3: Confundir custo de aquisição

```
Problema: Calcular ganho de capital errado (não deduzir IR já pago)
Consequência: Paga IR duas vezes sobre mesmo valor
Solução: Custo = strike price + IR do exercício
```

### Erro #4: Não declarar em IRPF

```
Problema: Colaborador não declara ganho de capital
Consequência: Malha fina, multa, juros
Solução: Declarar sempre (Ganhos de Capital + Bens e Direitos)
```

---

## 📋 Checklist Tributário

### Para Empresas

**Phantom Shares**:
- [ ] Reter IRRF 27,5% no pagamento
- [ ] Recolher DARF até dia 20 do mês seguinte
- [ ] Emitir recibo de pagamento com IR discriminado
- [ ] Declarar em DIRF anualmente
- [ ] Considerar INSS (consultar contador)

**Stock Options**:
- [ ] Informar colaborador sobre obrigação de pagar IR
- [ ] Fornecer cálculo de ganho no exercício
- [ ] Manter registro de FMV histórico
- [ ] Não reter IR (colaborador paga)

---

### Para Colaboradores

**Stock Options**:
- [ ] Pagar DARF no exercício (ganho = FMV - strike)
- [ ] Guardar comprovante de pagamento de IR
- [ ] Declarar em IRPF (Bens e Direitos)
- [ ] Pagar IR de ganho de capital na venda
- [ ] Declarar venda em IRPF

**Phantom Shares**:
- [ ] Verificar IR retido em recibo
- [ ] Declarar em IRPF (Rendimentos Tributáveis)
- [ ] Guardar recibo de pagamento

---

## 🎯 Resumo Executivo

**Stock Options**:
- IR no exercício: até 27,5% (tabela progressiva)
- IR na venda: 15-22,5% (ganho de capital)
- Tributação total: ~20-30% do ganho
- **Colaborador paga** (via DARF)

**Phantom Shares**:
- IR no pagamento: 27,5% (IRRF)
- INSS: Potencial (até teto)
- Tributação total: ~28-30% do ganho
- **Empresa retém e paga**

**Otimização**:
- Offshore (Cayman): Para Series A+ com exit grande
- Timing de exercício: Distribuir ao longo do tempo
- Deduções: Maximizar (dependentes, saúde, educação)

**Obrigações Empresa**:
- DIRF anual (phantom shares)
- Educar colaborador (stock options)
- Manter registros de FMV

---

**Próximo guia**: [vesting-cliff-guide.md](vesting-cliff-guide.md)
