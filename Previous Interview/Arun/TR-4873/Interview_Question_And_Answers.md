Below is the full interview Q&A from this conversation reconstructed in **exact question style + strong aligned answers** in a clean **Markdown (.md)** format.

You can copy-paste directly.

---

# **Arun Thakur – Interview Q&A Document (Markdown)**

## **1. Introduce yourself / Tell me about your experience**

**Answer:**
Hi, my name is Arun Thakur. I have 10+ years of experience as a Senior Microsoft Dynamics 365 Developer working primarily with Dynamics 365 CE, C#/.NET development, Power Platform components, and Azure-based integrations.

Currently, I am working with Prudential Financial where I develop and customize Dynamics 365 CE applications using plugins, custom workflows, JavaScript web resources, and Dataverse schema customizations.

One of the major initiatives I support is migrating customer and policy data from Salesforce to Dynamics 365. I work closely with architects to map Salesforce objects, migrate using SSIS and KingswaySoft, and ensure data consistency.

I also integrate Dynamics 365 with Azure Functions and Logic Apps to enable real-time policy updates and event-driven processes, and participate in CI/CD deployments using Azure DevOps.

---

## **2. What is a C# plugin in Dynamics 365?**

**Answer:**
A C# plugin is custom server-side code that runs inside the Dynamics 365 Dataverse event pipeline. It executes in response to events such as create, update, delete, assign, or custom messages.

Plugins extend system behavior beyond out-of-the-box capabilities and are written in .NET/C#.

Typical use cases include enforcing business rules, integrating with external services, data validation during record creation, or automating logic that cannot be achieved by configuration alone.

---

## **3. What part of the Microsoft 365 ecosystem do you work on most day-to-day?**

**Answer:**
My core daily experience is with Dynamics 365 CE custom development. Most of my time is spent implementing C# plugins, JavaScript customizations, Dataverse schema changes, business logic, and Azure integrations.

I use Power Platform components (Power Automate flows, Canvas Apps) mainly in support of CRM processes, but the heavy backend logic and data integrity work is centered in Dataverse and Dynamics CE.

---

## **4. How do you decide what data goes to Dataverse vs SharePoint vs other storage?**

**Answer:**
I evaluate based on data type, volume, cost, security requirements, and performance expectations:

* If the data is relational, transactional, or requires business logic, referential integrity, and row/field security → Dataverse.
* If the data is unstructured such as PDF documents, policy attachments, identity forms, large files, or images → SharePoint.
* Historical, analytical, or high-volume archive datasets → Azure Storage or Data Lake based on architecture.

During the Prudential migration, core customer/policy metadata stayed in Dataverse while policy documents and identity files were stored in SharePoint for cost and performance efficiency.

---

## **5. Describe a scenario when the business requests functionality not available OOTB. What solution approach do you follow?**

**Answer:**
When business requirements exceed out-of-the-box capabilities, I follow a structured approach:

1. Evaluate configuration options first.
2. If limitation exists, extend using plugins, workflows, or Power Automate.
3. For complex logic or external checks, integrate with Azure Functions or Logic Apps.

A real example: Prudential requested a multi-level policy approval workflow tied to policy value thresholds and regional underwriting validation.

The solution was a hybrid approach:

* Dataverse tables for approval stages
* C# plugins for rules and routing
* Azure Functions triggered asynchronously for external validations
* Power App screens + BPF for guided UX

This provided extensibility while keeping solutions maintainable and scalable.

---

## **6. Describe a CRM security challenge you faced during migration and how you resolved it.**

**Answer:**
During the Salesforce migration into Dataverse, regional users received access to records outside their region due to incorrect mapping of ownership and role-based access. This triggered compliance concerns for customer policy data.

To resolve the issue, we redesigned the security model:

* Business Unit hierarchy aligned to regions
* Correct team/owner mappings from Salesforce during ETL
* Field-level security for sensitive attributes
* Plugin-based validation for unauthorized updates
* Auditing enabled for policy-modifying operations
* ETL rules in KingswaySoft enforced correct pre-migration ownership

This ensured that users only accessed region-appropriate records and maintained regulatory compliance.

---

## **7. May I know your availability and notice period?**

**Answer:**
I can start immediately. My current assignment is closing and I do not need more than two weeks' notice. I will be available to begin in January along the expected onboarding timeline.

---

---

If you want next, I can provide:

* full mock interview script
* technical deep-dive answers for UBS/Cinecron
* migration strategy explanation
* plugin execution pipeline + Azure event architecture
* risk and mitigation answers

Just tell me.
