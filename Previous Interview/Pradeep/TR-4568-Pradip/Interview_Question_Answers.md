Below is your **complete interview Q&A in clean MD (Markdown) format**, ready for copy/paste or sharing.
All answers are written exactly in your speaking style — **natural, professional, and aligned with your profile + JD**.

---

# **Arun Thakur – Interview Q&A (Markdown Version)**

---

## **1. Introduction**

My name is Arun Thakur, and I have a little over **10 years of experience as a Senior Dynamics 365 CRM Developer**, primarily working across **D365 CE, Customer Insights, Azure Services, API Integrations, Power Platform, and .NET**. Currently, I am working with **Prudential Financial as a Tech Lead**, where I lead the **Customer 360 initiative**. I built end-to-end data pipelines using **Azure Data Factory**, created **Azure Functions** for real-time processing, handled large-volume migrations using **SSIS**, and configured **Customer Insights** with unified profiles, measures, and segments.

I also implemented **lead automation using Power Platform**, enhanced the customer portal with **custom JavaScript + Azure Functions**, and improved SLA-driven routing. Prior to Prudential, I worked with **Canopy Health, Wells Fargo, and Accenture (Best Buy)** in similar CRM modernization and integration roles. Overall, I bring strong practical experience across **ADF, Customer Insights, Azure Functions, and SSIS**, and I focus heavily on scalable, real-world solution delivery.

---

## **2. Day-to-Day Responsibilities at Prudential**

As a Lead Dynamics 365 Consultant, my day-to-day involves a mix of **technical leadership, design, and hands-on development**. I start by reviewing ADF pipeline runs, Azure Function triggers, and any overnight data loads that feed the **Customer 360 platform**. I work closely with architects and data engineers to design new ingestion flows, perform schema mapping, and define transformation rules.

I build and review **ADF pipelines, SSIS packages, plugins, JavaScript, and Dataverse integrations**. I also guide junior developers, review pull requests, and ensure we follow CI/CD best practices. Our team consists of about **10–12 members**, including CRM developers, data engineers, QA, and a product owner. My role focuses heavily on **technical direction, solution quality, and cross-team collaboration**.

---

## **3. Difference Between CE Data and Customer Insights Data**

CE holds **transactional, operational data**—such as leads, contacts, cases, and opportunities. It reflects day-to-day CRM activity.
Customer Insights stores **unified, enriched, multi-source data**, including CE, policy systems, marketing platforms, and portal interactions. CI performs matching, merging, deduping, and creates **Unified Profiles, KPIs, and segments**.

In simple terms:
**CE = System of Record**
**CI = System of Intelligence**

---

## **4. Data Sources Registered in Customer Insights**

The main data sources we connected were:

* **Dynamics 365 CE** (contacts, accounts, activities, custom entities)
* **Policy Administration System** (policies, premiums, claims)
* **Customer Portal Database** (logins, case submissions, interactions)
* **Marketing Automation System** (email events, campaign interactions)
* **Azure Function Event Logs** (real-time lead/policy events)
* **Master/Reference Data** (product mapping, region hierarchy)

These combined sources created a complete unified profile.

---

## **5. How Unification, Matching Rules & Duplicate Handling Work**

Customer Insights performs **mapping → matching → merging**.
We used both **deterministic** and **probabilistic** rules.

**Primary rule:**

* **Email = Email**

**Secondary rule:**

* **First Name + Last Name + Date of Birth**

CI merges records when rules match and uses **survivorship rules** to choose which source’s data dominates. CE was our **truth source** for contact details; the policy system was truth for policy information.

**Example:**
If CE has *John Carter* and the policy system has *John D. Carter* with same email, CI merges them into **one Unified Profile**.

---

## **6. Different Matching Rules for Different Sources**

Each system had its own rule because data quality varied.

* For **CE**, we used **Email + ContactID**.
* For **Policy System**, we used **Name + DOB** due to missing emails.

CI evaluates rules in order of priority and merges records accordingly.

---

## **7. What Is a Unified Customer Profile & How It Is Generated**

A **Unified Customer Profile** is the final consolidated customer record CI creates after combining data from all systems.

Steps:

1. **Ingestion** of multi-source data
2. **Mapping** fields to a common schema
3. **Matching** using defined rules
4. **Merging** duplicates using survivorship
5. **Enrichment** with KPIs & segments

It becomes the organization’s **single source of truth** for analytics and insights.

---

## **8. Example of a KPI Using Shared Measures**

One KPI we created was:

### **Total Annual Premium**

```
SUM(Policy.PremiumAmount) GROUP BY CustomerID
```

If a customer had three policies—300, 450, and 250—the KPI = **$1,000**.
This helped identify high-value customers and supported segmentation and CE insights.

---

## **9. Azure Function Used for Real-Time CE Integration**

We built an **HTTP-triggered Azure Function** that received real-time quote submissions from an external system and created/updated leads in CE.

**Key elements:**

* **Trigger:** HTTP Trigger
* **Authentication:** Azure AD App Registration (OAuth 2.0)
* **CE Connection:** Server-to-Server (Client ID + Secret)
* **Logic:** Validate payload → Check duplicates → Create/Update Lead
* **Monitoring:** Application Insights

This enabled real-time, secure integration of external leads into Dynamics 365.

---

## **10. ADF Pipeline for CRM Integration**

ADF pipeline pulled incremental data from the policy system → staged → transformed → loaded into Dataverse/CI.

**Key Features:**

* **Incremental loads** using ModifiedOn watermark
* **Metadata-driven mappings** for schema flexibility
* **Data Flow transformations** for cleansing and standardization
* **Dataverse Connector** for CRM load
* **Monitoring via** ADF portal + Log Analytics + Alerts

If pipeline failed, alerts were triggered and retries were attempted automatically.

---

## **11. SSIS Package for Integrating Data into Dynamics 365**

The SSIS package followed:
**Source → Staging → Validation → Transformation → D365 Load**

**Data Validation:**

* Mandatory field checks
* Data type validation
* Lookup validations
* Redirect invalid rows to **Error Table**

**Error Handling:**

* Conditional Splits
* Logging via Event Handlers
* Email notifications

**Restartability:**

* SSIS **Checkpoints**
* Batch-wise processing
* Audit table storing last successful runtime

This ensured reliable, restartable production loads.

---

## **12. PCF Control Developed (Policy Snapshot Viewer)**

I built a **PCF control** to show a real-time, unified policy snapshot on the Contact form.

**Why PCF instead of OOB?**

* OOB subgrid couldn’t merge **external API + Dataverse** data
* No conditional formatting
* No advanced sorting/filtering
* Poor UI flexibility

**PCF Features:**

* Built using **TypeScript + React + Fluent UI**
* Fetched data via **secured Azure Function**
* Combined CRM + external policy data
* Implemented **pagination, caching, debounce, memoization** for performance

This significantly improved the user experience and reduced navigation time.

---

## **13. Availability for Weekends / Odd Hours**

I am comfortable working during weekends or odd hours whenever required—especially during **deployments, CI refresh jobs, ADF reruns, or production issues**. It’s not frequent, but for critical releases or support windows, I make myself available and handle it responsibly.

---

# **Conclusion**

These answers summarize my real project experience across **Customer Insights, ADF, Azure Functions, SSIS, PCF, and CRM architecture**, and reflect exactly how I contribute as a Senior Dynamics 365 Consultant.

---
