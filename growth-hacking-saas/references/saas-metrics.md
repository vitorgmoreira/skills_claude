# Métricas Essenciais para SaaS por Estágio

## Métricas por Estágio de Crescimento

### Early Stage (Pre-PMF, $0-$1M ARR)

**Foco: Validar Product-Market Fit**

#### Métricas Críticas:
1. **Retention Rate (Taxa de Retenção)**
   - D1, D7, D30, D90 retention
   - Meta: 40%+ no D30 indica PMF forte
   - Se usuários não voltam, não há PMF

2. **NPS (Net Promoter Score)**
   - "Qual a probabilidade de recomendar?" (0-10)
   - Promotores (9-10) - Detratores (0-6)
   - Meta: 50+ indica PMF

3. **Time to Value (TTV)**
   - Tempo até usuário ter primeira experiência de valor
   - Meta: Reduzir ao máximo (minutos, não dias)

4. **Activation Rate**
   - % de signups que completam ação-chave
   - Meta: 30%+ é bom

5. **Qualitative Feedback**
   - Entrevistas com usuários
   - Como reagiriam se produto sumisse?
   - "Muito desapontados" por 40%+ = PMF

#### Métricas Secundárias:
- MRR (Monthly Recurring Revenue)
- Logo retention (% de empresas que continuam)
- Feature adoption rate

---

### Growth Stage ($1M-$10M ARR)

**Foco: Escalar o que funciona**

#### Métricas Críticas:

1. **CAC (Customer Acquisition Cost)**
   ```
   CAC = Total Sales & Marketing Spend / New Customers
   ```
   - CAC por canal (orgânico, pago, referral, etc.)
   - Meta: LTV:CAC ratio de 3:1 ou melhor

2. **LTV (Lifetime Value)**
   ```
   LTV = ARPU × Gross Margin % / Churn Rate
   ```
   - Meta: LTV > 3x CAC

3. **CAC Payback Period**
   ```
   Meses = CAC / (MRR por cliente × Gross Margin %)
   ```
   - Meta: < 12 meses

4. **MRR Growth Rate**
   - % de crescimento MRR mês-a-mês
   - Benchmarks:
     - 15-20%/mês: Excelente (early stage)
     - 10-15%/mês: Muito bom
     - 5-10%/mês: Bom

5. **Churn Rate (Taxa de Cancelamento)**
   - **Logo Churn**: % de clientes que cancelam
     - Meta: < 5% ao mês (SaaS B2B)
     - Meta: < 7% ao mês (SaaS B2C)
   - **Revenue Churn**: % de MRR perdido
     - Pode ser negativo com expansão

6. **Magic Number**
   ```
   Magic Number = Net New ARR Q / Sales & Marketing Spend Q-1
   ```
   - < 0.5: Ineficiente, otimizar antes de escalar
   - 0.5-0.75: Ok para escalar
   - 0.75-1.0: Ótimo, acelerar investimento
   - > 1.0: Excepcional

#### Métricas Secundárias:

7. **Conversion Rates (Taxas de Conversão)**
   - Visitor → Signup: 5-10%
   - Signup → Active User: 30-40%
   - Trial → Paid: 15-25%
   - Free → Paid: 2-5%

8. **Lead Velocity Rate (LVR)**
   - % de crescimento em qualified leads mês-a-mês
   - Leading indicator de receita futura

9. **ARPU (Average Revenue Per User)**
   ```
   ARPU = MRR / Total Active Customers
   ```
   - Rastrear por cohort e segmento

10. **Quick Ratio**
    ```
    Quick Ratio = (New MRR + Expansion MRR) / (Churned MRR + Contraction MRR)
    ```
    - Meta: > 4 (crescimento saudável)

---

### Scale Stage ($10M+ ARR)

**Foco: Eficiência e previsibilidade**

#### Métricas Críticas:

1. **Rule of 40**
   ```
   Rule of 40 = Growth Rate % + Profit Margin %
   ```
   - Meta: ≥ 40%
   - Ex: 30% growth + 10% margin = 40%
   - Mostra equilíbrio entre crescimento e rentabilidade

2. **Net Revenue Retention (NRR)**
   ```
   NRR = (Starting ARR + Expansion - Churn - Contraction) / Starting ARR
   ```
   - Meta: > 100% (expansion > churn)
   - Benchmarks:
     - 120%+: Excepcional
     - 110-120%: Excelente
     - 100-110%: Bom
     - < 100%: Precisa melhorar

3. **Gross Revenue Retention (GRR)**
   ```
   GRR = (Starting ARR - Churn - Contraction) / Starting ARR
   ```
   - Meta: > 90%
   - GRR alto = base de clientes sólida

4. **Sales Efficiency (Magic Number)**
   - Consistência trimestre-a-trimestre
   - Previsibilidade de retorno em marketing

5. **LTV:CAC Ratio**
   - Meta: 3:1 a 5:1
   - < 3:1: Pouco eficiente
   - > 5:1: Sub-investindo em crescimento

#### Métricas Secundárias:

6. **Burn Multiple**
   ```
   Burn Multiple = Net Burn / Net New ARR
   ```
   - < 1.5: Eficiente
   - 1.5-2: Ok
   - > 2: Ineficiente

7. **ARR per Employee**
   - Benchmark: $150K-$200K+
   - Indicador de eficiência operacional

8. **Months of Runway**
   ```
   Runway = Cash / Monthly Burn Rate
   ```
   - Meta: 18+ meses

9. **Gross Margin**
   ```
   Gross Margin = (Revenue - COGS) / Revenue
   ```
   - Meta SaaS: 70-80%+
   - Inclui: hosting, support, onboarding

10. **Sales & Marketing % of Revenue**
    - Benchmark: 30-50% do revenue
    - Varia por estágio e estratégia

---

## Métricas por Área Funcional

### Aquisição

- **Traffic Sources**: Orgânico, Pago, Direto, Referral, Social
- **Cost per Click (CPC)**
- **Cost per Lead (CPL)**
- **Lead-to-MQL Rate**
- **MQL-to-SQL Rate**
- **Channel ROI**

### Ativação/Onboarding

- **Signup Completion Rate**
- **Email Verification Rate**
- **Onboarding Completion Rate**
- **Time to First Value**
- **Feature Adoption Rate**
- **% Users Reaching "Aha Moment"**

### Engajamento

- **DAU (Daily Active Users)**
- **MAU (Monthly Active Users)**
- **DAU/MAU Ratio (Stickiness)**
  - Meta: > 20%
- **Session Duration**
- **Session Frequency**
- **Feature Usage per User**

### Monetização

- **Trial-to-Paid Conversion Rate**
- **Free-to-Paid Conversion Rate**
- **Average Deal Size**
- **Sales Cycle Length**
- **Win Rate**
- **Expansion Rate**
- **Upsell/Cross-sell Rate**

### Retenção

- **Cohort Retention Curves**
- **Churn Reasons (categorizado)**
- **At-Risk Customer Score**
- **Product Engagement Score**
- **Customer Health Score**

### Referral

- **NPS (Net Promoter Score)**
- **Viral Coefficient (K-factor)**
  ```
  K = (# of invites per user) × (conversion rate of invites)
  ```
  - K > 1: Crescimento viral
- **% of Customers Referring**
- **Referral Revenue Contribution**

---

## Benchmarks por Modelo de SaaS

### B2B Enterprise SaaS
- **ACV (Annual Contract Value)**: $50K-$500K+
- **Sales Cycle**: 3-12 meses
- **CAC**: $10K-$100K+
- **Payback Period**: 12-24 meses
- **Gross Churn**: < 1% ao mês
- **NRR**: 120%+

### B2B SMB SaaS
- **ACV**: $1K-$25K
- **Sales Cycle**: 1-3 meses
- **CAC**: $500-$5K
- **Payback Period**: 6-12 meses
- **Gross Churn**: 3-5% ao mês
- **NRR**: 100-110%

### B2C SaaS
- **ARPU**: $10-$100/mês
- **Sales Cycle**: Self-service (minutos)
- **CAC**: $10-$200
- **Payback Period**: 3-6 meses
- **Gross Churn**: 5-7% ao mês
- **Modelo**: Freemium ou free trial

### PLG (Product-Led Growth) SaaS
- **Free-to-Paid Rate**: 2-5%
- **PQL-to-Paid**: 20-30%
- **Self-Service %**: 80%+
- **Sales-Assisted %**: 20%-
- **Viral Coefficient**: 0.5-1.0+

---

## Dashboard Essencial por Estágio

### Early Stage Dashboard
1. Signups (diário/semanal)
2. Active users
3. D7/D30 Retention
4. NPS
5. MRR

### Growth Stage Dashboard
1. MRR & Growth Rate
2. New MRR, Expansion, Churn, Net New
3. CAC por canal
4. LTV:CAC
5. Payback period
6. Magic Number
7. Churn rate
8. Conversion funnel

### Scale Stage Dashboard
1. ARR & Growth Rate
2. NRR & GRR
3. Rule of 40
4. Sales Efficiency (Magic Number)
5. Unit Economics (LTV:CAC, Payback)
6. Cohort retention curves
7. Cash & Runway
8. Gross Margin
9. ARR per employee

---

## Periodicidade de Análise

### Diário
- MRR
- Signups
- Active users
- Churn events

### Semanal
- Funnel conversion
- CAC por canal
- Feature adoption
- Customer health scores

### Mensal
- Cohort analysis
- NRR/GRR
- Magic Number
- Unit economics
- Channel ROI

### Trimestral
- Rule of 40
- Strategy review
- Goal setting
- Board metrics
