# 📊 Bank Loan SQL Script Readme

A full exploratory data analysis (EDA) using SQL to uncover trends in bank loan performance, repayment behavior, and borrower characteristics. This project is visualized using Tableau and built for business and financial analysis use cases.

---

## 🧠 Domain Knowledge

Bank loans are vital financial products for both individuals and businesses. Understanding loan data helps institutions manage risk, improve approval accuracy, and optimize profitability.

**Key stages of the loan lifecycle:**
- Application submission (online or paper)
- Identity, income, credit, and employment verification
- DTI (Debt-to-Income) assessment
- Collateral evaluation (if applicable)
- Risk-based loan decisioning
- Agreement, disbursement, and repayment
- Ongoing monitoring & compliance

**Why banks analyze loan data:**
- Risk assessment & fraud detection
- Creditworthiness scoring
- Regulatory compliance (e.g. KYC, HMDA)
- Loan portfolio optimization
- Customer segmentation & product targeting
- Profitability forecasting

---

## 🗃️ Dataset Summary

- Source: Simulated financial data
- Total Records: 38,576
- Year: 2021
- Format: Relational table
- Tool: SQL Server

**Fields used:**  
`id`, `loan_amount`, `total_payment`, `term`, `int_rate`, `dti`, `loan_status`, `emp_length`, `purpose`, `home_ownership`, `issue_date`, `grade`, `sub_grade`

---

## 📌 Key Metrics & Results

### Loan Applications
- Total applications: 38,576
- Month-to-date (MTD): 4,314
- Previous MTD: 4,035
- Month-over-month (MoM) growth: +6.9%

### Funded Amounts
- Total funded: $435,857,570
- MTD funded: $53,981,425
- Previous MTD funded: $47,754,825
- MoM growth: +13.0%

### Amount Received
- Total received: $473,070,933
- MTD received: $58,074,380
- Previous MTD received: $50,132,030
- MoM growth: +15.8%

### Interest Rate & DTI
- Average interest rate: 12.05%
- MTD interest rate: 12.36%
- Previous MTD: 11.94%

- Average DTI: 13.33%
- MTD DTI: 13.67%
- Previous MTD: 13.30%

---

## 🟢 Good Loans vs 🔴 Bad Loans

**Good Loans (Fully Paid or Current):**
- 33,243 loans
- 86.2% of total
- Funded: $370,224,850
- Amount received: $435,786,170

**Bad Loans (Charged Off):**
- 5,333 loans
- 13.8% of total
- Funded: $65,532,225
- Amount received: $37,284,763

---

## 📋 Loan Status Breakdown

**Fully Paid**
- Loan count: 32,145
- Funded: $351,358,350
- Received: $411,586,256
- Interest rate: 11.64%
- DTI: 13.17%

**Charged Off**
- Loan count: 5,333
- Funded: $65,532,225
- Received: $37,284,763
- Interest rate: 13.88%
- DTI: 14.00%

**Current**
- Loan count: 1,098
- Funded: $18,866,500
- Received: $24,199,914
- Interest rate: 15.10%
- DTI: 14.72%

---

## 📆 Monthly Trends (Applications by Month)

- December: 4,314 apps — highest volume
- November: 4,035 apps
- Strong loan activity in Q4
- Gradual increase from Q1 to Q4
- Steady growth in funded and received amounts

---

## 🗺️ Applications by State (Top States)

- California: 6,894 apps
- New York: 3,701 apps
- Florida: 3,128 apps
- Texas: 2,773 apps
- Illinois: 1,486 apps

---

## ⏱️ Term Breakdown

**36 months**
- Applications: 28,237
- Funded: $273M
- Received: $294.7M

**60 months**
- Applications: 10,339
- Funded: $162.7M
- Received: $178.3M

---

## 🧍 Employment Length

- 10+ years: 8,870 apps — strongest performing segment
- <1 year: 4,575 apps
- 3 years: 4,088 apps
- 1 year: 3,229 apps

---

## 🏠 Home Ownership Status

- Renters: 18,439 apps
- Mortgage holders: 17,198 apps
- Owners: 2,838 apps

---

## 🎯 Loan Purpose Breakdown

- Debt consolidation: 18,214 apps — most common
- Credit card refinancing: 4,998 apps
- Home improvement: 2,876 apps
- Small business: 1,776 apps
- Other: 3,824 apps
## 📈 Key Business Insights

This section highlights the **underlying behavioral patterns, borrower profiles, and lending trends** extracted from the dataset. These insights go beyond KPI metrics and offer a story about when, where, and why customers borrow—and how lenders can respond intelligently.

### 1. Geographic Distribution
- California dominates loan applications (6.8k+), followed by NY, FL, TX, and GA.
- These high-volume states drive a large percentage of lending activity.
- Ideal for launching geo-targeted lending campaigns and adjusting underwriting thresholds regionally.

### 2. Seasonal Patterns
- Loan activity builds steadily from Q1 to Q4.
- December has the highest application, funding, and repayment volumes—likely due to holiday spending and debt restructuring.
- January through March represents a “quiet period” for lending cycles.

### 3. Employment Tenure & Trust
- 10+ year employed borrowers represent the **largest and most reliable** segment.
- <1 year borrowers also show high volume, suggesting growing credit access among early-tenure employees.
- 6–9 year tenure buckets are underrepresented, and may require product re-alignment or segmentation.

### 4. Loan Purpose Demand
- Debt consolidation is the #1 reason (~18.2k apps), signaling high consumer debt burdens.
- Credit card, home improvement, and small business loans round out the top 5.
- These should guide the creation of bundled or niche lending products.

### 5. Term Preferences
- 36-month loans dominate (73.2%), while 60-month loans are fewer but involve larger amounts.
- Shorter terms show better repayment efficiency, aligning with lender risk mitigation goals.

### 6. Homeownership Breakdown
- Renters submit the most applications (~18.4k), but mortgage holders show the highest repayment totals.
- Fully owned homes (no mortgage) are underrepresented, suggesting lower borrowing needs or risk-aversion.

---

## 🧩 Solutions Implementation

These insights translate into **actionable, real-world strategies** that banks or financial institutions could realistically implement. Each insight corresponds with practical lending, marketing, or operational moves.

### 1. Regional Targeting
- Prioritize underwriting and marketing in CA, NY, FL, TX, and NJ.
- Create **state-specific offers**, adjusting risk scores based on regional repayment behavior.

### 2. Seasonal Loan Strategies
- Deploy **holiday-timed loan campaigns** from September through December.
- Add pre-approval flows, reduced documentation, or bundled refinancing packages during Q4.
- Optimize staffing and loan servicing capacity around seasonal spikes.

### 3. Employment-Based Segmentation
- Offer **fast-track approval** or discounted rates to 10+ year employees.
- Launch **“Starter Credit” products** for <1 year borrowers with flexible repayment structures.
- Investigate drop-off in 6–9 year applicants to uncover hidden friction or exclusion criteria.

### 4. Product Strategy by Purpose
- Debt Consolidation: Introduce **consolidation bundles** with lower blended interest rates.
- Credit Card: Provide **targeted balance transfers** with fixed payoff dates.
- Small Business: Offer **limited-purpose microloans** with short cycles and optional coaching.

### 5. Term-Based Lending Models
- Promote 36-month loans as the **default product**.
- Use dynamic DTI + income scoring to gate eligibility for 60-month loans.
- Offer early payoff incentives to improve cash inflow and reduce long-term risk.

### 6. Homeownership Lifecycle Strategy
- Offer **first-time buyer prep loans** to renters to build credit history.
- Cross-sell **refinance or remodel packages** to mortgage holders.
- For homeowners (own outright), offer tax-advantaged HELOC-style lines of credit.

---
---

## 📊 Tableau Dashboard

Interactive dashboard visualizes:
- Summary KPIs
- Loan performance breakdowns
- Time-series and geographic trends
- Drill-down details

**📎 View Dashboard Here:**  
🔗 [Bank Loan Tableau Dashboard](https://public.tableau.com/app/profile/daniel.groza8136/viz/BankLoanReport_17573909988010/DETAILS?publish=yes)

**Dashboard Pages:**
- **Summary**: KPIs, good vs bad loans, loan status
- **Overview**: Monthly, geo, term, purpose, homeownership
- **Details**: Record-level table with filters

---

## 🧰 Tools Used

- SQL Server (T-SQL)
- Tableau Public
- GitHub
- Excel (optional for export formatting)

---

## 🚀 How to Use This Project

- Explore SQL logic in this repository
- Visit the Tableau dashboard to interact with visuals
- Apply filters by grade, purpose, term, verification status
- Use this project as a BI case study for financial lending data

---

## 👨‍💻 About Me

**Daniel Groza**  
Business & Data Analyst  
📍 Based in Charlotte, NC  
🎓 B.S. in Business Analytics, International Business, and Spanish  
🔧 Certified: Google, Microsoft, Tableau, IBM  
📁 Building multi-sector dashboards for BI & analytics

**GitHub**: [https://github.com/dgroza07/SQL-Portfolio-Projects](https://github.com/dgroza07/SQL-Portfolio-Projects)  
**LinkedIn**: [https://www.linkedin.com/in/daniel-c-groza/](https://www.linkedin.com/in/daniel-c-groza/)  
**Tableau**: [Bank Loan Dashboard](https://public.tableau.com/app/profile/daniel.groza8136/viz/BankLoanReport_17573909988010/DETAILS?publish=yes)

---

