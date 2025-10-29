# Willingness to Pay: Metodologias de Pesquisa

Guia completo sobre como descobrir quanto seu cliente está disposto a pagar, usando metodologias validadas: Van Westendorp, Conjoint Analysis, Win/Loss Analysis, entrevistas e outras técnicas.

---

## Por Que Descobrir Willingness to Pay (WTP)

**WTP = O máximo que cliente pagaria pelo seu produto.**

**Por que importa:**

1. **Evita deixar dinheiro na mesa**
   - Se WTP é R$500, mas você cobra R$200 → Perdeu R$300

2. **Evita preço muito alto**
   - Se WTP é R$200, mas você cobra R$500 → Não vende

3. **WTP varia 10x entre personas**
   - Startup vs. Enterprise
   - SMB vs. Mid-market
   - Descobrir WTP de cada segmento maximiza revenue

---

## Problema: Cliente Não Sabe (ou Não Fala) WTP Real

**Se você perguntar diretamente:**
```
"Quanto você pagaria por X?"
```

**Respostas típicas:**
- "Depende..." (vago)
- R$50 (muito menos que real WTP - quer deal)
- "Não sei" (sincero, mas inútil)

**Conclusão:** Pergunta direta não funciona.

**Solução:** Usar metodologias indiretas e baseadas em dados.

---

## Metodologia 1: Van Westendorp Price Sensitivity Meter (PSM)

### Conceito

**Método criado por economista holandês Peter van Westendorp (1976).**

**Faz 4 perguntas para descobrir range de preços aceitável.**

---

### As 4 Perguntas

Você mostra o produto/descrição e pergunta:

**1. A que preço você consideraria [produto] BARATO DEMAIS, fazendo você questionar a qualidade?**
- (Too Cheap - TC)

**2. A que preço você consideraria [produto] uma PECHINCHA - um ótimo negócio?**
- (Bargain - B)

**3. A que preço você começaria a pensar que [produto] está FICANDO CARO, mas ainda consideraria comprar?**
- (Getting Expensive - GE)

**4. A que preço [produto] seria CARO DEMAIS - você não consideraria comprar?**
- (Too Expensive - TE)

---

### Como Analisar Respostas

**Passo 1:** Coletar respostas de 50-200 pessoas (quanto mais, melhor).

**Passo 2:** Criar gráfico com 4 linhas (% acumulada de respostas):

```
Eixo X: Preço (R$)
Eixo Y: % de respondentes

4 linhas:
- Too Cheap (cresce com preço)
- Bargain (decresce)
- Expensive (cresce)
- Too Expensive (cresce mais rápido)
```

**Passo 3:** Identificar pontos de interseção.

---

### Pontos-Chave do Gráfico

**1. PMC (Point of Marginal Cheapness)**
- Interseção: "Too Cheap" × "Expensive"
- **Preço mínimo aceitável**
- Abaixo disso: Qualidade questionável

**2. PME (Point of Marginal Expensiveness)**
- Interseção: "Bargain" × "Too Expensive"
- **Preço máximo aceitável**
- Acima disso: Muito caro

**3. IDP (Indifference Price Point)**
- Interseção: "Too Cheap" × "Too Expensive"
- **Preço "neutro"**
- Nem barato, nem caro

**4. OPP (Optimal Price Point)**
- Interseção: "Bargain" × "Expensive"
- **Preço ótimo recomendado**
- Balance entre percepção de valor e acessibilidade

---

### Exemplo Prático: CRM para SMB

**Amostra:** 100 SMBs brasileiras

**Respostas médias:**
- Too Cheap: R$50
- Bargain: R$200
- Getting Expensive: R$500
- Too Expensive: R$800

**Análise:**
- PMC (preço mínimo): ~R$150
- PME (preço máximo): ~R$650
- OPP (preço ótimo): ~R$350-R$400

**Recomendação:** Precificar entre R$350-R$400/mês.

---

### Vantagens do Van Westendorp

**✅ Simples de aplicar**
- 4 perguntas, fácil de responder

**✅ Revela range de preços**
- Não só um número, mas faixa aceitável

**✅ Identifica floor e ceiling**
- Preço mínimo (qualidade) e máximo (acessibilidade)

---

### Desvantagens

**❌ Assume produto único**
- Não compara features ou competidores

**❌ Hipotético (não compra real)**
- "O que você pagaria" ≠ "O que você paga"

**❌ Não considera contexto**
- Comparação com alternativas, budget

---

### Quando Usar Van Westendorp

**✅ Produto novo (sem dados históricos)**

**✅ Quer validar range de preços**

**✅ Pesquisa rápida (200-500 respondentes)**

---

## Metodologia 2: Conjoint Analysis (Análise Conjunta)

### Conceito

**Método estatístico que descobre VALOR RELATIVO de features.**

**Cliente escolhe entre opções (trade-offs), você infere WTP.**

---

### Como Funciona

**Passo 1:** Definir atributos e níveis.

**Exemplo: CRM**

**Atributos:**
1. Número de usuários: 5, 10, 50
2. Integrações: 5, 20, Ilimitado
3. Suporte: Email, Chat, Phone 24/7
4. Preço: R$100, R$300, R$500, R$800

---

**Passo 2:** Criar combinações (cenários).

**Cenário A:**
- 5 usuários
- 5 integrações
- Email support
- R$100/mês

**Cenário B:**
- 10 usuários
- 20 integrações
- Chat support
- R$300/mês

**Cenário C:**
- 50 usuários
- Ilimitado integrações
- Phone 24/7
- R$500/mês

---

**Passo 3:** Pedir para cliente RANQUEAR ou ESCOLHER.

**Pergunta:**
```
Qual dessas opções você prefere?
[ ] Cenário A
[ ] Cenário B
[ ] Cenário C
```

**Ou:** Ranquear de 1 a 3.

---

**Passo 4:** Repetir com ~10-20 combinações diferentes.

**Passo 5:** Análise estatística (regressão).

**Output:**
- "Suporte por telefone vale R$150/mês para cliente"
- "Integrações ilimitadas valem R$100/mês"
- "50 usuários vs. 5 usuários vale R$200/mês"

---

### Exemplo de Resultado

**Feature Values (WTP incremental):**

| Feature | WTP Incremental |
|---------|-----------------|
| Chat support (vs. email) | +R$50/mês |
| Phone support (vs. email) | +R$150/mês |
| 20 integrações (vs. 5) | +R$80/mês |
| Ilimitado integrações (vs. 5) | +R$120/mês |
| 50 usuários (vs. 5) | +R$250/mês |

**Implicação:**
- Tier básico (5 users, 5 integ, email): R$200/mês
- Tier Pro (10 users, 20 integ, chat): R$200 + R$80 + R$50 = R$330/mês
- Tier Enterprise (50 users, ilimitado, phone): R$200 + R$250 + R$120 + R$150 = **R$720/mês**

---

### Vantagens de Conjoint Analysis

**✅ Mede valor de features individualmente**
- Descobre quais features cliente valoriza mais

**✅ Força trade-offs reais**
- Cliente escolhe entre opções (mais realista)

**✅ Statistically robust**
- Análise de regressão, confiança estatística

---

### Desvantagens

**❌ Complexo de implementar**
- Precisa de software estatístico
- Survey design complexo

**❌ Requer amostra grande**
- Mínimo 100-200 respondentes para ser válido

**❌ Demorado**
- Survey leva 15-20 min para responder
- Análise leva dias

---

### Quando Usar Conjoint

**✅ Produto com múltiplas features**

**✅ Quer decidir quais features em quais tiers**

**✅ Tem budget para pesquisa (ou ferramenta)**

**Ferramentas:**
- Qualtrics (caro, enterprise)
- Conjointly (acessível, SaaS)
- Sawtooth Software

---

## Metodologia 3: Win/Loss Analysis

### Conceito

**Entrevistar clientes que COMPRARAM vs. que NÃO COMPRARAM.**

**Descobrir por que decidiram (ou não).**

---

### Como Fazer

**Passo 1: Identificar cohorts**

**Wins:**
- Clientes que fecharam (últimos 30 dias)

**Losses:**
- Prospects que avançaram no funil, mas não fecharam

---

**Passo 2: Entrevista (15-30 min)**

**Perguntas para Wins:**
1. Por que escolheu nosso produto (vs. alternativas)?
2. Preço foi fator? Muito alto, justo, ou bargain?
3. Quase não comprou? Por quê?
4. Se preço fosse 20% maior, teria comprado?

**Perguntas para Losses:**
1. Por que não comprou?
2. Foi preço? (Se sim, quanto seria aceitável?)
3. Qual alternativa escolheu? Por quê?
4. Se oferecêssemos X feature ou Y desconto, mudaria decisão?

---

**Passo 3: Análise temática**

**Categorizar razões:**

**Wins - Por que compraram:**
- 60%: Melhor features que competidor
- 30%: Preço competitivo
- 10%: Suporte/atendimento

**Losses - Por que não compraram:**
- 40%: Preço muito alto
- 30%: Falta de feature X
- 20%: Escolheram competidor (melhor fit)
- 10%: Budget congelado

---

### Insights de Pricing

**Se muitos Losses dizem "preço muito alto":**
- Considerar reduzir preço OU
- Melhorar comunicação de valor OU
- Criar tier mais barato

**Se Wins dizem "bargain, teria pago mais":**
- **Você está deixando dinheiro na mesa!**
- Considerar aumentar preço

---

### Exemplo Real

**SaaS de Marketing Automation**

**Win/Loss de 50 Wins, 50 Losses:**

**Wins:**
- 70% disseram: "Preço foi justo, esperado"
- 20% disseram: "Até achei barato comparado a HubSpot"
- 10% disseram: "Foi caro, mas features compensaram"

**Losses (preço-relacionado):**
- 25% disseram: "2x mais caro que Mailchimp, não justifica"
- 15% disseram: "Orçamento só tinha R$300/mês, vocês queriam R$500"

**Insight:**
- WTP está entre R$500-R$800 (wins acham justo/barato)
- Mas há segmento SMB que só paga R$300
- **Recomendação:** Criar tier Starter de R$300 para capturar SMB

---

### Vantagens de Win/Loss

**✅ Qualitativo, rico**
- Entende CONTEXTO da decisão

**✅ Revela objeções reais**
- Não é hipotético, é decisão real

**✅ Descobre competidores**
- Quem está ganhando deals, por quê

---

### Desvantagens

**❌ Demorado**
- Entrevistas 1-on-1 levam tempo

**❌ Amostra pequena**
- 20-50 entrevistas (não estatisticamente significativo)

**❌ Viés de resposta**
- Cliente pode não falar verdade sobre preço

---

### Quando Usar Win/Loss

**✅ Após lançamento (tem deals reais)**

**✅ Quer entender objeções de preço**

**✅ Quer comparar com competidores**

---

## Metodologia 4: Customer Interviews (Entrevistas Qualitativas)

### Conceito

**Conversar com clientes atuais e prospects sobre valor e preço.**

---

### Roteiro de Entrevista

**Objetivo:** Descobrir valor percebido, não perguntar preço direto.

**Perguntas:**

**1. Problema/Valor:**
- Qual problema nosso produto resolve para você?
- Quanto custa esse problema hoje? (tempo, dinheiro, oportunidade)
- Quanto vale para você resolver esse problema?

**Exemplo:**
```
Cliente: "Seu CRM economiza 5h/semana da minha equipe de vendas"
Você: "Quanto custa 5h/semana?"
Cliente: "Temos 10 vendedores, custo de R$100/h. 5h × 10 = 50h × R$100 = R$5k/semana = R$20k/mês"
```

**→ Valor econômico: R$20k/mês. WTP provável: R$2k-R$6k/mês (10-30%).**

---

**2. Alternativas:**
- O que você usava antes?
- Quanto custava?
- Por que trocou?

**Exemplo:**
```
Cliente: "Usávamos Salesforce, custava R$8k/mês"
Você: "Por que trocou?"
Cliente: "Salesforce é overkill, pagávamos por features que não usávamos"
```

**→ WTP: Provavelmente R$3k-R$6k (menos que R$8k, mas disposto a pagar por simplicidade).**

---

**3. Budget:**
- Quanto você tem de budget para essa categoria?
- Como justifica ROI internamente?

**Exemplo:**
```
Cliente: "Nosso budget de sales tools é R$10k/mês total"
Você: "Quanto desses R$10k está alocado para CRM?"
Cliente: "R$4k-R$5k"
```

**→ WTP ceiling: R$5k/mês.**

---

**4. Sensibilidade a Preço:**
- Se preço fosse 20% mais alto, ainda compraria?
- Se preço fosse 20% mais baixo, compraria mais (mais seats, features)?

**Respostas indicam elasticidade.**

---

### Exemplo de Descoberta de WTP via Entrevista

**Cliente:** Startup SaaS B2B, 20 pessoas

**Entrevista:**

**Você:** Quanto tempo sua equipe economiza por semana usando nosso produto?
**Cliente:** Umas 10 horas coletivamente.

**Você:** Quanto custa essas 10 horas?
**Cliente:** Nosso custo médio é R$150/h. 10h = R$1.500/semana = R$6k/mês.

**Você:** Quanto você pagava pela alternativa anterior?
**Cliente:** Google Sheets (grátis) + muito trabalho manual. Consideramos Airtable (R$1k/mês), mas não fechamos.

**Você:** Por que não fechou Airtable?
**Cliente:** Achamos caro para o que oferecia. Seu produto tem mais features pelo mesmo preço.

**Você:** Se nosso preço fosse R$1.500/mês (vs. R$1k atual), você compraria?
**Cliente:** Hmm, difícil. R$1k está no limite do nosso budget.

**Você:** E se fosse R$800?
**Cliente:** Fecharia na hora.

---

**Análise:**
- Valor econômico criado: R$6k/mês
- Budget ceiling: R$1k-R$1.5k/mês
- WTP sweet spot: R$800-R$1k/mês
- **Preço atual (R$1k) está no topo do WTP**
- **NÃO há espaço para aumentar preço para esse segmento (startups)**

---

### Vantagens de Entrevistas

**✅ Profundo, contextual**
- Entende o "por quê" por trás do número

**✅ Descobre valor econômico**
- Cliente articula ROI, você quantifica

**✅ Flexível**
- Pode adaptar perguntas em tempo real

---

### Desvantagens

**❌ Não-escalável**
- 10-20 entrevistas = dias de trabalho

**❌ Viés qualitativo**
- Não é estatístico

**❌ Cliente pode mentir**
- "Pagaria R$500" (mas na verdade só paga R$300)

---

### Quando Usar Entrevistas

**✅ Early-stage, descobrindo pricing**

**✅ Produto complexo (B2B)**

**✅ Quer entender contexto, não só número**

---

## Metodologia 5: A/B Testing de Preço

### Conceito

**Testar preços diferentes com grupos diferentes, medir conversão.**

**Método mais "científico" - dados reais de compra.**

---

### Como Fazer

**Setup:**
1. Dividir tráfego em 2 grupos (A/B)
2. Grupo A vê preço X
3. Grupo B vê preço Y
4. Medir conversion rate

**Exemplo:**
- Grupo A: R$99/mês → Conversion 8%
- Grupo B: R$149/mês → Conversion 6%

**Análise:**
- Grupo A: R$99 × 8% = R$7.92 revenue/visitor
- Grupo B: R$149 × 6% = R$8.94 revenue/visitor
- **Grupo B gera +13% revenue → Preço ótimo é R$149**

---

### Variações

#### Teste 1: Preço Absoluto

**Testar R$99 vs. R$149 vs. R$199.**

**Descobrir:** Qual preço maximiza revenue.

---

#### Teste 2: Framing

**Mesmo preço, framing diferente.**

**Variante A:**
```
R$99/mês
```

**Variante B:**
```
R$99/mês
ou
R$990/ano (economize R$198!)
```

**Medir:** Qual converte mais para anual.

---

#### Teste 3: Tiers

**Testar Good-Better-Best vs. apenas 2 tiers.**

**Variante A:**
```
[ Starter: R$99 ]
[ Pro: R$299 ]
```

**Variante B:**
```
[ Starter: R$99 ]
[ Pro: R$199 ]
[ Enterprise: R$499 ]
```

**Medir:** ACV (Average Contract Value).

---

### Cuidados com A/B Testing de Preço

**⚠️ Problema 1: Clientes descobrem preços diferentes**

**Cenário:**
- Cliente A viu R$99
- Cliente B viu R$149
- Cliente B descobre que A pagou menos
- **Backlash, perda de confiança**

**Solução:**
- Testar em cohorts separados (novo tráfego vs. novo geografia)
- Ou: Testar com anúncio (quem clica em Ad A vê preço A)

---

**⚠️ Problema 2: Tamanho de amostra**

**Precisa de volume suficiente.**

**Exemplo:**
- Se só tem 100 visitors/mês
- Grupo A: 50 visitors, 4 conversions (8%)
- Grupo B: 50 visitors, 3 conversions (6%)
- **Diferença não é estatisticamente significativa**

**Solução:** Precisa de 1.000+ visitors por variante para significância.

---

**⚠️ Problema 3: Otimizar para métrica errada**

**Não otimizar só para conversion rate.**

**Exemplo:**
- Preço R$50 → Conversion 15%
- Preço R$200 → Conversion 5%

**Qual é melhor?**
- R$50 × 15% = R$7.50 revenue/visitor
- R$200 × 5% = R$10 revenue/visitor
- **R$200 é melhor (mais revenue)**

**Métrica correta:** Revenue per visitor OU LTV × Conversion.

---

### Quando Usar A/B Testing

**✅ Tem tráfego suficiente (1.000+ visitors/mês)**

**✅ Produto self-service (não sales-led)**

**✅ Quer dados objetivos, não opiniões**

---

## Metodologia 6: Análise de Competidores

### Conceito

**Ver quanto competidores cobram = proxy de WTP de mercado.**

---

### Como Fazer

**Passo 1:** Identificar 5-10 competidores diretos.

**Passo 2:** Coletar pricing:
- Website público
- Mystery shopping (fingir ser prospect, pedir quote)
- G2/Capterra reviews (clientes mencionam preços)

**Passo 3:** Criar tabela comparativa:

| Competidor | Tier Básico | Tier Pro | Enterprise | Value Metric |
|------------|-------------|----------|------------|--------------|
| Comp A | R$99/mês | R$499/mês | Custom | Per-user |
| Comp B | R$149/mês | R$599/mês | R$2k/mês | Per-user |
| Comp C | Freemium | R$399/mês | Custom | Usage-based |
| **Você** | ? | ? | ? | ? |

---

**Passo 4:** Análise de positioning:

**Se competidores cobram R$100-R$200:**
- Você pode cobrar R$150 (parity)
- Ou R$99 (value/disruptor)
- Ou R$250 (premium, se justificar)

**WTP de mercado está no range R$100-R$250.**

---

### Limitações

**❌ Competidor pode estar precificando errado**
- Só porque todos cobram R$100 não significa que é o ótimo

**❌ Seu produto pode ser diferente**
- Mais valor = pode cobrar mais
- Menos valor = precisa cobrar menos

**❌ Pricing público pode não ser real**
- Descontos, negociações

---

### Quando Usar

**✅ Mercado estabelecido (não novo)**

**✅ Validação rápida (sanity check)**

**✅ Complementar a outras metodologias**

---

## Metodologia 7: Análise de Cohorts (Dados Internos)

### Conceito

**Se você já tem clientes, analisar quais pagam mais/menos.**

---

### Como Fazer

**Segmentar clientes por:**
1. **Indústria** (fintech, SaaS, e-commerce, etc.)
2. **Tamanho** (1-10 pessoas, 10-50, 50-200, 200+)
3. **Região** (Brasil, EUA, Europa)
4. **Use case** (vendas, marketing, suporte)

**Analisar:**
- ACV médio por segmento
- Churn rate por segmento
- NPS por segmento

---

### Exemplo de Insights

**Análise:**

| Segmento | ACV Médio | Churn/Ano | NPS |
|----------|-----------|-----------|-----|
| Fintech (50-200 people) | R$8k/mês | 10% | 65 |
| E-commerce (10-50 people) | R$2k/mês | 30% | 45 |
| SaaS (10-50 people) | R$3k/mês | 15% | 70 |

**Insights:**
1. **Fintech tem WTP 4x maior que e-commerce**
   - Considerar tier premium para fintech
   - Ou verticalization

2. **E-commerce tem churn altíssimo (30%)**
   - Ou preço é muito alto para valor entregue
   - Ou não é bom fit
   - Considerar reduzir preço OU parar de focar nesse vertical

3. **SaaS tem NPS alto (70) e ACV médio**
   - Sweet spot
   - Dobrar down nesse segmento

---

### Vantagens

**✅ Dados reais, não hipotéticos**

**✅ Revela segmentação natural**

**✅ Identifica oportunidades**
- Quais segmentos pagariam mais

---

### Quando Usar

**✅ Já tem base de clientes (50+)**

**✅ Quer otimizar pricing por segmento**

---

## Combinando Metodologias

**Nenhuma metodologia sozinha é perfeita.**

**Recomendação: Usar 2-3 metodologias complementares.**

---

### Framework Completo de Pricing Research

**Fase 1: Qualitativo (Entender)**
- **Customer interviews** (10-20): Descobrir valor, contexto
- **Win/Loss analysis** (20-30): Objeções reais

**Fase 2: Quantitativo (Validar)**
- **Van Westendorp** (200+ respondentes): Range de preços
- Ou **Conjoint Analysis** (200+): Valor de features

**Fase 3: Competitivo (Benchmark)**
- **Análise de competidores**: Pricing de mercado

**Fase 4: Teste (Otimizar)**
- **A/B testing**: Testar preços finalistas
- **Cohort analysis**: Ajustar por segmento

---

### Exemplo de Timeline

**Semana 1-2:** Customer interviews (15 entrevistas)
- Output: Valor econômico estimado, range inicial de WTP

**Semana 3:** Van Westendorp survey (300 respondentes)
- Output: OPP = R$350-R$450/mês

**Semana 4:** Análise competitiva
- Output: Mercado cobra R$300-R$600

**Semana 5:** Definir preços finalistas
- Opção A: R$349/mês
- Opção B: R$399/mês

**Semana 6-8:** A/B test (se tiver tráfego)
- Output: R$399 gera +15% revenue/visitor → Escolher R$399

---

## Erros Comuns em Pricing Research

### Erro 1: Perguntar Preço Diretamente

**Pergunta ruim:**
```
"Quanto você pagaria por nosso produto?"
```

**Por que é ruim:** Cliente vai chutar baixo (quer deal).

**Solução:** Perguntar valor econômico, trade-offs, comparações.

---

### Erro 2: Survey com Amostra Pequena

**Exemplo:** 20 respondentes para Van Westendorp.

**Problema:** Não é estatisticamente significativo.

**Solução:** Mínimo 100-200 respondentes.

---

### Erro 3: Só Ouvir Early Adopters

**Problema:** Early adopters têm WTP diferente de mainstream.

**Early adopters:**
- Pagam premium por novidade
- Toleram bugs
- WTP alto

**Mainstream:**
- Price-sensitive
- Quer produto maduro
- WTP menor

**Solução:** Segmentar pesquisa por tipo de cliente.

---

### Erro 4: Ignorar Contexto Competitivo

**Exemplo:** Van Westendorp diz WTP é R$500, mas competidor cobra R$200.

**Problema:** Cliente vai escolher competidor.

**Solução:** Considerar alternativas, posicionamento.

---

### Erro 5: Não Testar (Só Pesquisar)

**Problema:** Pesquisa é hipotética. Teste é real.

**Exemplo:**
- Survey: "Pagaria R$500"
- Na hora de comprar: "R$500 é caro, vou pensar"

**Solução:** Sempre validar com dados reais (A/B test, deals reais).

---

## Checklist de Pricing Research

**Antes de definir preços, você deve:**

- [ ] **Falou com 10+ clientes** sobre valor, problemas, alternativas?
- [ ] **Quantificou valor econômico** criado para cliente?
- [ ] **Rodou Van Westendorp** ou Conjoint com 100+ respondentes?
- [ ] **Analisou pricing de 5+ competidores** diretos?
- [ ] **Fez Win/Loss analysis** de deals recentes?
- [ ] **Segmentou WTP** por persona/indústria/tamanho?
- [ ] **Testou preços** com dados reais (se possível)?

**Se respondeu SIM para 5+: Você tem base sólida para pricing.**

**Se respondeu NÃO para maioria: Precisa de mais research.**

---

## Ferramentas para Pricing Research

### Van Westendorp / Surveys
- **Google Forms** (grátis)
- **Typeform** (UI melhor)
- **Qualtrics** (enterprise, caro)
- **SurveyMonkey** (mid-tier)

### Conjoint Analysis
- **Conjointly** (R$500-R$2k, acessível)
- **Qualtrics** (enterprise)
- **Sawtooth Software** (especializado, caro)

### A/B Testing
- **Google Optimize** (descontinuado, mas alternativas)
- **Optimizely** (enterprise)
- **VWO** (mid-market)
- **Custom** (implementar próprio A/B test)

### Win/Loss Interviews
- **Clozd** (plataforma dedicada, cara)
- **Gong** (conversation intelligence)
- **Manual** (fazer entrevistas você mesmo)

---

## Conclusão: Recomendações por Estágio

### Early-Stage (Pré-Product-Market Fit)

**Metodologias:**
1. **Customer interviews** (10-20)
2. **Van Westendorp** (100-200 respondentes)
3. **Competitor analysis**

**Output:** Range inicial de WTP, preços para testar.

---

### Growth-Stage (Post-PMF, Escalando)

**Metodologias:**
1. **Van Westendorp** ou **Conjoint** (500+ respondentes)
2. **Win/Loss analysis** (ongoing)
3. **A/B testing** (contínuo)
4. **Cohort analysis** (por segmento)

**Output:** Pricing otimizado por segmento, evidência para aumentar preços.

---

### Mature (Liderança de Mercado)

**Metodologias:**
1. **Conjoint analysis** (para mudanças grandes)
2. **Cohort analysis** (ongoing)
3. **Competitive intelligence** (monitoring)
4. **Customer advisory board** (insights qualitativos)

**Output:** Ajustes finos, pricing de novos produtos/tiers.

---

**Próximo arquivo:** `tier-structure-guide.md` (como estruturar tiers: quantos, quais features, naming, Good-Better-Best, packaging)