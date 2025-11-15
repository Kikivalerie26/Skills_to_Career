
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
<br>•Imported CFPB complaint data filtered for Bank of America from 2017–2023.

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
| `complaint_channel` | Type of channel complaint was submitted: web, phone, email, fax, referral, postal mail |
| `date_submitted` | Date consumer submitted the complaint |
| `date_received` |The date the CFPB received the complaint |
| `state_abbrv` | Two-letter state abbreviation |
| `state_name` | Full state name |
| `product` | The financial product category (e.g., mortgage, credit card) |
| `sub_product` | Specific product within main category |
| `issue` | The primary issue the consumer experienced (e.g., incorrect credit reporting, dispute error) |
| `sub_issue` | Additional details about the issue |
| `company_public` | Public-facing response from the company |
| `company_response_to_consumer` | How the company resolved or responded to the customer |
| `timely_response` | Whether the company responded within the required timeframe |
| `positive_resolution_flag` | Binary indicator representing if the outcome was positive |
| `timely_flag` | Binary flag indicating timely response (1 = Yes, 0 = No) |
| `received_days` | Days between complaint submission and official receipt |
| `year` | Year extracted from Date Received |
| `month` | Month extracted from Date Received |

---

##  Final Deliverables

| Sheet Name | Description |
|------------|-------------|
| `Business Problem Report`  | Structured documentation outlining the core business problem, project goals, and the purpose of each analytical component |
| `Data Cleaning and Transformation Report`    | High-level summary of the cleaning steps, and the and key insights |
| `Interactive Dashboard`   | A multi-page Power BI dashboard visualizing complaint trends, product issues, geographic distribution, and responsiveness metrics |
| `Insights & Recommendation Report`   | A detailed interpretation of insights across products, issues, regions, and channels, along with data-driven recommendations to improve service quality and reduce complaints |



---

##  Learnings and Assumptions

**Learnings**

<br>•Complaint analysis reveals hidden breakdowns in customer experience.
<br>•Trend analysis helps predict peak problem periods.
<br>•Operational delays often stem from manual processes (mail, referrals).
<br>•Data inconsistencies require strong cleaning and transformation before visualization.

**Assumptions**

<br>•Complaints accurately reflect customer sentiment and service quality.
<br>•Missing values were handled consistently and do not bias results.
<br>•Date Received is the best indicator for trend analysis..

---

##  Final Thoughts

This project strengthened my ability to work with large, real-world financial datasets, including cleaning unstructured text fields, standardizing categorical variables, and preparing multi-year complaint data for analysis. I gained hands-on experience in identifying product-level trends, evaluating operational performance, and measuring response timeliness- all of which are essential skills for analytics roles in the financial services industry.

Additionally, I developed a deeper understanding of how complaint data can reveal underlying customer experience issues, regional performance disparities, and early indicators of compliance risk. By creating dashboards and performing exploratory analysis, I honed my skills in transforming raw data into actionable insights that drive informed decision-making.

Leveraging data modeling, feature engineering, and visual analytics, this project demonstrates how Bank of America leadership can adopt a proactive approach to complaint management, address root causes, and implement long-term improvements in service quality and customer satisfaction.




