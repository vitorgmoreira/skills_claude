# Psicologia de Precificação para SaaS

Guia completo sobre táticas psicológicas de pricing: anchoring, charm pricing, framing, decoy pricing, loss aversion e outras técnicas comportamentais.

---

## Por Que Psicologia Importa em Pricing

**Decisões de compra não são puramente racionais.**

**Humanos usam atalhos mentais (heurísticas) para decidir.**

**Pricing que entende psicologia converte melhor.**

---

## 1. Anchoring (Ancoragem)

### Conceito

**O primeiro número que cliente vê "ancora" sua percepção de valor.**

**Todos os preços subsequentes são comparados a essa âncora.**

---

### Como Funciona

**Estudo clássico (Dan Ariely):**
1. Mostrar número aleatório (ex: últimos 2 dígitos do CPF)
2. Perguntar: "Você pagaria esse valor por X?"
3. Depois perguntar: "Quanto você pagaria?"

**Resultado:** Pessoas com CPF terminando em número alto (ex: 87) ofereceram 2-3x mais que pessoas com número baixo (ex: 12).

**Conclusão:** Primeiro número ancora tudo.

---

### Aplicações em SaaS Pricing

#### Tática 1: Mostrar Tier Mais Caro Primeiro

**Ordem tradicional (esquerda → direita):**
```
[ Basic ]  →  [ Pro ]  →  [ Enterprise ]
  R$99         R$499        R$2.499
```

**Ordem com anchoring (direita → esquerda):**
```
[ Enterprise ]  →  [ Pro ]  →  [ Basic ]
   R$2.499          R$499       R$99
```

**Ou verticalmente:**
```
[ Enterprise - R$2.499 ]  ← Âncora
[ Pro - R$499 ]          ← Parece "razoável"
[ Basic - R$99 ]         ← Parece "barato"
```

**Efeito:** Pro (R$499) parece barato comparado a R$2.499.

---

#### Tática 2: Incluir Tier "Aspiracional" Caro

**Objetivo:** Não é vender esse tier. É ancorar percepção.

**Exemplo:**

```
[ Starter - R$99/mês ]
[ Pro - R$499/mês ]      ← Tier que você quer vender
[ Premium - R$2.499/mês ] ← Âncora (poucos compram)
```

**Efeito:** R$499 parece "médio" e razoável.

**Sem a âncora:**
```
[ Starter - R$99/mês ]
[ Pro - R$499/mês ]      ← Parece caro (5x o básico!)
```

---

#### Tática 3: Preço Anual como Âncora

**Mostrar preço anual primeiro, depois mensal.**

**Exemplo:**

```
R$4.999/ano
ou apenas R$419/mês
```

**Efeito:** R$419/mês parece pequeno comparado a R$4.999.

**Vs. mostrar mensal primeiro:**
```
R$419/mês
ou R$4.999/ano
```

**Parece mais caro psicologicamente.**

---

#### Tática 4: Comparar com Custo de Alternativa

**Ancorar contra custo da alternativa.**

**Exemplo:**

**Sem anchoring:**
```
Nosso CRM: R$500/usuário/mês
```

**Com anchoring:**
```
Contratar SDR: R$8.000/mês
Nosso CRM que aumenta produtividade em 30%: R$500/mês
```

**Efeito:** R$500 parece barato vs. R$8.000.

---

### Exemplos Reais de Anchoring

#### Exemplo 1: Apple iPhone Pricing

**Lançamento típico:**
- iPhone Pro Max: R$9.000 (âncora)
- iPhone Pro: R$7.500
- iPhone regular: R$5.500 ← Maioria compra
- iPhone SE: R$3.000

**Sem Pro Max (R$9k):**
- iPhone Pro (R$7.5k) pareceria caríssimo

**Com Pro Max:**
- iPhone regular (R$5.5k) parece "razoável"

#### Exemplo 2: Basecamp - Preço Flat

**Pricing:**
```
R$499/mês - FLAT
(Ilimitado usuários, projetos, tudo)
```

**Anchoring implícito:**
- Competidores cobram R$X/usuário
- Para 50 usuários: R$2.500-R$5.000/mês
- **R$499 flat parece MUITO barato**

**Basecamp usa competidores como âncora.**

---

## 2. Charm Pricing (Preço Psicológico)

### Conceito

**Terminar preços em 9, 7, ou 5 em vez de números redondos.**

**Exemplos:**
- R$99 em vez de R$100
- R$497 em vez de R$500
- R$2.999 em vez de R$3.000

---

### Por Que Funciona

#### Teoria 1: Left-Digit Effect

**Cérebro processa primeiro dígito da esquerda.**

**R$99 vs. R$100:**
- R$99: Cérebro processa "90-alguma coisa"
- R$100: Cérebro processa "100"
- **Percepção: R$99 está na faixa dos R$90, não R$100**

**Diferença de apenas R$1, mas psicologicamente "uma faixa abaixo".**

#### Teoria 2: Sinalização de Desconto

**Preços em .99 ou .97 sinalizam "deal", "promoção".**

**Preços redondos (R$100) sinalizam "premium", "qualidade".**

---

### Aplicações em SaaS

#### Quando Usar Charm Pricing

**✅ Target é SMB, price-sensitive**
- R$99/mês em vez de R$100
- Sinaliza value for money

**✅ Tier mais baixo (Starter)**
- R$99 parece acessível
- R$100 parece "três dígitos" (barreira psicológica)

**✅ Produto é self-service, volume**
- Converte melhor em landing pages
- A/B tests mostram +5-10% conversion

#### Quando NÃO Usar (Preços Redondos)

**❌ Target é Enterprise**
- R$10.000/mês é mais profissional que R$9.997/mês
- Charm pricing pode parecer "barato", "amador"

**❌ Produto premium, high-end**
- Apple cobra US$1.999 (não US$1.997)
- Sinaliza qualidade, não desconto

**❌ Pricing é custom/negociado**
- Ninguém negocia para R$9.997/mês
- Fica ridículo

---

### A/B Tests de Charm Pricing

**Estudo 1: E-commerce**
- Preço A: US$20
- Preço B: US$19
- **Resultado:** +24% de vendas em US$19

**Estudo 2: SaaS (Price Intelligently)**
- R$100/mês vs. R$99/mês
- **Resultado:** +8% conversion em R$99

**Mas:** Efeito menor em B2B enterprise (diferença de 2-3%).

---

### Variações de Charm Pricing

#### Opção 1: .99 (Mais Comum)

**Exemplos:**
- R$99/mês
- R$499/mês
- R$999/mês

**Percepção:** Desconto, value.

#### Opção 2: .97 (Desconto Maior)

**Exemplos:**
- R$97/mês
- R$497/mês

**Percepção:** Promoção ativa, deal.

**Uso:** Preços promocionais, limited-time offers.

#### Opção 3: .95 (Meio-Termo)

**Exemplos:**
- R$95/mês
- R$495/mês

**Menos comum em SaaS, mais em e-commerce.**

#### Opção 4: Números Redondos (Premium)

**Exemplos:**
- R$100/mês
- R$500/mês
- R$5.000/mês

**Percepção:** Premium, qualidade, profissional.

**Uso:** Enterprise, luxury SaaS.

---

## 3. Decoy Pricing (Efeito Isca)

### Conceito

**Adicionar opção "isca" para fazer outro tier parecer melhor.**

**Isca tem custo/benefício ruim de propósito.**

---

### Como Funciona (Estudo The Economist)

**Teste original:**

**Opção A (sem decoy):**
```
[ Digital: US$59/ano ]
[ Print + Digital: US$125/ano ]
```

**Resultado:** 68% escolheram Digital, 32% Print+Digital.

**Opção B (com decoy):**
```
[ Digital: US$59/ano ]
[ Print: US$125/ano ]           ← DECOY (isca ruim)
[ Print + Digital: US$125/ano ] ← Target
```

**Resultado:** 16% Digital, 0% Print, **84% Print+Digital**.

**Conclusão:** Decoy (Print por US$125) fez Print+Digital parecer incrível (mesmo preço, mais valor).

---

### Aplicações em SaaS

#### Tática 1: Tier Intermediário como Decoy

**Estrutura:**

```
[ Starter: R$99/mês ]
  - 5 usuários
  - Features básicas

[ Pro: R$299/mês ]              ← DECOY
  - 10 usuários
  - Features avançadas

[ Business: R$399/mês ]         ← TARGET
  - 50 usuários
  - Tudo do Pro + Admin + API
```

**Análise:**
- Starter → Pro: +R$200 para +5 usuários
- Pro → Business: +R$100 para +40 usuários + features enterprise

**Business é OBVIAMENTE melhor valor que Pro.**

**Efeito:** Maioria escolhe Business (não Pro).

---

#### Tática 2: Tier Anual vs. Mensal como Decoy

**Estrutura:**

```
[ Mensal: R$50/mês ]            ← DECOY
  = R$600/ano

[ Anual: R$499/ano ]            ← TARGET
  Economize R$101/ano!
```

**Mensal serve de decoy para anual parecer deal incrível.**

---

### Exemplos Reais

#### Exemplo 1: Apple iCloud Storage

```
[ 50GB: R$4/mês ]
[ 200GB: R$14/mês ]   ← DECOY
[ 2TB: R$40/mês ]     ← TARGET
```

**Análise:**
- 50GB → 200GB: +R$10 para +150GB (R$0.07/GB)
- 200GB → 2TB: +R$26 para +1.800GB (R$0.01/GB)

**2TB é valor absurdo comparado a 200GB.**

**Resultado:** Maioria que precisa de mais que 50GB pula direto para 2TB.

#### Exemplo 2: Zoom Pricing

```
[ Basic: Grátis ]
  40min meetings

[ Pro: R$75/mês ]     ← DECOY
  Meetings ilimitados
  1 host

[ Business: R$100/mês ] ← TARGET
  Meetings ilimitados
  10+ hosts
  Admin features
```

**Business é só R$25 a mais, mas com muito mais valor.**

---

### Quando Usar Decoy Pricing

**✅ Você quer empurrar clientes para tier específico**

**✅ Tier target tem valor muito melhor (mas cliente não percebe sem comparação)**

**✅ 3+ tiers (precisa de espaço para decoy)**

---

### Cuidados com Decoy

**❌ Não fazer decoy MUITO óbvio**
- Cliente pode perceber manipulação
- Perde confiança

**❌ Não prejudicar marca**
- Se todo mundo escolhe Tier A, e ninguém escolhe Tier B (decoy), considerar remover Tier B
- Ter tier que ninguém compra parece ruim

---

## 4. Price Framing (Enquadramento de Preço)

### Conceito

**Maneira como você apresenta o preço influencia percepção.**

**Mesmo preço, framing diferente, percepção diferente.**

---

### Tática 1: Breakdown (Divisão)

**Quebrar preço grande em pedaços pequenos.**

**Exemplo 1:**

**Sem framing:**
```
R$1.200/ano
```

**Com framing:**
```
Apenas R$3,30/dia
(menos que um café!)
```

**Efeito:** R$3,30/dia parece trivial. R$1.200 parece muito.

---

**Exemplo 2: Spotify**

```
R$21,90/mês

ou

R$0,73/dia - Menos que um café
```

**Framing diminui percepção de custo.**

---

**Exemplo 3: Gym Memberships**

**Academia cobra:**
```
R$150/mês

Framed como:
R$5/dia para sua saúde
```

---

### Tática 2: Comparação com Alternativa

**Comparar preço com custo de alternativa cara.**

**Exemplo:**

**Sem framing:**
```
Nosso CRM: R$300/mês
```

**Com framing:**
```
Contratar SDR adicional: R$8k/mês
ou
Nosso CRM que dobra sua produtividade: R$300/mês

Economize R$7.700/mês
```

---

**Exemplo 2: Zapier**

```
Automatização manual: 10 horas/mês × R$100/hora = R$1.000
Zapier: R$299/mês

Economize R$701/mês + seu tempo
```

---

### Tática 3: Desconto Percentual vs. Absoluto

**Regra:**
- **Valor baixo:** Mostrar desconto %
- **Valor alto:** Mostrar desconto R$

**Exemplo baixo (R$100):**

**Desconto de R$20:**
- ❌ "Economize R$20" (parece pouco)
- ✅ "Economize 20%!" (parece muito)

**Exemplo alto (R$10.000):**

**Desconto de R$2.000:**
- ✅ "Economize R$2.000" (WOW!)
- ❌ "Economize 20%" (meh)

---

### Tática 4: Annual Savings

**Enfatizar economia anual vs. mensal.**

**Exemplo:**

```
[ Mensal: R$50/mês ]

[ Anual: R$500/ano ]
Economize R$100/ano! ← 2 meses grátis
```

**Framing "R$100/ano" + "2 meses grátis" converte melhor que só mostrar preço.**

---

### Tática 5: Remove o Símbolo R$

**Estudos mostram que remover símbolo de moeda reduz "dor de pagar".**

**Restaurantes de luxo fazem isso:**
- ❌ R$ 150,00
- ✅ 150 (sem símbolo)

**Em SaaS:**

**Opção A:**
```
R$ 499 / mês
```

**Opção B:**
```
499 / mês
```

**Efeito pequeno, mas mensurável (+2-5% em alguns A/B tests).**

---

## 5. Loss Aversion (Aversão à Perda)

### Conceito

**Humanos sentem mais DOR de perder algo do que PRAZER de ganhar.**

**Perder R$100 dói 2x mais que ganhar R$100.**

---

### Aplicações em Pricing

#### Tática 1: Free Trial → Paid (Perder Acesso)

**Durante trial, cliente cria valor:**
- Documentos no Notion
- Dados no CRM
- Automações no Zapier

**Quando trial acaba:**
- "Você vai PERDER acesso a tudo que criou"
- **Loss aversion:** Cliente não quer perder

**Efeito:** Conversion rate alto (20-60% em trials).

---

#### Tática 2: "Continue usando" em vez de "Comece a pagar"

**Framing ruim:**
```
Trial acabou. Comece a pagar R$499/mês.
```

**Framing bom:**
```
Trial acabou. Continue usando [produto] por apenas R$499/mês.
```

**"Continue" evoca loss aversion (não perder o que já tem).**

---

#### Tática 3: Mostrar o Que Cliente Perde

**Email de fim de trial:**

**Versão A (fraca):**
```
Seu trial acabou. Upgrade para continuar.
```

**Versão B (loss aversion):**
```
Seu trial acabou.

Você vai perder acesso a:
- 47 documentos que você criou
- 12 integrações configuradas
- 89 tarefas automatizadas

Continue usando por R$299/mês
```

**Versão B converte 30-50% melhor.**

---

#### Tática 4: Countdown Timers (Urgência)

**Adicionar timer de trial:**

```
⏰ Restam 3 dias de trial

Após isso, você perderá acesso a:
[lista do que vai perder]
```

**Urgência + Loss aversion = Conversão.**

---

## 6. Social Proof (Prova Social)

### Conceito

**Humanos copiam comportamento de outros.**

**"Se outros compraram, deve ser bom."**

---

### Aplicações em Pricing

#### Tática 1: "Mais Popular" Badge

**Destacar tier que maioria compra.**

```
[ Starter ]    [✨ PRO - MAIS POPULAR ✨]    [ Enterprise ]
  R$99/mês              R$499/mês                Custom
```

**Efeito:** Clientes gravitam para "Popular".

**Aumento de 10-30% de escolha desse tier.**

---

#### Tática 2: Número de Clientes

**Mostrar quantos clientes usam o tier.**

```
[ Pro - R$499/mês ]
Escolhido por 10.000+ empresas
```

**Ou:**

```
[ Enterprise ]
Usado por 500 das Fortune 1000
```

**Social proof reduz risco percebido.**

---

#### Tática 3: Logos de Clientes

**Mostrar logos próximo ao pricing.**

```
Empresas que confiam em [Produto]:
[Logo Nubank] [Logo iFood] [Logo Stone]

[ Ver Planos ]
```

**Efeito:** "Se Nubank usa, deve ser bom."

---

#### Tática 4: Testimonials Específicos

**Incluir depoimento próximo a tier.**

```
[ Pro - R$499/mês ]

"Aumentamos vendas em 40% após usar [Produto]"
- João Silva, Head of Sales na XYZ Corp
```

**Social proof + resultado concreto.**

---

## 7. Scarcity (Escassez)

### Conceito

**Coisas escassas parecem mais valiosas.**

**"Limitado" aumenta desejo.**

---

### Aplicações (Cuidado: Uso Ético)

#### Tática 1: Limited-Time Discount

**Desconto temporário.**

```
50% OFF no primeiro ano
Apenas até 31/12

R$499/mês → R$249/mês
```

**IMPORTANTE: Precisa ser REAL. Deadline fake é anti-ético.**

---

#### Tática 2: Limited Spots (Para High-Touch)

**Para produtos com onboarding manual.**

```
Abrimos apenas 10 vagas por mês para onboarding dedicado.

9/10 vagas preenchidas este mês.
```

**Se for verdade, cria urgência.**

---

#### Tática 3: Early Adopter Pricing

```
Preço Early Adopter: R$299/mês
(Garantido para sempre)

Após lançamento oficial: R$499/mês
```

**Incentiva compra early, recompensa early adopters.**

---

### ⚠️ Cuidado com Fake Scarcity

**Exemplos ruins (anti-éticos):**
- "Apenas 2 licenças restantes!" (mas sempre tem)
- Countdown timer que reseta
- "Oferta termina em 1 hora" (mas nunca termina)

**Resultado:** Perde confiança, má reputação.

**Regra:** Só use scarcity se for REAL.

---

## 8. Reciprocity (Reciprocidade)

### Conceito

**Se você dá algo de graça, pessoa sente obrigação de retribuir.**

---

### Aplicações em SaaS

#### Tática 1: Free Tier Generoso

**Dar muito valor de graça.**

**Exemplo: Notion**
- Free tier é 90% do produto
- Cliente cria valor massivo (stored value)
- Sente obrigação de pagar quando empresa cresce

**Reciprocidade + Loss aversion.**

---

#### Tática 2: Free Tools/Resources

**Dar ferramentas grátis, depois vender produto.**

**Exemplo: HubSpot**
- Website Grader (grátis)
- Free CRM (grátis)
- Blogs, cursos (grátis)

**Cliente recebe valor → Reciprocidade → Compra produto pago.**

---

#### Tática 3: Free Trial Sem Cartão

**Trial sem compromisso.**

**Cliente pensa:**
- "Eles me deram 30 dias grátis, sem pedir cartão"
- "Isso é generoso"
- Reciprocidade → Maior chance de converter

---

## 9. Price Bundling (Pacote)

### Conceito

**Vender múltiplos itens juntos por preço menor que soma individual.**

---

### Quando Funciona

#### ✅ Produtos Complementares

**Exemplo: Microsoft Office**
- Word separado: R$200
- Excel separado: R$200
- PowerPoint separado: R$200
- **Office Bundle: R$400** (economize R$200)

---

#### ✅ Aumentar Perceived Value

**Bundle parece "deal".**

**Exemplo em SaaS:**

**Sem bundle:**
```
CRM: R$300/mês
Email marketing: R$200/mês
Analytics: R$150/mês
Total: R$650/mês
```

**Com bundle:**
```
Suite completa: R$499/mês
Economize R$151/mês!
```

---

### Tipos de Bundling

#### 1. Pure Bundling (Só Vende Bundle)

**Não pode comprar produtos separados.**

**Exemplo:** Cable TV (tem que comprar pacote, não canais individuais).

**Em SaaS:** Raro (clientes querem flexibilidade).

---

#### 2. Mixed Bundling (Bundle + Produtos Separados)

**Pode comprar bundle OU produtos individuais.**

**Exemplo: HubSpot**
```
Marketing Hub: R$2k/mês
Sales Hub: R$2k/mês
Service Hub: R$2k/mês

ou

Growth Suite (3 produtos): R$5k/mês
Economize R$1k/mês
```

---

### Vantagens de Bundling

**✅ Aumenta ACV (Average Contract Value)**
- Cliente compra mais por bundle deal

**✅ Reduz Churn**
- Switching cost maior (usa 3 produtos, não 1)

**✅ Perceived Value**
- "Economizei R$150!" (mesmo que não usaria todos os produtos)

---

### Desvantagens

**❌ Pode Cannibalizar Revenue**
- Cliente que pagaria R$650 agora paga R$499

**❌ Cliente Pode Não Usar Tudo**
- Compra bundle, usa 1 de 3 produtos
- Percebe que desperdiçou
- Churn

---

## 10. Endowment Effect (Efeito Dotação)

### Conceito

**Pessoas valorizam mais o que já possuem.**

**"Meu carro vale mais que carros idênticos no mercado."**

---

### Aplicações em SaaS

#### Tática 1: Free Trial Cria Ownership

**Durante trial, cliente "possui" o produto.**

**Quando trial acaba:**
- Cliente não quer "perder" o produto
- Endowment effect + loss aversion

---

#### Tática 2: Default Settings

**Features ativadas por default.**

**Exemplo:**
- Todos os planos vêm com "Advanced analytics" ativado no trial
- Cliente se acostuma
- Quando vê que precisa pagar para manter: Endowment effect

**Mais provável de pagar para não perder.**

---

## 11. Partitioned Pricing (Preço Fragmentado)

### Conceito

**Dividir preço em partes (base + add-ons).**

**Exemplo:**
```
Base: R$300/mês
+ Usuários extras: R$50/usuário
+ Storage adicional: R$20/100GB
Total: R$450/mês
```

---

### Quando Funciona

**✅ Base price parece baixo**
- Cliente vê "R$300/mês"
- Esquece dos add-ons
- Conta final: R$450

**✅ Cliente sente controle**
- "Escolho o que quero pagar"

---

### Quando NÃO Funciona

**❌ Bill shock**
- Cliente esperava R$300
- Recebe conta de R$450
- Churn

**❌ Complexidade**
- Muitos add-ons = confusão

---

## 12. Round Numbers vs. Precise Numbers

### Conceito

**Números redondos (R$500) vs. precisos (R$487).**

---

### Quando Usar Cada Um

#### Round Numbers (R$500)

**✅ Decisões emocionais**
- Produtos de luxo
- Gifting
- "Parece certo"

---

#### Precise Numbers (R$487)

**✅ Decisões racionais**
- B2B
- Cliente está comparando alternativas
- Sinaliza que preço foi "calculado" (não arbitrário)

**Estudo:** Ofertas de imóveis com números precisos (ex: US$367.450) são mais aceitas que redondos (US$370.000).

**Razão:** Precisão sinaliza "eu sei o valor exato disso".

---

## 13. Pay What You Want (Experimental)

### Conceito

**Cliente escolhe quanto pagar.**

**Raro em SaaS, mas interessante.**

---

### Quando Pode Funcionar

**✅ Custo marginal zero**
- Digital products
- Conteúdo

**✅ Reciprocidade**
- Cliente sente obrigação de pagar "justo"

---

### Exemplos

#### Exemplo 1: Humble Bundle

- Pay what you want por bundle de games
- Média: US$7-10 (mesmo podendo pagar US$1)

#### Exemplo 2: Panera Bread (Experimento)

- Restaurante deixou clientes pagarem o que queriam
- Média foi 80% do preço normal

---

### Por Que Não Funciona em Maioria dos SaaS

**❌ Muitos pagariam $0**

**❌ Complexidade operacional**

**❌ Posicionamento confuso**
- "Se produto é bom, por que não tem preço fixo?"

---

## 14. Grandfathering (Proteger Preço Antigo)

### Conceito

**Quando você aumenta preços, clientes antigos mantêm preço velho.**

---

### Vantagens

**✅ Reduz churn de aumento de preço**

**✅ Recompensa lealdade**

**✅ Goodwill**

---

### Desvantagens

**❌ Complexidade operacional**
- Múltiplos preços ativos

**❌ Deixa revenue na mesa**
- Clientes antigos pagam menos

---

### Quando Usar

**Aumento grande (>30%):**
- Grandfather para evitar churn massivo

**Aumento pequeno (<15%):**
- Aplicar para todos (comunicar bem)

---

## 15. Decoy Effect com Billing Frequency

### Conceito

**Usar billing mensal como decoy para anual.**

---

### Estrutura

```
[ Mensal: R$50/mês ]
  = R$600/ano

[ Anual: R$500/ano ]  ← 17% de desconto
  (R$41.66/mês)
```

**Framing adicional:**
```
Economize R$100/ano!
ou
Ganhe 2 meses grátis!
```

---

### Por Que Funciona

**Mensal serve de âncora.**

**Cliente pensa:**
- "Se eu for ficar mais de 10 meses, anual compensa"
- Maioria fica >10 meses
- **Escolhe anual**

---

### Vantagens do Anual (para Vendor)

**✅ Cash flow upfront**

**✅ Churn menor**
- Commitment anual

**✅ CAC payback mais rápido**

---

## Checklist de Psicologia de Pricing

**Ao criar sua página de pricing, considerar:**

- [ ] **Anchoring:** Mostrar tier mais caro primeiro ou criar tier aspiracional?
- [ ] **Charm pricing:** Usar .99 para tiers SMB? Redondo para enterprise?
- [ ] **Decoy:** Há tier intermediário que serve de isca para tier target?
- [ ] **Framing:** Preço anual está enfatizado com savings?
- [ ] **Loss aversion:** Trial comunica o que cliente vai perder?
- [ ] **Social proof:** "Mais popular" badge? Logos? Testimonials?
- [ ] **Scarcity:** Alguma urgência real (deadline, limited spots)?
- [ ] **Bundling:** Há oportunidade de bundle com desconto?
- [ ] **Annual discount:** Desconto anual é suficiente (15-20%)?
- [ ] **Simplicidade:** Cliente consegue entender preços em <30 segundos?

---

## Combinando Múltiplas Táticas

**Exemplo de pricing page que usa 5+ táticas:**

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Escolhido por 10.000+ empresas               (Social Proof)
[Logo] [Logo] [Logo]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

┌────────────┐  ┌──────────────────┐  ┌──────────────┐
│  STARTER   │  │ ✨ PRO - POPULAR ✨ │  │  ENTERPRISE │  (Social Proof: Popular badge)
│            │  │                  │  │              │
│  R$ 99/mês │  │   R$ 499/mês    │  │  R$ 2.499/mês│  (Anchoring: Mais caro à direita)
│            │  │                  │  │              │
│ 5 usuários │  │  10 usuários    │  │  50 usuários │  (Decoy: Pro tem má relação custo/benefício)
│ Core       │  │  Core + Advanced│  │  Everything  │
└────────────┘  └──────────────────┘  └──────────────┘
                      ↑ DECOY                ↑ TARGET

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Pague anualmente e economize 20%!           (Framing: Savings)

Mensal: R$499/mês = R$5.988/ano
Anual:  R$4.788/ano (economize R$1.200!)    (Decoy: Mensal é isca para anual)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

"Aumentamos vendas em 35% no primeiro mês"  (Social Proof: Testimonial)
- Maria Santos, CEO da Startup XYZ

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

⏰ Oferta por tempo limitado: 50% OFF      (Scarcity - se for real!)
   Termina em: 3 dias

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**Resultado:** Combina 6 táticas psicológicas para maximizar conversão.

---

## Erros Comuns de Psicologia de Pricing

### Erro 1: Usar Todas as Táticas

**Problema:** Fica over-engineered, manipulativo.

**Cliente percebe:**
- Countdown timers falsos
- "Apenas 2 vagas" (mas sempre tem)
- Badges de "popular" em todos os tiers

**Resultado:** Perde confiança.

**Solução:** Escolher 2-3 táticas autênticas.

---

### Erro 2: Fake Scarcity

**Exemplo:** Timer que reseta todo dia.

**Resultado:** Cliente descobre, má reputação viral.

**Solução:** Só usar scarcity REAL.

---

### Erro 3: Complexidade Excessiva

**Exemplo:**
- 5 tiers
- 3 billing frequencies
- 10 add-ons opcionais
- Decoys múltiplos

**Resultado:** Paralisia de escolha, cliente desiste.

**Solução:** Simplicidade > clever tactics.

---

### Erro 4: Charm Pricing em Enterprise

**Exemplo:** Cobrar R$9.997/mês de enterprise.

**Problema:** Parece amador, não-profissional.

**Solução:** Redondo (R$10.000) para enterprise.

---

## Conclusão: Princípios-Chave

**1. Entenda Psicologia, Mas Não Manipule**
- Use táticas éticas
- Scarcity, urgência = OK se REAL
- Fake = Ruim

**2. Teste Tudo**
- A/B test charm pricing
- Test order de tiers
- Test framing de preço

**3. Simplicidade Vence Complexidade**
- Cliente deve entender em <30 segundos
- Se precisa de 5 minutos para explicar pricing: Simplifique

**4. Contexto Importa**
- SMB: Charm pricing, badges "popular"
- Enterprise: Preços redondos, profissional

**5. Combine 2-3 Táticas (Não Todas)**
- Anchoring + Social proof + Decoy: OK
- Todas as 15 táticas: Manipulativo

---

**Próximo arquivo:** `willingness-to-pay.md` (metodologias para descobrir quanto cliente pagaria: Van Westendorp, Conjoint Analysis, Win/Loss Analysis, entrevistas)