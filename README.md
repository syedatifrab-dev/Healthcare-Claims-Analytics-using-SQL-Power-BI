# Healthcare-Claims-Analytics-using-SQL-Power-BI
This project simulates health insurance claims analytics for Aetna, inspired by real-world claims processing experience at Concentrix.  The dashboard analyzes claims volume, denials, turnaround time (TAT), and quality KPIs to support operational efficiency, SLA compliance, and process improvement.  

*🎯 Business Objectives*

-Monitor claims performance across approval, denial, and pending states

-Identify top denial reasons and error patterns

-Track turnaround time (TAT) and SLA compliance

-Measure quality metrics such as First-Pass Yield

-Enable data-driven process improvements

*📊 Dataset Description*

The project uses a star schema model.

Fact Table

claims_12000_rows.csv (12,000+ rows)

ClaimID

MemberID

ProviderID

ProcessorID

CPT / ICD codes

Claim Status (Approved / Denied / Pending)

Denial Reason

Billed & Approved Amounts

Received & Processed Dates

Rework Flag

*Dimension Tables*

Members (Age, Gender, Plan Type, State)

Providers (Type, Specialty, Location)

Processors (Team, Experience)

Date (Calendar attributes)

*🧱 Data Modeling*

Star schema with Claims as Fact

One-to-many relationships to dimensions

Optimized for Power BI performance and DAX simplicity

*⚙️ Data Preparation (Power Query)*

Removed duplicates

Standardized date formats

Handled nulls for pending claims

Created Turnaround Time (TAT) column
  -TAT_Days = ProcessedDate - ReceivedDate

📈 Dashboards & KPIs
1️⃣ Executive Claims Overview

KPIs

Total Claims

Approval Rate

Denial Rate

Average TAT

Visuals

Line chart: Claims trend over time

Donut chart: Claim status distribution

Bar chart: Claims by plan type

2️⃣ Denial & Error Analysis

Visuals

Bar chart: Denials by reason

Heatmap: Provider vs Denial Rate

Table: CPT codes with highest denials

Insight

Eligibility issues and missing documentation are top denial drivers.

3️⃣ Turnaround Time & SLA

Visuals

Line chart: Avg TAT trend

Gauge: SLA compliance %

Column chart: TAT by claim status

4️⃣ Quality & Productivity

Visuals

KPI: First-Pass Yield

Bar chart: Error rate by processor/team

Table: Rework vs Non-rework claims


🧠 Business Impact

Helps operations teams reduce rework and denials

Improves SLA monitoring and turnaround time

Enables leadership-level visibility into claims health

Demonstrates transition from operations → analytics

🛠 Tools & Technologies

Power BI

Power Query

DAX

Excel / CSV

Healthcare domain knowledge (Claims lifecycle)




















Validated categorical fields
