# Dynamics 365 Customer Engagement – Interview Questions & Answers (Consulting / Advisory Role)

---

## 1. How do you handle scenarios where Dynamics 365 F&O and CRM do not share the same database, especially in fraud-related systems?

**Answer:**  
Yes, I’ve worked in that exact scenario, and it’s actually very common in regulated environments. In most enterprise and fraud-heavy implementations, **F&O and CRM are intentionally kept on separate databases**. F&O acts as the **system of record for financial transactions**, while CRM remains the **system of engagement**.

Instead of database-level sharing, I use **integration at the service layer**. CRM only stores the data required for customer interaction—such as case context, flags, and high-level indicators—while sensitive transactional or fraud data stays in F&O. Integration is handled using **event-driven patterns, Power Automate, Dataverse virtual tables, or Azure services**, depending on latency and complexity.

This approach improves **security, compliance, scalability, and performance**, and aligns with best practices.

---

## 2. How do you reconcile golden records from a third-party metadata or MDM service back into Dynamics 365?

**Answer:**  
In this model, the **MDM or metadata service is the system of truth**, and Dynamics 365 is a consumer of mastered data. I never try to make Dynamics the mastering system.

Golden records are exposed through **secure APIs or events** from the MDM platform. On the Dynamics side, I either:
- Use **Dataverse virtual tables** for real-time visibility without data duplication, or  
- Sync a **controlled subset of mastered attributes** into Dataverse using **Azure Functions, Logic Apps, or Power Automate**.

Each record carries a **master ID** from the MDM system to enable reconciliation, lineage, and duplicate detection. Any conflicting updates from Dynamics are either rejected or routed back to the MDM system based on governance rules.

---

## 3. Is there an out-of-the-box solution for cross-tenant COE observability?

**Answer:**  
No, there is **no true out-of-the-box solution** for cross-tenant COE observability, and that’s by design. COE is scoped **per tenant** for security and isolation reasons.

The correct approach is to build a **central observability layer**. Each tenant runs COE independently, and relevant data—such as environment health, app usage, flow failures, and audit logs—is exported using supported APIs into a **central Azure monitoring layer** like Log Analytics, Azure Monitor, or a Data Lake with Power BI.

This aligns well with the **Microsoft Well-Architected Framework**, especially the **Operational Excellence and Security pillars**, while maintaining tenant isolation.

---

## 4. Instead of rebuilding Power BI reports, can existing BI files be reused?

**Answer:**  
Yes, absolutely. If Power BI reports are built on a clean semantic model, I always prefer **reuse over redevelopment**.

Existing **PBIX files** can be repointed to a new centralized data layer using **parameters or shared datasets**. This avoids duplicating visuals and logic and ensures consistent metrics across environments.

Using **shared Power BI datasets** also improves governance, simplifies maintenance, and accelerates deployment across Dev, QA, and Prod.

---

## 5. How do you handle exceptions or errors in Power Automate?

**Answer:**  
I design flows assuming failure will happen. I use a **Try–Catch–Finally pattern** implemented through **Scope actions**.

- **Try scope:** Core business logic  
- **Catch scope:** Runs on failure or timeout, captures error details  
- **Finally scope:** Cleanup or final notifications  

Errors are logged to **Dataverse or Application Insights**, alerts are sent via **email or Teams**, and retry policies are applied for transient failures. For long-running flows, I also implement **compensation logic** to avoid inconsistent data states.

---

## 6. What is DLP in the Power Platform?

**Answer:**  
DLP stands for **Data Loss Prevention**. It controls how data moves between connectors to prevent sensitive data exposure.

Connectors are grouped into:
- **Business**
- **Non-Business**
- **Blocked**

DLP policies ensure that Business data cannot be accidentally shared with non-approved or personal services. It’s a key governance mechanism in enterprise and regulated environments.

---

## 7. What categories can a data source be placed into in a DLP policy?

**Answer:**  
There are **three categories**:
- **Business:** Enterprise-approved, sensitive data sources (Dataverse, Dynamics 365, Azure services)
- **Non-Business:** Allowed but isolated productivity tools
- **Blocked:** Not allowed due to security or compliance risk  

The categorization is based on **data sensitivity and business risk**, not just technology.

---

## 8. How do you handle mixed audiences (business and technical stakeholders) in the same meeting?

**Answer:**  
I act as a **translator and facilitator**. I start with business outcomes, then translate them into technical terms for IT teams. When technical constraints come up, I explain their **business impact**.

I continuously validate understanding, use examples and UI walkthroughs, and always close with a **clear summary and written follow-up** so both sides stay aligned.

---

## 9. How do you handle out-of-scope requests from customers?

**Answer:**  
I acknowledge the request first, then anchor the discussion back to the agreed scope. If it’s small, I answer it at a high level. If it’s larger, I explain why it needs a separate engagement and document it as a follow-up.

I never say a hard “no”—I provide a **clear path forward** while protecting the engagement boundaries.

---

## 10. How do you keep up to date with Microsoft changes?

**Answer:**  
I follow **official Microsoft release plans**, roadmap updates, and documentation. I stay active in the **community**, validate changes from an architectural perspective, and focus on **customer impact** rather than just features.

I also share learnings with peers, which helps reinforce understanding.

---

## 11. How do you manage time when supporting multiple customers in parallel?

**Answer:**  
I prioritize based on **impact and urgency**, not just calendar order. I separate work into **advisory, discovery, and enablement modes**, document everything after each interaction, and set clear expectations with customers.

That structure allows me to switch contexts efficiently while maintaining quality.

---

## 12. How do you handle ambiguous customer requirements during the first engagement?

**Answer:**  
I treat the first call as a **discovery session**, not a delivery session. I listen carefully, ask open-ended questions, summarize what I hear, and validate understanding before suggesting solutions.

After the call, I document objectives, assumptions, and next steps and share them with the account manager to drive clarity.

---

## 13. Are customer interactions ad-hoc or scheduled?

**Answer:**  
All interactions are **pre-scheduled**. Customers don’t call directly. Meetings are set up by the **Customer Success Account Manager or Microsoft lead**, with context provided in advance.

Most interactions happen via **scheduled Teams meetings**, followed by email-based guidance or follow-up sessions.

---

## 14. Have you worked directly with customers in an advisory capacity?

**Answer:**  
Yes. At Vanguard, I acted as the **primary customer-facing solution architect**, leading design walkthroughs, resolving production issues, and guiding business and IT teams through Dynamics 365 Customer Service implementations.

That customer-facing advisory role is something I’m very comfortable with and enjoy.

---
