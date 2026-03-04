# Interview Preparation Q&A (Power BI / D365 / UKG)

## 1. Give an overview of your Power BI development experience.

**Answer:** I have around 8+ years of experience specifically in Power
BI development, mainly focused on building enterprise-level reporting
solutions for finance, operations, and supply chain teams. My work
usually starts with requirement gathering where I work directly with
stakeholders to understand KPIs and reporting needs. I then design the
data model using a star schema and build Power BI dashboards. I also
write advanced DAX measures such as budget vs actual, operating margin,
and rolling 12‑month trends. I work with large datasets and optimize
performance using techniques like incremental refresh, reducing
cardinality, and optimizing relationships. I also implement Row-Level
Security to ensure users only see relevant data.

------------------------------------------------------------------------

## 2. Talk about your experience building semantic models and star schemas from ERP data.

**Answer:** In several projects I have built Power BI semantic models
using ERP data from systems like Dynamics 365 Finance and Operations.
ERP systems are highly normalized, so I transform the data into a star
schema for analytics. I create fact tables for transactional data and
dimension tables for attributes like department, account, date, or cost
center. I establish one‑to‑many relationships from dimensions to facts
to ensure correct filtering. I also remove unnecessary columns and
optimize the model for performance. Then I build DAX measures that serve
as reusable business metrics across reports.

------------------------------------------------------------------------

## 3. Talk about your direct work with Dynamics 365.

**Answer:** I have worked directly with Dynamics 365 in multiple
projects, primarily integrating data from Dynamics 365 Finance and
Operations into Power BI for reporting. I work with modules such as
General Ledger, Accounts Payable, Procurement, and Supply Chain. I
extract ERP data through Azure SQL or reporting layers, analyze the
table structures, and convert them into star schema models. I then build
financial measures like operating margin and budget vs actual. I also
validate that Power BI results match ERP reports and implement Row-Level
Security to control access.

------------------------------------------------------------------------

## 4. Provide examples of complex DAX measures you have built.

**Answer:** One example is Budget vs Actual Variance where I created
measures for actual totals, budget totals, and variance percentage.
Another example is Operating Margin calculation using revenue and
operating expenses. I have also created Rolling 12‑Month Trend measures
using time intelligence to analyze performance trends. Additionally, I
built Year‑over‑Year growth measures and department-level expense
allocation calculations that distribute shared costs across departments
based on allocation logic.

------------------------------------------------------------------------

## 5. Are those DAX measures around financial logic or time intelligence?

**Answer:** They are usually a combination of both financial logic and
time intelligence. Financial logic includes calculations like operating
margin or budget variance based on accounting rules. Time intelligence
includes calculations like rolling 12‑month trends, year‑to‑date totals,
or year‑over‑year comparisons. In most financial dashboards both
concepts are combined so users can see financial metrics and how they
trend over time.

------------------------------------------------------------------------

## 6. Talk about your experience implementing Row-Level Security in an enterprise environment.

**Answer:** I have implemented Row-Level Security in several enterprise
Power BI environments. In large organizations different users should
only see data relevant to their department or region. I create roles in
the dataset and apply filters to dimension tables such as department or
region. In many cases I implement dynamic security using a user mapping
table that connects user email addresses with their assigned business
unit. Power BI automatically filters data based on the logged-in user.
This ensures proper governance and compliance.

------------------------------------------------------------------------

## 7. Talk about your experience ensuring reconciliation between ERP transactional data and reporting data.

**Answer:** When working with ERP systems like Dynamics 365 Finance and
Operations, reconciliation is critical. I first identify the
source-of-truth tables such as General Ledger transactions. Then I
validate record counts and transaction totals between the ERP system and
the reporting dataset. I also compare totals such as revenue and
expenses with ERP reports like trial balances. If discrepancies appear,
I check transformation logic, filters, and relationships in the model. I
often create validation pages in Power BI dashboards so finance teams
can quickly confirm that totals match ERP data.

------------------------------------------------------------------------

## 8. Talk about your experience independently gathering requirements and delivering production-ready dashboards.

**Answer:** In many projects I manage the entire lifecycle from
requirement gathering to production deployment. I meet with stakeholders
such as finance or operations teams to understand KPIs and reporting
needs. I document metrics, filters, and layout expectations. Then I
design the semantic model using a star schema and build DAX measures for
the required KPIs. After building the dashboards, I validate them with
business users and reconcile numbers with ERP reports. Finally, I
publish the reports to Power BI Service, configure refresh schedules,
apply Row-Level Security, and deliver the production-ready dashboard.

------------------------------------------------------------------------

## 9. Has anyone else approached you or submitted your resume for this UKG role?

**Answer:** No, I have not been approached by anyone else for this
position with UKG, and I have not shared my resume with any other vendor
for this role. Your team is the only team I have been working with
regarding this opportunity.

------------------------------------------------------------------------

## 10. Are you familiar with Kronos / UKG?

**Answer:** Yes, I am familiar with Kronos. Kronos merged with Ultimate
Software and is now known as Ultimate Kronos Group (UKG). It is an HCM
platform used for workforce management including timekeeping,
scheduling, payroll, and workforce analytics. Data from systems like UKG
can be integrated into reporting platforms like Power BI to analyze
workforce metrics such as employee hours, labor costs, and staffing
performance.

------------------------------------------------------------------------

## 11. Are you comfortable working in Eastern Time hours?

**Answer:** Yes, that would not be an issue. Even though I'm based in
McKinney, Texas in Central Time, I am comfortable adjusting my schedule
to work in Eastern Time to align with the team and business operations.

------------------------------------------------------------------------

## 12. When will you be available to start?

**Answer:** My current client engagement is expected to wrap up next
Friday, so I would be available to start from the following Monday. I
can also be flexible depending on the onboarding timeline.
