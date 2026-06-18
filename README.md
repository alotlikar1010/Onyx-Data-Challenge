# Onyx DataDNA Challenge June 2026
UK Fintech Neobank Digital Transaction Health Monitor Analytics Challenge

# Description
In this challenge, you will analyze a transactional dataset from a UK-based fintech neobank tracking customer activity, transaction performance, fraud exposure, and fee revenue across digital banking channels. The data spans individual transactions, customer profiles, transaction types, merchant categories, and supporting dimensions including regions, devices, channels, and KYC status. Your objective is to uncover revenue opportunities, identify fraud and operational risks, and detect customer behaviour patterns — helping Risk, Finance, Product, and Compliance teams improve transaction success rates, reduce revenue leakage, strengthen fraud controls, and enhance the overall customer experience through data-driven decisions.


# Dataset
https://datadna.onyxdata.co.uk/challenges/june-2026-datadna-uk-fintech-neobank-digital-transaction-health-monitor-analytics-challenge/

# Tools and Technology

## Power BI
- Data Modeling
  - Star schema
  - Fact and dimension relationships
  - Many-to-one cardinality

- DAX
  - Calculated measures
  - Calculated columns
  - FILTER, DIVIDE, COUNTROWS patterns

- Power Query
  - Data transformation
  - Null handling
  - Custom columns

- Data Visualization
  - Matrix reports
  - Filled maps
  - Conditional formatting
  - Multi-page report design


## Key Insights
# Executive Summary 
🔢 HEADLINE NUMBERS
Zephyr Bank processed 1,500 transactions worth £1.90M between 
January and May 2026. Total fee revenue collected was £750.17, 
against £587 in uncollected fees — meaning 44% of potential 
fee revenue was lost.

📊 CUSTOMER SEGMENTS
Standard segment leads transaction volume. Premium customers 
generate the highest total value but carry a disproportionate 
fraud exposure. Business segment produces the highest fee 
revenue per transaction despite lowest volume.

🗺️ REGIONAL ACTIVITY
London dominates transaction volume with 375 transactions — 
nearly double any other region. All fraud activity in the 
dataset is concentrated in London, making it the single 
highest-risk region for H1 2026.

🚨 TRANSACTION FAILURES
Only 15% of all transactions completed successfully. Declined 
transactions account for 35%, Reversed 25%, and Pending 25%. 
The leading failure reason is Insufficient Funds, followed 
equally by Card Limit Exceeded and Fraud Suspected.

💳 FRAUD EXPOSURE
20% of all transactions were flagged as fraudulent — 1 in every 
5 transactions. Fraud flags are entirely concentrated among 
KYC-verified Premium customers in the London region, which 
warrants an urgent risk investigation.

💸 FEE LEAKAGE
Transfer - International shows the largest gap between the 
standard fee (£2.50) and actual fee charged. ATM Withdrawals 
and Crypto Purchases follow. Total leakage of £587 across H1 
represents a significant and recoverable revenue gap for Finance.

─────────────────────────────────────────────────────────────
⚠️  TOP 3 ACTIONS FOR STAKEHOLDERS
1. RISK   → Investigate London-based Premium customer fraud 
            cluster immediately
2. FINANCE → Audit International Transfer fee application — 
            recover £400+ in leakage
3. PRODUCT → Address 85% non-completion rate — prioritise 
            Declined transaction UX fixes
   
