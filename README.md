# Onyx DataDNA Challenge June 2026
UK Fintech Neobank Digital Transaction Health Monitor Analytics Challenge

# Description
In this challenge, you will analyze a transactional dataset from a UK-based fintech neobank tracking customer activity, transaction performance, fraud exposure, and fee revenue across digital banking channels. The data spans individual transactions, customer profiles, transaction types, merchant categories, and supporting dimensions including regions, devices, channels, and KYC status. Your objective is to uncover revenue opportunities, identify fraud and operational risks, and detect customer behaviour patterns — helping Risk, Finance, Product, and Compliance teams improve transaction success rates, reduce revenue leakage, strengthen fraud controls, and enhance the overall customer experience through data-driven decisions.


# Dataset
https://datadna.onyxdata.co.uk/challenges/june-2026-datadna-uk-fintech-neobank-digital-transaction-health-monitor-analytics-challenge/

# Tools and Technology

## Power BI
- Data Modeling
- DAX
- Power Query
- Data Visualization

# Screenshot


## Key Insights
# Executive Summary 
🔢 HEADLINE NUMBERS
Zephyr Bank processed 1,500 transactions worth £1.90M between January and May 2026. Total fee revenue collected was £750.17, against £587 in uncollected fees — meaning 44% of potential fee revenue was lost.

📊 CUSTOMER SEGMENTS
Standard segment leads transaction volume. Premium customers generate the highest total value but carry a disproportionate 
fraud exposure. Business segment produces the highest fee revenue per transaction despite lowest volume.

🗺️ REGIONAL ACTIVITY
London dominates transaction volume with 375 transactions — nearly double any other region. All fraud activity in the dataset is concentrated in London, making it the single highest-risk region for H1 2026.

🚨 TRANSACTION FAILURES
Only 15% of all transactions completed successfully. Declined transactions account for 35%, Reversed 25%, and Pending 25%.The leading failure reason is Insufficient Funds, followed equally by Card Limit Exceeded and Fraud Suspected.

💳 FRAUD EXPOSURE
20% of all transactions were flagged as fraudulent — 1 in every 5 transactions. Fraud flags are entirely concentrated among KYC-verified Premium customers in the London region, which warrants an urgent risk investigation.

💸 FEE LEAKAGE
Transfer - International shows the largest gap between the standard fee (£2.50) and actual fee charged. ATM Withdrawals 
and Crypto Purchases follow. Total leakage of £587 across H1 represents a significant and recoverable revenue gap for Finance.

⚠️  TOP 3 ACTIONS FOR STAKEHOLDERS
1. RISK   → Investigate London-based Premium customer fraud cluster immediately
2. FINANCE → Audit International Transfer fee application recover £400+ in leakage
3. PRODUCT → Address 85% non-completion rate — prioritise Declined transaction UX fixes

# Temporial Trend

📈 MONTHLY VOLUME & VALUE
Transaction value peaked in January (£465K, 304 txns) and hit its lowest point in April (£264K, 279 txns) — a 43% 
drop in value despite only an 8% drop in volume, suggesting fewer high-value transactions rather than fewer customers 
transacting. May shows recovery to £392K.

💰 FEE REVENUE — STABLE, NOT VOLUME-LINKED
Fee revenue stayed in a tight £134–163 band all five months, peaking in March (£163.41). It does not track the volume dip 
in April — fee collection held steady even as transaction value fell, pointing to fee revenue per transaction rather than overall volume.

📅 FRAUD RATE BY DAY OF WEEK
Monday carries the highest fraud rate (25.2%), while Wednesday is the safest day (14.1%) — a meaningful ~11 percentage point gap. Friday and Saturday also run above average (21–22%), suggesting weekday-start and weekend activity both warrant closer monitoring.

📊 TRANSACTION STATUS BY MONTH
Declined is the leading status in every single month (92–114 transactions) — this is a consistent, structural pattern rather than a one-off spike. Completed transactions remain the smallest group throughout (35–51 per month).

🔥 HOURLY HEATMAP
Activity is broadly spread across all 24 hours with no single dominant time block — the busiest individual hour-day combinations (e.g. Thursday 3pm, Thursday 7pm, Friday 4pm) each account for only 14–16 transactions, roughly in line with the average. Fraud flags peak slightly around 3pm, 6pm, and 9pm but the variation across hours is modest.

⚠️ WHAT THIS MEANS
1. The April dip in value (not volume) deserves investigation check if large-ticket transaction types specifically 
   dropped that month.
2. Decline issues are persistent, not seasonal — a fix needs to address root cause, not a particular month.
3. Monday's elevated fraud rate is the clearest day-of-week signal in the data and a reasonable starting point for the fraud team's monitoring rules.
   
# Customer & Segment Analysis

💰 VALUE CONCENTRATION IN PREMIUM
Premium customers drive 63.3% of total transaction value (£1.2M) from just 375 transactions, but also carry the highest fraud rate at 40% — the most value-concentrated and risk-concentrated segment by far. Starter customers show 0% fraud across all 375 of their transactions, making them the cleanest segment.

🗺️ FRAUD IS A TWO-REGION PROBLEM, NOT JUST LONDON
London accounts for the most transactions (375) and the highest fraud rate (60%). Midlands is the only other region with any fraud exposure, at 33.3%. All eight remaining regions — including South East, Scotland, and North West — show 0% fraud. This narrows the investigation to two regions rather than treating fraud as nationally distributed.

🔍 KYC VERIFICATION ANOMALY
100% of fraud (300 of 300 flagged transactions) comes from KYC-verified customers; the unverified group has zero fraud flags despite making up 300 transactions. Verified customers also have a notably worse decline rate (37.5% vs 25%). This pattern suggests either fraud is occurring after verification (account takeover) or the KYC process isn't a meaningful fraud deterrent on its own — worth flagging to Compliance as a process question, not just a customer-screening one.

💵 FEE REVENUE PER TRANSACTION FAVOURS BUSINESS
Business customers pay the highest average fee per transaction (£1.00) despite the lowest transaction volume (300), generating £300.37 in total fees. Standard customers pay the lowest average fee (£0.17) despite the highest volume (450 transactions) — the segment with the most activity is the least profitable per transaction.

🚨 RISK CONCENTRATED IN JUST 4 CUSTOMERS
Only 4 of 20 customers carry any fraud exposure at all, and each sits at exactly 100% fraud rate across all 75 of their transactions: Charlotte Lewis (Midlands, £22.4K), Daniel Oka for (London, £33.7K), Mohammed Al-Hassan (London, £5.6K), and Rajan Mehta (London, £1.12M). Rajan Mehta alone accounts for the vast majority of risk-adjusted value exposure in the entire dataset.

⚠️ WHAT THIS MEANS
1. Risk team should prioritise Rajan Mehta's account first —  £1.12M at 100% fraud rate is the single largest exposure in H1 2026.
2. Investigate whether London + Midlands share a common merchant, channel, or onboarding cohort driving fraud,since all 4 flagged customers fall in these two regions.
3. Compliance should review whether KYC verification is being exploited post-approval rather than failing at the screening stage.

# Channel, Merchant & Device Health

📲 AUTOMATED CHANNEL IS THE FRAUD HOTSPOT Automated transactions carry the highest fraud rate at 37.5% (150 of 400 flagged) — more than double Mobile App and Web Browser (16.7% each). ATM Network has 0% fraud but still shares the same 37.5% decline rate as Automated, suggesting its failures are driven by something other than fraud (likely insufficient funds or limits).

⚠️ RISK CLASSIFICATIONS DON'T MATCH ACTUAL FRAUD
Fuel (Low risk) has the highest fraud rate of any merchant category at 31.3%, ahead of Gambling (High risk) at 30.1%. Four categories — Online Retail, Loan & Credit, Electronics, and Gambling — sit within a tight 30.1–31.0% band, while Dining & Restaurants and Entertainment (both Low risk) are right behind at 29.8%. The risk_flag classification is not
predictive of actual fraud rate in this dataset and should be reviewed.

💻 DEVICE PATTERNS REVEAL THREE DISTINCT PROBLEMS
iOS: 40% decline rate but 0% fraud — a processing/UX issue, not a risk issue. Android & Web: 0% declines but 20% fraud each, with fraud appearing in different status categories (Android stuck in Pending, Web ending in Reversed).No device recorded (ATM/Automated transactions): the highest fraud rate of any group at 40%, and 100% of these end in Declined. This is the single highest-risk operational segment and was easy to overlook since it has no device label.

🌍 INTERNATIONAL VS DOMESTIC
International transactions have a higher fraud rate (25% vs 18.8%) despite being only 20% of volume (300 vs 1,200).Domestic transactions have a slightly higher decline rate (35.4% vs 33.3%). International transactions are riskier per-transaction even though domestic produces more total failures.

💸 FEE LEAKAGE — AND THE OPPOSITE PROBLEM
Transfer-International accounts for £400 of fee under collection alone — by far the largest gap, charging an average of £0.50 against a £2.50 standard fee. But several transaction types that should carry no fee (Standing Order, Loan Repayment, Direct Debit, Savings Pot Transfer, Transfer-Outbound) are being charged £0.75–£0.88 on average where the typical fee is £0.00 — this is overcharging, not leakage, and is a separate billing-accuracy issue Finance should review alongside the leakage.

⚠️ WHAT THIS MEANS
1. The "N/A device" segment (ATM/Automated, 40% fraud, 100% decline-on-fraud) is the most acute operational risk on this page and deserves its own line item — it was hidden by having no device label.
2. Don't rely on risk_flag to prioritise fraud investigation; use actual fraud rate by category instead.
3. Finance should treat fee leakage (under-charging on International Transfers) and fee overcharging (on supposedly free transaction types) as two separate corrective actions.
