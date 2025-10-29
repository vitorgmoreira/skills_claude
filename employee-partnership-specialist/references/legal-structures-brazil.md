# Estruturas Jurídicas de Equity no Brasil

Guia completo sobre LTDA vs SA, transformação, requisitos legais e compliance para programas de equity.

---

## 🏢 LTDA vs SA: Comparação Completa

### Sociedade Limitada (LTDA)

**Características**:
- Tipo societário mais comum no Brasil (~95% das empresas)
- Regulada pelo Código Civil (não Lei das SAs)
- Capital dividido em quotas (não ações)
- Menor burocracia e custos
- Não tem ações negociáveis

**Equity options em LTDA**:
- ✅ **Phantom Shares** (ações fantasma)
- ✅ **SARs** (Stock Appreciation Rights)
- ❌ **Stock Options** reais (NÃO permitido legalmente)
- ❌ **RSUs** (não faz sentido sem ações)

**Vantagens**:
- Custos menores (contabilidade ~R$1-3k/mês)
- Menos burocracia
- Flexibilidade contratual

**Desvantagens**:
- Não pode dar ownership real (apenas synthetic)
- Dificulta captação de investidores (VCs preferem SA)
- Limitações para IPO

---

### Sociedade Anônima (SA)

**Características**:
- Capital dividido em **ações**
- Regulada pela Lei 6.404/76 (Lei das SAs)
- Pode ser **fechada** (maioria) ou **aberta** (listada em bolsa)
- Requerida para stock options reais
- Exigida por investidores (Series A+)

**Equity options em SA**:
- ✅ **Stock Options** (principal motivo para virar SA)
- ✅ **Phantom Shares**
- ✅ **RSUs**
- ✅ **SARs**

**Vantagens**:
- Permite ownership real (ações)
- Facilita investimentos (VCs exigem SA)
- Caminho para IPO
- Mais credibilidade

**Desvantagens**:
- Custos maiores (contabilidade ~R$5-15k/mês)
- Mais burocracia (AGE, atas, publicações)
- Compliance mais rigoroso

---

## 🔄 Transformação LTDA → SA

### Quando Transformar?

**Sinais de que é hora**:
- ✅ Levantando Series A (investidores exigem)
- ✅ Quer dar stock options reais (não phantom)
- ✅ Planejando IPO no longo prazo
- ✅ >R$10M em valuation

**Ainda pode esperar**:
- ❌ Pre-seed, early seed
- ❌ Phantom shares atendem necessidade
- ❌ Ainda não tem investidor exigindo

---

### Processo de Transformação

**Etapas** (2-4 meses):

**1. Preparação** (semanas 1-2):
- Auditoria contábil (balanço patrimonial)
- Regularização de pendências (débitos, tributos)
- Definição de capital social da SA
- Escolha de advogado especializado

**2. Assembleia de Transformação** (semana 3):
- Convocação de Reunião de Quotistas
- Aprovação da transformação (unanimidade ou maioria qualificada)
- Aprovação do Estatuto Social da SA
- Lavratura de ata

**3. Registro e Publicações** (semanas 4-8):
- Registro na Junta Comercial
- Publicação em Diário Oficial
- Publicação em jornal de grande circulação
- Atualização CNPJ (mesmo número mantido)

**4. Ajustes Finais** (semanas 9-16):
- Ajustes contábeis
- Comunicação a bancos, fornecedores
- Setup de governança (Conselho, etc.)

---

### Custos de Transformação

| Item | Valor Estimado |
|------|----------------|
| Honorários advocatícios | R$15.000 - R$30.000 |
| Contabilidade (ajustes + setup) | R$5.000 - R$10.000 |
| Registro Junta Comercial | R$500 - R$2.000 |
| Publicações (DO + jornal) | R$2.000 - R$5.000 |
| Despesas diversas | R$2.000 - R$5.000 |
| **TOTAL** | **R$30.000 - R$80.000** |

**Custos recorrentes pós-transformação**:
- Contabilidade: R$5-15k/mês (vs R$1-3k em LTDA)
- Publicações anuais: R$3-8k/ano
- Auditoria (se necessário): R$20-50k/ano

---

## 📜 Stock Options em SA: Requisitos Legais

### Aprovação em Assembleia Geral

**Processo**:
1. Conselho de Administração propõe Plano de Stock Options
2. Convocação de Assembleia Geral Extraordinária (AGE)
3. Aprovação por maioria (ou unanimidade conforme estatuto)
4. Lavratura de ata registrando aprovação

**Itens obrigatórios no Plano**:
- Número máximo de ações a serem emitidas
- Beneficiários elegíveis (colaboradores, administradores)
- Strike price (preço de exercício)
- Prazo de exercício
- Condições de vesting

---

### Registro CVM (se aplicável)

**Quando necessário**:
- SA aberta (listada em bolsa) → registro CVM obrigatório
- SA fechada → não precisa (maioria das startups)

**Exceção**: Oferta pública de stock options em SA fechada pode exigir registro

---

## 🧾 Phantom Shares em LTDA: Como Estruturar

### Natureza Jurídica

Phantom shares **NÃO são quotas societárias**, são:
- Contrato civil de participação nos lucros/ganhos futuros
- Direito contratual (não societário)
- Não gera ownership legal da empresa

---

### Documentação Necessária

**1. Plano de Phantom Shares** (empresa):
- Documento interno aprovado pelos sócios
- Define regras gerais do programa
- Não precisa registro em Junta

**2. Acordo Individual de Phantom Shares**:
- Contrato entre empresa e colaborador
- Especifica quantidade, vesting, triggers de pagamento
- Assinado individualmente

**Não precisa**:
- ❌ Alteração contratual
- ❌ Registro em Junta Comercial
- ❌ Aprovação em assembleia

---

### Triggers de Pagamento

Phantom shares são pagas quando:
1. **Exit (M&A)**: Empresa vendida
2. **Liquidez**: Distribuição de dividendos extraordinários
3. **IPO**: Conversão em ações reais (se transformar SA)
4. **Outros eventos**: Definidos em contrato

**Importante**: Empresa precisa ter CAIXA para pagar (diferente de stock options onde colaborador compra)

---

## ⚖️ Aspectos Trabalhistas

### Equity NÃO é Salário

**Fundamentação legal**:
- Equity é participação societária ou direito contratual
- Não tem natureza salarial (se bem estruturado)
- Não integra base de cálculo de FGTS, 13º, férias

**Cuidados para evitar natureza salarial**:
- ✅ Vesting de longo prazo (4 anos)
- ✅ Documento separado do contrato de trabalho
- ✅ Não vincular a performance mensal/anual
- ✅ Deixar claro: "não é remuneração variável"
- ❌ Evitar: pagar equity como bônus anual recorrente

---

### Rescisão e Equity

**Good Leaver vs Bad Leaver** (definir em contrato):

**Good Leaver** (saída amigável):
- Demissão sem justa causa
- Pedido de demissão após período mínimo
- Invalidez, morte
- **Mantém**: Equity já vestido
- **Perde**: Equity não vestido

**Bad Leaver** (saída problemática):
- Demissão com justa causa
- Violação de deveres
- Competição desleal
- **Perde**: Todo equity (vestido e não vestido) ou parte

**Cláusula de repurchase**:
- Empresa pode recomprar equity de bad leaver
- Preço: geralmente strike price (no gain)

---

## 🌍 Estruturas Offshore

### Por Que Offshore?

**Vantagens**:
- Otimização tributária (paraísos fiscais)
- Facilita investimento estrangeiro
- Estrutura comum em VCs (Cayman, Delaware)
- IPO futuro (NASDAQ, NYSE)

**Desvantagens**:
- Complexidade jurídica
- Custos de setup (R$50-150k)
- Custos recorrentes (R$20-50k/ano)

---

### Estrutura Típica: Cayman + Brasil

```
INVESTIDORES INTERNACIONAIS
    ↓
CAYMAN HOLDCO (holding offshore)
    ↓
SPV BRASIL (Sociedade de Propósito Específico)
    ↓
OPCO BRASIL (SA operacional)
```

**Como funciona equity**:
1. Colaboradores recebem stock options da **Cayman Holdco**
2. Cayman Holdco possui SPV Brasil
3. SPV Brasil possui Opco Brasil (operação real)
4. No exit, Cayman é vendida (não empresa BR diretamente)

**Benefícios tributários**:
- Cayman: 0% imposto corporativo
- Ganho de capital em Cayman pode ter tratamento mais favorável
- Estruturação de exit mais eficiente

**Quando usar**:
- Series A+ com investidores internacionais
- Planejando IPO nos EUA
- Empresa global (não apenas Brasil)

**Quando NÃO usar**:
- Seed stage, operação 100% Brasil
- Complexidade não justifica benefício

---

## 📋 Compliance e Regulação

### LGPD em Programas de Equity

**Dados pessoais envolvidos**:
- CPF, RG, endereço
- Dados bancários (para pagamento)
- Informações de equity (quantidade, vesting)

**Obrigações**:
- Base legal: execução de contrato
- Consentimento para compartilhar com cap table tool (Carta, etc.)
- Política de privacidade específica

---

### Nota Fiscal

**Phantom Shares**:
- Pagamento é tributado como bônus/PLR
- Empresa deve emitir recibo de pagamento
- Retenção de IR na fonte (IRRF)

**Stock Options**:
- Exercício: colaborador paga empresa (emitir NF se valor alto)
- Venda futura: ganho de capital (DARF individual)

---

### Contratos Internacionais

Se colaborador é estrangeiro ou equity é offshore:
- Contrato em inglês + português (bilíngue)
- Escolha de foro (Brasil ou Delaware/Cayman)
- Arbitragem (recomendado para disputas internacionais)

---

## 🎯 Resumo Executivo

**LTDA**:
- Use: Pre-seed, seed
- Equity: Phantom shares
- Custo: Baixo (R$1-3k/mês contabilidade)

**SA**:
- Use: Series A+, stock options reais
- Custo transformação: R$30-80k
- Custo recorrente: R$5-15k/mês

**Offshore (Cayman)**:
- Use: Series A+ internacional, IPO futuro
- Custo setup: R$50-150k
- Custo recorrente: R$20-50k/ano

**Compliance**:
- Equity ≠ salário (estruturar bem)
- Good/bad leaver definido em contrato
- LGPD: consentimento para dados

---

**Próximos guias**:
- [contracts-templates.md](contracts-templates.md) - Modelos de contratos
- [taxation-brazil.md](taxation-brazil.md) - Tributação detalhada
