# Vesting, Cliff e Aceleração

Guia completo sobre estruturas de vesting, cliff, good/bad leaver e acceleration clauses.

---

## 📅 Vesting: Conceito Fundamental

**Vesting** = Processo gradual de "conquistar" o direito ao equity ao longo do tempo

**Por quê vesting existe?**:
- Retenção (incentivo para ficar 4 anos)
- Proteção da empresa (pessoa que sai cedo não leva equity todo)
- Alinhamento de longo prazo

---

## ⏱️ Estrutura Padrão de Vesting

### Modelo 4 anos com Cliff de 1 ano

```
PADRÃO DA INDÚSTRIA (Silicon Valley + Brasil):
- Duração total: 4 anos
- Cliff: 1 ano
- Vesting após cliff: Mensal

Exemplo - 48.000 stock options:
Mês 0-11: 0 options vestidas (cliff)
Mês 12: 12.000 options vestidas (25% de uma vez)
Mês 13-48: 1.000 options/mês (remaining 75% ÷ 36 meses)
```

**Cronograma visual**:
```
Ano 1: ||||||||||||  → 25% (cliff)
Ano 2: ||||||||||||  → 50% total
Ano 3: ||||||||||||  → 75% total
Ano 4: ||||||||||||  → 100% total
```

---

## 🧱 Cliff: O Período de Teste

### O Que É Cliff?

**Cliff** = Período mínimo antes de qualquer equity vestir

**Regra**: Se sair ANTES do cliff, perde TODO equity (0%)

**Exemplo**:
```
Pessoa recebe 10.000 options, cliff 1 ano

Cenário A: Sai no mês 11 (antes do cliff)
- Equity vestido: 0
- Leva: Nada

Cenário B: Sai no mês 13 (após cliff)
- Equity vestido: 25% + 2 meses adicionais = ~29%
- Leva: 2.900 options
```

---

### Por Que 1 Ano de Cliff?

**Razões**:
1. **Período de teste**: 1 ano mostra se pessoa se adapta
2. **Proteção da empresa**: Evita "job hoppers" pegarem equity
3. **Padrão de mercado**: Todo mundo usa 1 ano

**Variações**:
- **6 meses**: Raro, usado em contratações muito seniores (C-level)
- **3 meses**: Muito raro, só para casos especialíssimos
- **2 anos**: Nunca (ninguém aceita)

---

## 📆 Frequência de Vesting Pós-Cliff

### Mensal (Recomendado)

```
Exemplo (4 anos, cliff 1 ano, vesting mensal):
- Ano 1: 25% no mês 12
- Anos 2-4: 2.08% por mês (25% ÷ 12 meses)

Vantagem: Granularidade fina, justo para colaborador
```

### Trimestral

```
Exemplo:
- Ano 1: 25% no trimestre 4
- Anos 2-4: 6.25% por trimestre

Vantagem: Menos burocrático para empresa
Desvantagem: Menos justo (pessoa que sai no meio do trimestre perde)
```

### Anual

```
Exemplo:
- Ano 1: 25%
- Ano 2: 25%
- Ano 3: 25%
- Ano 4: 25%

Desvantagem: Muito chunky, não recomendado (exceto para founders)
```

**Recomendação**: **Vesting mensal pós-cliff** (padrão de mercado)

---

## 🚪 Good Leaver vs Bad Leaver

### Definições

**Good Leaver** (saída "boa"):
- Demissão sem justa causa
- Pedido de demissão após período mínimo (ex: 1-2 anos)
- Morte, invalidez
- Acordo mútuo

**Bad Leaver** (saída "ruim"):
- Demissão com justa causa
- Violação de deveres (fraude, roubo, quebra de confidencialidade)
- Competição desleal
- Pedido de demissão antes de período mínimo

---

### Consequências

**Good Leaver**:
- **Mantém**: Todo equity JÁ vestido
- **Perde**: Equity NÃO vestido ainda
- **Pode exercer** options vestidas (geralmente 90 dias após saída)

**Bad Leaver**:
- **Perde**: TODO equity (vestido + não vestido)
- OU: Empresa tem direito de **recomprar** equity vestido a strike price (sem ganho)

---

### Exemplo Completo

```
Pessoa com 10.000 options, sai no mês 30 (2.5 anos)
Equity vestido: 25% (ano 1) + 18 meses × 2.08% = 62.5%
Equity não vestido: 37.5%

GOOD LEAVER:
- Mantém: 6.250 options (62.5%)
- Perde: 3.750 options (37.5%)
- Pode exercer 6.250 em 90 dias

BAD LEAVER:
- Perde: 10.000 options (100%)
OU
- Empresa recompra 6.250 options por R$6.250 (strike R$1)
- Sem ganho (FMV atual R$10 = teria R$62.5k, mas perde)
```

---

## ⚡ Acceleration (Aceleração de Vesting)

### O Que É?

**Acceleration** = Vesting acelerado em eventos específicos (exit, demissão)

**Tipos**:
1. **Single Trigger**: 1 evento acelera (ex: M&A)
2. **Double Trigger**: 2 eventos precisam ocorrer (ex: M&A + demissão)

---

### Single Trigger Acceleration

**Definição**: Vesting acelera automaticamente no exit (M&A, IPO)

```
Exemplo:
- Pessoa com 50% vestido
- Empresa vendida (exit)
- Single trigger: 100% veste imediatamente

Resultado: Pessoa pode exercer tudo e vender no exit
```

**Vantagens (colaborador)**:
- Garante participação plena no exit
- Não fica "preso" após aquisição

**Desvantagens (empresa/comprador)**:
- Comprador não gosta (colaborador pode sair logo após exit)
- Dificulta M&A

**Raridade**: Pouco comum (VCs geralmente não permitem)

---

### Double Trigger Acceleration

**Definição**: Vesting acelera SE dois eventos ocorrerem:
1. Exit (M&A, IPO)
2. E demissão sem justa causa OU downgrade de cargo

```
Exemplo:
- Pessoa com 50% vestido
- Empresa vendida (Trigger 1)
- Pessoa é demitida pelo comprador sem justa causa (Trigger 2)
- Double trigger: 100% veste imediatamente

Resultado: Pessoa protegida se comprador demitir
```

**Vantagens**:
- Protege colaborador de demissão pós-exit
- Comprador aceita (colaborador só acelera se for demitido)
- Balanceado para ambos lados

**Recomendação**: **Double trigger para key hires** (C-level, VP-level)

---

### Comparação

| Tipo | Quando acelera | Comum? | Para quem? |
|------|---------------|--------|------------|
| Sem aceleração | Nunca | Comum | ICs, mid-level |
| Single trigger | Exit | Raro | Founders (às vezes) |
| Double trigger | Exit + demissão | Comum | C-level, VPs |

---

## 👑 Reverse Vesting para Founders

### O Que É?

**Reverse vesting** = Founders já têm equity, mas com vesting (ao contrário de ganhar gradualmente)

**Razão**: Investidores exigem (protege se founder sair cedo)

---

### Como Funciona

```
Founder tem 40% da empresa

SEM reverse vesting:
- Founder sai no mês 6
- Leva 40% (empresa fica com problema)

COM reverse vesting (4 anos, cliff 1 ano):
- Founder sai no mês 6 (antes do cliff)
- Empresa RECOMPRA 40% de volta (por preço simbólico, ex: R$1)
- Founder sai com quase nada
```

**Estrutura típica**:
- 4 anos de vesting
- Cliff de 1 ano (às vezes 6 meses para founders)
- Se sair antes: empresa recompra equity

---

## 🧮 Cálculo de Vesting

### Fórmula Geral

```
Equity vestido = Equity total × (Tempo trabalhado / Vesting period)

Com cliff de 1 ano:
- Se tempo < 1 ano: Equity vestido = 0
- Se tempo ≥ 1 ano: Equity vestido = 25% + ((tempo - 12 meses) / 36 meses) × 75%
```

### Exemplos

**Exemplo 1**: Sai no mês 11
```
10.000 options, 4 anos, cliff 1 ano
Tempo: 11 meses < 12 meses (cliff)
Vestido: 0
```

**Exemplo 2**: Sai no mês 24 (2 anos)
```
10.000 options, 4 anos, cliff 1 ano

Vestido = 25% (cliff) + ((24 - 12) / 36) × 75%
        = 25% + (12/36) × 75%
        = 25% + 25%
        = 50%
        = 5.000 options
```

**Exemplo 3**: Completa 4 anos
```
10.000 options, 4 anos, cliff 1 ano
Vestido = 100% = 10.000 options
```

---

## 📋 Checklist de Vesting

### Ao Estruturar Programa

- [ ] Duração: 4 anos (padrão)
- [ ] Cliff: 1 ano (padrão)
- [ ] Frequência pós-cliff: Mensal (recomendado)
- [ ] Good/bad leaver definido claramente
- [ ] Acceleration (se aplicável): Double trigger para key hires
- [ ] Prazo para exercer após saída: 90 dias (padrão)

### No Contrato Individual

- [ ] Quantidade total de equity
- [ ] Vesting schedule explícito
- [ ] Data de início do vesting (start date)
- [ ] Definição de good/bad leaver
- [ ] Cláusula de repurchase (bad leaver)
- [ ] Acceleration clauses (se aplicável)
- [ ] Post-termination exercise period

---

## ⚠️ Erros Comuns

**Erro #1**: Não ter cliff
```
Problema: Pessoa sai em 3 meses, leva 6.25% de equity
Solução: Sempre cliff de 1 ano mínimo
```

**Erro #2**: Vesting muito longo (>4 anos)
```
Problema: Ninguém aceita vesting de 5-6 anos
Solução: 4 anos é padrão, não mude
```

**Erro #3**: Good/bad leaver mal definido
```
Problema: Disputa legal sobre se pessoa é good ou bad leaver
Solução: Definir claramente em contrato com exemplos
```

**Erro #4**: Single trigger em todos
```
Problema: Exit acontece, todo mundo acelera e sai
Solução: Single trigger só para founders (se tanto), double trigger para key hires
```

---

## 🎯 Resumo Executivo

**Padrão de mercado (use sempre)**:
- 4 anos de vesting
- Cliff de 1 ano
- Vesting mensal pós-cliff

**Good/Bad Leaver**:
- Good: Mantém vestido, perde não-vestido
- Bad: Perde tudo (ou empresa recompra a strike price)

**Acceleration**:
- Sem aceleração: ICs, mid-level
- Double trigger: C-level, VP-level
- Single trigger: Evitar (problemas em M&A)

**Reverse Vesting**:
- Founders: 4 anos, cliff 6-12 meses
- Protege investidores

**Prazo pós-saída**:
- 90 dias para exercer options (padrão)
- Após 90 dias: options expiram

---

**Próximo guia**: [communication-transparency.md](communication-transparency.md)
