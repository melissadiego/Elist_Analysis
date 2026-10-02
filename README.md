# EList Electronics: Executive Revenue & Loyalty Analytics

An executive-level Tableau analytics dashboard analyzing sales performance, YoY revenue growth, and monthly order trends for EList Electronics.

## Overview

EList Electronics is a global e-commerce retailer specializing in consumer tech and electronic accessories. Operating across multiple international markets and sales channels, the company relies heavily on customer loyalty programs, seasonal promotional strategies, and efficient post-purchase experience management to drive long-term revenue growth.

This project analyzes EList's multi-year transactional order data (2019–2022) to evaluate key financial indicators, monitor order volumes, and measure loyalty program performance. The analysis also addresses raw data quality issues, including inconsistent identifier formats and incomplete relational lookup schemas, to bridge the gap between raw transactional logs and executive-ready decision-making.

## Key Business Objectives
* **Revenue Trends & Sales Performance:** Track macro sales trajectory, average order value (AOV), and year-over-year (YoY) revenue growth across global regions.
* **Loyalty Program Impact:** Evaluate customer adoption rates and compare purchasing frequency, order value, and total revenue contribution between loyalty and non-loyalty members.
* **Operational Quality & Refunds:** Monitor product refund rates over time to identify operational friction, customer churn risks, and return behavior across channels.


## Executive Summary


<img width="661" height="401" alt="image" src="https://github.com/user-attachments/assets/bf175368-cd75-438b-8cde-c5384ae20c0e" />


Between 2019 and 2022, EList Electronics generated $28.11M in total revenue across 108,124 orders, maintaining an average monthly revenue of $585.68K.

* **Macro Trajectory:** Significant pandemic-era growth peaked in 2020 (+163% YoY), followed by an initial post-peak decline in 2021 (-10% YoY) that accelerated into a severe contraction in 2022 (-46% YoY).
* **Loyalty & Retention:** While overall order volume contracted in 2021–2022, loyalty program adoption scaled rapidly, establishing a steady revenue baseline that cushioned the downturn.
* **Operational Progress & Data Quality:** Recorded product refund rates dropped to 0.00% by 2022. However, a data quality audit identified a post-2021 refund-logging cutoff in the raw order data, confirming this is an unrecorded tracking gap rather than an operational improvement.

## Overall Sales Trends

From 2019 through late 2020, EList experienced rapid revenue expansion, followed by a post-pandemic demand stabilization phase through 2022.

* **Historical Growth Surge (2019 – Late 2020):** Sales started at a steady baseline of $250K–$350K/month throughout 2019 before climbing rapidly in 2020, peaking in December 2020 at an all-time high of **$1.25M ($1,251,721)** in monthly revenue.
* **Post-Peak Stabilization (2021 – 2022):** Following the late-2020 spike, monthly sales normalized across global channels, holding steady at $600K–$800K through 2021 before tapering off in 2022.
* **Low Point & Holiday Recovery:** Monthly revenue hit its lowest point of $178K ($178,275) in late 2022, before showing early signs of a holiday upturn toward year-end.


### Monthly & Yearly Growth Dynamics

EList’s financial trajectory was defined by hyper-expansion during pandemic lockdowns, followed by a sharp post-peak correction as macroeconomic conditions normalized and consumer spending shifted away from home electronics.

#### Yearly Growth Dynamics (YoY)

<img width="661" height="375" alt="image" src="https://github.com/user-attachments/assets/ef87aee5-5155-413c-8846-dbedd5f8c457" />

* **2020 Surge (+163% YoY): Demand Surge & Macro Windfalls**
  * *Driver:* Widespread stay-at-home mandates and remote-work shifts triggered an unprecedented surge in consumer electronics demand.
  * *Impact:* EList capitalized on elevated digital shopping traffic, scaling revenue rapidly to an all-time peak of $1.25M in December 2020.

* **2021 Stabilization (-10% YoY): High Baseline Comparisons & Market Normalization**
  * *Driver:* As physical retail reopened and pandemic restrictions eased, online electronics buying stabilized against 2020's record-high comparison baseline.
  * *Impact:* Top-line revenue contracted slightly (-10% YoY) but remained historically elevated, supported by accelerating loyalty program adoption that cushioned falling non-member demand.

* **2022 Post-Pandemic Correction (-46% YoY): Macro Headwinds & Demand Exhaustion**
  * *Driver:* Broader macroeconomic pressures including rising inflation, elevated interest rates, and pulled-forward demand from prior upgrade cycles severely curtailed discretionary tech spending.
  * *Impact:* Annual revenue collapsed by -46% YoY, troughing at $178K in late 2022. This steep drop highlighted EList’s vulnerability to cyclical electronics demand and underscored the need to revamp member retention strategies.

#### Monthly Volatility (MoM)

<img width="675" height="402" alt="image" src="https://github.com/user-attachments/assets/df9c07f5-c126-4bbf-999f-21eeb0493f43" />

* **Peak MoM Increase (+50.3%): Seasonal Surge & Holiday Promotional Pushes (December 2020)**
  * *Driver:* Accelerated by holiday promotional campaigns, year-end shopping volume, and heightened online retail demand during stay-at-home restrictions.
  * *Impact:* Driven by peak purchasing cycles, EList recorded its highest single-month expansion (+50.3% MoM), lifting monthly revenue to an all-time peak of $1.25M.

* **Maximum MoM Drop (-55.2%): Post-Holiday Hangover & Off-Peak Demand Adjustments**
  * *Driver:* Following intense Q4 shopping surges, consumer electronics spending typically experiences an immediate off-peak drop-off in early Q1 as holiday promotional campaigns end and demand normalizes.
  * *Impact:* Revenue suffered a sharp -55.2% MoM contraction in January post-holiday transitions, exposing significant baseline volatility following peak promotional cycles.


### Loyalty Program Performance & Strategic Recommendation

Customer engagement metrics reveal a more nuanced picture than the simple assumption that "loyalty members are better customers." While non-members place higher-value single orders ($274.61 vs. $240.23) and buy slightly more often (1.26 vs. 1.16 orders), rapid loyalty program adoption established a crucial revenue baseline that cushioned EList during its post-peak market decline.

#### Program Insights

* **Revenue Adoption & Crossover (2019–2021):** Loyalty program revenue scaled steadily from 2019 onward, officially overtaking non-loyalty sales by mid-2021 to become EList's primary revenue driver. Today, program members account for 39% of total lifetime revenue across 45% of the customer base.
* **Downturn Stabilization (2021–2022):** As non-loyalty revenue plummeted during the post-pandemic market pullback, loyalty spend held significantly higher than non-member spend through late 2021 and 2022. This recurring member base cushioned top-line contraction and reduced revenue swings compared to volatile guest shopper demand.

<img width="661" height="401" alt="image" src="https://github.com/user-attachments/assets/5a9643af-9e6f-4e4e-9901-162aef022604" />


#### Key Behavioral Metrics

* **Average Order Value (AOV):** Non-loyalty customers generate a higher average basket size at **$274.61** compared to **$240.23** for loyalty members—a **$34.38** gap per order[cite: 7, 10, 11, 13].
* **Purchase Frequency:** Non-loyalty customers demonstrate a slightly higher purchase frequency per user (**1.26 orders**) than loyalty members (**1.16 orders**)[cite: 8, 10, 11, 13]. This gap confirms that the loyalty program is not currently driving higher order volume per customer; instead, its strategic value lies in providing revenue predictability and stability during market pullbacks [cite: 6, 10].

#### Verdict: Retain the Loyalty Program, but Reassess Its Value Proposition


<img width="661" height="401" alt="image" src="https://github.com/user-attachments/assets/262d5f8d-fc85-4fc0-bafc-ee7cc39a53f2" />

On a per-transaction and per-customer basis, non-loyalty customers currently outperform loyalty members across both AOV and purchase frequency[cite: 7, 8, 10, 11]. However, EList should retain the program: its rapid adoption and sustained revenue contribution through the 2021–2022 market contraction established an essential revenue cushion[cite: 6]. 

Rather than assuming the program inherently creates behavioral loyalty (larger, more frequent orders), EList must recognize this gap as a key program design opportunity to actively incentivize repeat high-value behavior[cite: 10].

#### Actionable Next Steps

1. **Bridge the AOV and Frequency Gap:** Introduce tiered reward thresholds (e.g., *"Spend $275 to unlock free expedited shipping or double points"*) to elevate member order value past non-member baselines, along with frequency-based incentives (e.g., a bonus discount on a 3rd purchase)[cite: 10].
2. **Re-verify Program ROI & Acquisition Mechanics:** Given that loyalty members currently track lower on AOV and frequency, confirm what specific operational benefits (e.g., lower customer acquisition cost, higher multi-year retention) offset program expenses before allocating additional marketing budget[cite: 10].
   
<img width="661" height="401" alt="image" src="https://github.com/user-attachments/assets/3261dd53-0c68-4762-9a80-672d860c57b8" />


### Refund Rates & Data Governance Audit

An analysis of product return performance revealed an apparent operational improvement that, upon deeper investigation, uncovered a significant data ingestion gap in the raw order dataset.

#### Key Findings

* **Historical Peak & Decline (2019–2021):** Recorded product refund rates peaked at **9.22% in 2020** (up from 5.73% in 2019), driven by high order volume and supply chain delays during the pandemic demand surge. Return rates stabilized down to **3.61% in 2021** as operations normalized.
* **The 2022 Data Cutoff Anomaly (0.00%):** In 2022, the recorded refund rate dropped abruptly to **0.00%**. A data pipeline audit confirmed this is an **unrecorded data logging gap** rather than flawless operational fulfillment—the `refund_ts` timestamp field ceased to populate after 2021 in the upstream order pipeline.

#### Operational & Data Governance Action Items

1. **Pipeline Audit & Pipeline Fix:** Flag the missing post-2021 `refund_ts` ingestion issue to the data engineering team to restore active logging and backfill missing return records before drawing conclusions on recent product quality or customer satisfaction.
2. **Adjust Metric Baseline:** Exclude 2022 return metrics from executive reporting until data completeness is restored, using 2021's **3.61% baseline** for product return projections.

<img width="661" height="401" alt="image" src="https://github.com/user-attachments/assets/0d8535db-8ef0-4c0e-a83a-790714a1b127" />



## Strategic Recommendations

Based on executive-level trends across sales volume, loyalty adoption, and operational quality from 2019–2022, EList should execute three primary strategies to reignite growth and optimize profitability:

<img width="661" height="401" alt="image" src="https://github.com/user-attachments/assets/4f0ff716-5a26-4ad6-a208-6bb67b7325bc" />


#### 1. Bridge the AOV Gap via Tiered Incentives & Premium Loyalty Perks
* **Finding:** Box plot price distributions reveal that while Loyalty Members offer highly predictable spend tightly clustered under $200, Non-Loyalty shoppers drive the majority of high-ticket outlier purchases ($500 to $3,000+), resulting in a $34.38 lower Average Order Value (AOV) for members ($240.23 vs. $274.61).
* **Action:** EList must revamp its program to capture high-value buyers by introducing spend-threshold rewards (e.g., free expedited shipping or bonus reward points on orders over $275) and VIP tier perks tailored for premium electronics buyers.

#### 2. Optimize Repeat Engagement & Frequency-Based Rewards
* **Finding:** Non-loyalty users currently exhibit a higher purchase frequency (1.26 orders per user) than enrolled loyalty members (1.16 orders per user), indicating the program is underperforming as an accelerator for repeat order frequency.
* **Action:** Shift the loyalty engagement strategy from passive point accumulation to proactive re-engagement triggers (e.g., automated replenishment discounts on accessories, bounce-back coupons for a 3rd purchase, and targeted lifecycle email campaigns).

#### 3. Resolve Data Ingestion Gaps & Re-establish Return Metrics
* **Finding:** Recorded product refund rates artificially dropped to 0.00% in 2022 due to an upstream pipeline logging cutoff (`refund_ts` timestamp ceased populating after 2021).
* **Action:** Data engineering must audit and patch the ETL logging pipeline to backfill missing refund records. In the interim, executive forecasting should benchmark product return expectations against 2021's 3.61% baseline rate rather than unverified 0% figures.

## Dashboard Preview

🔗 [View the full interactive dashboard on Tableau Public](https://public.tableau.com/app/profile/melissa.diego7336/viz/ElistProject_17883044843860/OverallSalesGrowth)

## EList Data 

The database structure, as shown below, consists of four tables: 
* orders
* customers
* geo_lookup
* order_status

with a total row count of 108,124 records.

<img width="845" height="512" alt="image" src="https://github.com/user-attachments/assets/8e7bdd7d-9466-4f64-9516-dd35add2f04d" />



## Tech Stack & Tools
* **Data Visualization:** Tableau Desktop (Executive KPIs, Trend Dashboards, Cohort Comparison)
* **Data Transformation & Preprocessing:** Google Sheets (Data Audit Logging, String Standardization, Null Management)
* **Data Modeling:** Relational Lookups (Primary/Foreign Key Joins between Orders & Country Schema)
* **Documentation:** GitHub/ Markdown

**Data Preprocessing Note:** The row count difference between the total relational database records (108,124) and the cleaned orders dataset (101,129) reflects foreign key join boundaries and the exclusion of unlinked, non-transactional system logs.
