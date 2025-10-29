# Valuation e Strike Price

Guia sobre como definir strike price, fair market value e atualização de valuation.

---

## 💰 Strike Price: O Que É?

**Strike price** (ou exercise price) = Preço que colaborador paga para comprar ações ao exercer stock options

**Regra fundamental**: Strike price deve ser ≤ Fair Market Value (FMV) no momento da concessão

---

## 📊 Fair Market Value (FMV)

**FMV** = Valor "justo" da ação no mercado

**Como determinar**:
1. **Pós-rodada de investimento**: Preço pago pelo investidor (price per share)
2. **Entre rodadas**: Valuation da última rodada (conservador) ou projeção
3. **409A valuation** (conceito EUA): Avaliação independente

**Exemplo**:
```
Series A:
- Investidor paga R$20M por 20% da empresa
- Valuation pós-money: R$100M
- Total de ações: 10M
- Price per share (FMV): R$100M / 10M = R$10,00

Strike price para options concedidas agora: R$10,00
```

---

## 🎯 Definindo Strike Price

### Opção 1: Strike = FMV (Padrão)

**Mais comum e seguro**:
- Strike price = FMV atual
- Sem risco tributário (não há "desconto")
- Colaborador ganha se empresa valorizar

---

### Opção 2: Strike < FMV (Desconto para Early Employees)

**Para primeiros 10-20 contratados**:
- Strike price com desconto de 30-70% do FMV
- Compensa risco maior

**Exemplo**:
```
FMV: R$10,00
Strike price (30% desconto): R$7,00

Vantagem para colaborador:
- Ganho imediato no exercício: (R$10 - R$7) × 10.000 = R$30k extra
```

**Cuidado tributário**: Desconto pode ser considerado renda tributável no exercício

---

## 🔄 Atualização de Valuation

**Quando atualizar**:
- Após cada rodada de investimento (obrigatório)
- Anualmente (entre rodadas, recomendado)
- Eventos materiais (M&A offer, pivot significativo)

**Strike price para futuras concessões**:
- Sempre usar FMV ATUAL (no momento da concessão)
- Options já concedidas: strike price não muda (fixo)

---

## 📈 Preferred vs Common Stock

**Investidores compram Preferred Stock** (ações preferenciais):
- Liquidation preference (recebem primeiro no exit)
- Proteção anti-diluição
- Direitos especiais

**Colaboradores recebem Common Stock** (ações ordinárias):
- Sem liquidation preference
- Vale menos que preferred (desconto de 10-40%)

**Impacto no strike price**:
```
Investidor paga R$10/ação (preferred)
FMV de common stock: R$6-9/ação (desconto aplicado)
Strike price para options: R$6-9 (não R$10)
```

---

**Ver**: `equity-fundamentals.md` para contexto completo
