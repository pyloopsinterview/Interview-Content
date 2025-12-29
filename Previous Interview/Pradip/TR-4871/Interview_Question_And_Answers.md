# Interview Questions & Answers – Pradip Rimal (Dynamics 365 / Power Platform)

---

## Question 1  
**That you would have seen in the past, and how did you overcome those challenges? Could you walk me through that experience? Also, I’d love to know a little bit about your experience in the finance domain.**

### Answer  
One of the biggest challenges I faced was during my time at Huntington National Bank, where Dynamics 365 CRM was used for customer onboarding and internal banking workflows. The main issue was handling large volumes of customer data coming from multiple systems while meeting strict regulatory and security requirements.

We experienced performance bottlenecks, especially during peak hours, because some plugins were synchronous and doing heavy processing. To resolve this, I refactored those plugins by moving non-critical logic to asynchronous execution, optimizing FetchXML and SQL queries, and reducing unnecessary database calls. I also implemented proper logging and error handling.

Another challenge was data security. Different banking teams needed access to the same records but with different visibility levels. I redesigned security roles, business units, and field-level security so users only saw what they were authorized to see.

This experience helped me build secure, high-performing, and scalable CRM solutions that meet financial compliance standards.

---

## Question 2  
**A little bit more on the technical nit-gritty side—when you said you owned the end-to-end architecture, including Power Platform and traditional CRM admin work—how would you describe your expertise there? Where are you stronger?**

### Answer  
When I talk about owning the end-to-end architecture, I break it into two pillars: the core Dynamics 365 CRM foundation and the Power Platform/Azure layer.

On the core CRM side, I’m very strong. I’ve built environments from scratch, including data models, custom entities, relationships, security roles, business units, plugins, workflows, custom actions, forms, dashboards, and solution management across Dev, QA, and Prod.

At Huntington National Bank, I owned the CRM foundation—setting up security models, solution structures, and data access patterns whenever new business units were onboarded.

On the Power Platform side, my experience is enterprise-focused. I work with Power Automate for complex business processes, model-driven apps, Dataverse design, and Power Apps for extending CRM functionality. I also design Azure-based integrations using Azure Functions, Data Factory, and SSIS.

Overall, my strongest area is traditional Dynamics 365 CRM architecture and backend development, with solid expertise in Power Platform and Azure to deliver scalable, cloud-first solutions.

---

## Question 3  
**Since you design the solution from the foundation level, how do you decide what belongs in Dataverse versus SharePoint or other storage? Do you use APIs or an indirection layer while classifying data?**

### Answer  
When designing a Dynamics 365 solution from scratch, I decide data placement based on four main factors.

First, if the data is transactional or relational—such as customers, cases, approvals, or compliance data—it belongs in Dataverse because it needs relationships, security, auditing, and business logic.

Second, if the data is document-heavy or unstructured, like PDFs, contracts, or statements, it goes into SharePoint. Dataverse only stores metadata and references, while SharePoint handles versioning and document management efficiently.

Third, for high-volume or long-term historical data, I use Azure SQL or Data Lake, with Azure Data Factory managing ingestion. Dataverse only holds active or summary data to keep performance optimal.

Finally, I always design with an indirection layer. External systems never talk directly to Dataverse. I use Azure Functions or custom APIs as a middle layer to handle validation, transformation, and throttling. This keeps Dataverse clean and makes future system changes easier.

In short:
- Dataverse for core transactional data  
- SharePoint for documents  
- Azure storage for large or historical data  
- Azure Functions/APIs as the integration layer  

This approach ensures scalability, security, and long-term maintainability.

---
