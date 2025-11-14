
# Bank of America Customer Insight Project
**Financial Services – Consumer Complaint Analysis (2017–2023)**

This project analyzes consumer complaints submitted against Bank of America to the Consumer Financial Protection Bureau (CFPB) from 2017 to 2023.
The goal is to uncover patterns in **customer dissatisfaction**, **complaint patterns**, **service breakdowns**, **overall responsiveness**, **operational bottlenecks**, **response delays**, and **regulatory risks**- ultimately providing insights that can guide better decision-making in the financial services sector.
It was completed as a Financial Data analyst project.

---

##  Project Overview

Bank of America, one of the largest financial institutions in the United States, receives a consistently high volume of consumer complaints across products such as credit cards, deposits, mortgages, loans, and credit reporting.

This project leverages seven years of CFPB complaint data to:
<br>•Identify which products and issues generate the most complaints
<br>•Analyze geographic and demographic complaint patterns
<br>•Assess response timeliness and resolution quality
<br>•Compare the effectiveness of complaint submission channels
<br>•Provide data-driven recommendations for process and service improvements

---
## Methodology

The project followed a structured analytical workflow:
1.**Data Extraction**
Imported CFPB complaint data filtered for Bank of America from 2017–2023.

2.**Data Cleaning & Preparation**
<br>•Standardized date formats
<br>•Filled missing values
<br>•Cleaned text fields
<br>•Removed duplicates
<br>•Added calculated fields (resolution speed, region categories)

3.**Exploratory Data Analysis (EDA)**
<br>•Complaint distribution by year
<br>•Top products & issues
<br>•Resolution categories
<br>•Response timeliness
<br>•Complaint submission channels
<br>•Geographic patterns

4.**Visualization & Dashboard Development**
<br>•Dashboards created using Power BI.

5.**Insights & Recommendations**
Identified root issues, regional anomalies, and operational improvement oppurtunities

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
| **Top Complaint Issue** | The product-level analysis reveals that certain financial products generate a disproportionately high number of customer complaints for Bank of America. <br><br>**Findings:** <br>• The highest complaint volumes came from credit card, checking/deposit accounts, and mortgage products. <br>• Credit card complaints accounted for over 35% of total submissions. <br>•Loan-related complaints showed consistent year-over-year growth from 2020–2023.  <br><br>**Insights:** <br>• High volumes suggest recurring dissatisfaction with fees, billing disputes, and transaction errors. <br>• Mortgage and loan complaints are strongly tied to delays, miscommunication, and documentation issues. <br><br>**Recommendations:** <br>• Improve transparency in credit card billing, enhance fraud dispute processes, and streamline mortgage servicing workflows to minimize delays. |
| **Regional Complaint Patterns** | Geographic analysis indicates that complaints are concentrated in states with larger customer bases, but certain regions show disproportionate complaint rates. <br><br>**Findings:** <br>•California, Texas, Florida, and New York have the highest complaint counts.<br>• Several mid-sized states show elevated complaints relative to population, signaling potential regional service issues. <br><br>**Insights:** <br>• High-volume states may require optimized staffing and service coverage.<br>• Regional disparities suggest potential branch-level or policy-level inconsistencies. <br><br>**Recommendations:** <br>• Perform targeted regional audits, increase oversight in high-complaint states, and reinforce service quality standards across branches. |
| **Submission Channels** |Analysis of how customers file complaints reveals a clear preference for digital channels, though non-digital options experience slower response times.<br><br>**Findings:** <br>•Web submissions make up more than half of all complaints.<br>• Complaints submitted via phone or mail have longer resolution timelines. <br><br>**Insights:** <br>• Customers expect fast, convenient reporting options.<br>•Manual processes in non-digital channels lead to delayed case handling. <br><br>**Recommendations:** <br>•Expand digital submission features, automate intake routing, and optimize processing workflows for phone and mail submissions. |
| **Response Timeliness & Resolution Quality** | Timeliness and resolution type analysis shows inconsistencies in how quickly complaints are addressed and how effectively they are closed. <br><br>**Findings:** <br>• A significant number of complaints fall under **“delayed response.”**.<br>• **“Closed with explanation”** is the dominant outcome, indicating customers may not feel issues are fully resolved. <br><br>**Insights:** <br>• Delays increase customer dissatisfaction and regulatory risk.<br>•Resolution quality may suffer due to high caseloads or unclear internal processes. <br><br>**Recommendations:** <br>•Track SLA performance more closely, implement automated overdue alerts, and improve agent decision-making guidelines to reduce incomplete resolutions.|

---

##  Dataset Description

| Column Name | Description |
|-------------|-------------|
| `complaint_id` | Unique identifier for each customer |
| `complaint_channel` | Type of channel complaint was submitted: web, phone, email, fax, referral, postal mail. |
| `date_submitted` | Date consumer submitted the complaint. |
| `date_received` |The date the CFPB received the complaint. |
| `state_abbrv` | Two-letter state abbreviation. |
| `state_name` | Full state name |
| `product` | Product price in USD |
| `sub_product` | Date of user activity (YYYY-MM-DD) |
| `issue` | Product price in USD |
| `sub_issue` | Date of user activity (YYYY-MM-DD) |
| `company_public` | Product price in USD |
| `company_response_to_consumer` | Date of user activity (YYYY-MM-DD) |
| `timely_response` | Product price in USD |
| `positive_resolution_flag` | Date of user activity (YYYY-MM-DD) |
| `timely_flag` | Product price in USD |
| `received_days` | Date of user activity (YYYY-MM-DD) |
| `year` | Product price in USD |
| `month` | Date of user activity (YYYY-MM-DD) |

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



