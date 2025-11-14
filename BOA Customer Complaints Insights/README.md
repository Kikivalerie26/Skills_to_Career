
# Bank of America Customer Insight Project
**Financial Services – Consumer Complaint Analysis (2017–2023)**

The goal is to uncover actionable insights into **customer dissatisfaction**, **complaint patterns**, **service breakdowns**, and **overall responsiveness**.
It was completed as a Financial Data analyst onboarding project.

---

##  Project Overview

This project analyzes Bank of America consumer complaints submitted to the Consumer Financial Protection Bureau (CFPB) between 2017 and 2023.

The dataset provided captured customer-submitted complaints across multiple financial products, complaint categories, submission channels, company response types, geographic locations, and resolution timeliness. These records offer a detailed view into how customers experience Bank of America’s financial services and how effectively the organization responds.

Bank of America is one of the largest financial institutions in the U.S., yet continues to receive a high volume of complaints regarding credit cards, mortgages, loans, deposits, and credit reporting.
These complaints highlight challenges around:

**Customer experience and transparency**
<br>•Confusing fees, unclear communication, and unsatisfactory resolutions.

**Operational efficiency**
<br>•Delays in processing disputes, loan applications, or transaction issues.

**Compliance and regulatory performance**
<br>•Concerns about fair credit reporting, improper charges, and regulation breaches.

**Service delays and ineffective resolutions**
<br>•Slow response times and inconsistent outcomes impacting customer satisfaction.
   
---

##  Tools Used

- Microsoft Excel/Powerquery – initial cleaning, exploratory analysis
- Power BI – dashboard development, visual exploration, KPI tracking
- Functions: `DAX()`, `TEXT()`, `DATEDIF()`


---

##  Key Results

Complaints increased significantly between 2020–2023, with peaks May–August.
Web is the most preferred complaint channel and has the best timeliness performance.
Checking/savings products show the highest complaints.
Complaint resolution timeliness is high (93.77%), but certain product categories lag.
Geographic analysis shows uneven distribution, with certain states reporting elevated complaint volumes.
Majority of issues relate to incorrect information, fraud disputes, and account closure difficulties.

### Results Synopsis

| Analysis | Summary |
|----------|---------|
| **Product Complaint Distribution** | The product-level analysis reveals that certain financial products generate a disproportionately high number of customer complaints for Bank of America. <br><br>**Findings:** <br>• The highest complaint volumes came from credit card, checking/deposit accounts, and mortgage products. <br>• Credit card complaints accounted for over 35% of total submissions. <br>•Loan-related complaints showed consistent year-over-year growth from 2020–2023.  <br><br>**Insights:** <br>• High volumes suggest recurring dissatisfaction with fees, billing disputes, and transaction errors. <br>• Mortgage and loan complaints are strongly tied to delays, miscommunication, and documentation issues. <br><br>**Recommendations:** <br>• Improve transparency in credit card billing, enhance fraud dispute processes, and streamline mortgage servicing workflows to minimize delays. |
| **Top Complaint Issues** | Customer retention analysis indicates a **declining retention trend** over time. <br><br>**Findings:** <br>• Highest retention was observed in September 2020 with **13%** after one month. <br>• Retention rates drop below 7% by the second month across most cohorts. <br>• By the third and fourth months, retention rates approach **0%**. <br>• January 2021 shows no retention beyond the first month. <br><br>**Insights:** <br>• The e-commerce platform struggles with maintaining repeat customers beyond the first purchase. <br><br>**Recommendations:** <br>• Implement loyalty programs, personalized offers, and stronger post-purchase engagement strategies to boost repeat purchases and reduce churn. |

---

##  Dataset Description

| Column Name | Description |
|-------------|-------------|
| `user_id` | Unique identifier for each customer |
| `event_type` | Type of event: product view, cart open, or purchase |
| `category_code` | Product category code |
| `brand` | Brand name of the product |
| `price` | Product price in USD |
| `event_date` | Date of user activity (YYYY-MM-DD) |

---

##  Analysis

| Section | Description |
|---------|-------------|
| **Raw Data** | The dataset represents user interactions with an e-commerce platform, capturing different event types related to product engagement. The key fields include `user_id`, `event_type`, `category_code`, `brand`, `price`, and `event_date`. The time range analyzed spans from **September 24, 2020 to September 28, 2021**. For meaningful insights, only relevant portions of the dataset — specifically `user_id`, `event_date`, and `event_type` — were used. |
| **Conversion Funnel** | To analyze how users interact with the website, the primary focus was on **purchase events** from the `event_type` field. It was assumed that all interactions were recorded without missing data. Each `user_id` represents a distinct individual, and multiple interactions are recorded as separate rows. |
| **Retention Rates** | To build cohorts and calculate monthly retention rates, the primary focus was on the `user_id`, `first_purchase_month`, and `cohort_age` attributes from the `purchase_activity` sheet. Due to incomplete data for **February 2021**, no retention rate was calculated for that cohort. |

---

##  Final Deliverables

| Sheet Name | Description |
|------------|-------------|
| `Table of Contents` | Organized index of all sheets and their purposes |
| `Executive Summary` | High-level summary of results and key insights |
| `conversion_funnel` | Pivot table showing user flow and conversion rates |
| `retention_rates` | Table with calculated cohort retention percentages |
| `cohort_analysis` | Pivot table with unique user counts per cohort age |
| `purchase_activity` | Filtered purchases dataset, with additional cohort columns |
| `first_purchase` | Pivot table displaying first purchase dates per user |
| `raw_user_activity` | Full original raw event logs from the Shopify App |

---

##  Learnings and Assumptions

- Each `user_id` was treated as a unique individual.
- Assumed all recorded interactions were accurate and complete.
- Focused only on relevant events to create a clean, meaningful analysis.
- First purchases determined cohort assignment.
- No retention calculated for cohorts impacted by missing/incomplete data (e.g., February 2021).

---

##  Final Thoughts

This project developed my skills in cleaning e-commerce datasets, building conversion funnels, segmenting user cohorts, and calculating retention — all essential capabilities for data-driven decision-making in an e-commerce environment.



