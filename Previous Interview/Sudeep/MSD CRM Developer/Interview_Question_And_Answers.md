Below is your complete **Interview Q&A Document** in **Markdown (MD) format**, containing **all the questions you were asked** during the interview along with **well-structured, correct answers** exactly aligned to the responses you practiced.

---

# **Dynamics 365 / Power Platform Interview – Full Q&A (Markdown Version)**

## **1. Give me your introduction.**

I’m Sudeep Chandra, a **Lead Microsoft Dynamics 365 and Power Platform Developer** with over **12 years of experience** delivering enterprise CRM, F&O, AX, and Power Platform solutions. I specialize in **customizations, plugins, JavaScript, integrations, Power Apps, Power Automate, Dataverse, and Azure services**, and I’ve worked with major clients like **Walmart, Albertsons, NextEra Energy, Cisco**, and **Greenbrier**. My focus is on building scalable, secure, cloud-optimized systems through a mix of **architecture, technical leadership, and hands-on development**.

---

## **2. Do you know about DataVerse / DataWars and have you worked on Flows?**

Yes, I have extensive hands-on experience with **Dataverse** for modeling data, relationships, security roles, and automation. I’ve also built numerous **Power Automate Flows**, including complex workflows involving parallel branches, loops, API calls, and system integrations.

---

## **3. What is your current company and project?**

I am working for **Walmart** on the **Dynamics 365 & Power Platform Transformation Project**, handling CRM, Power Apps, Power Automate, Dataverse, and integrations with SAP, Salesforce, and Oracle using Azure services like **Logic Apps, ADF, and Service Bus**.

---

## **4. What is the name of the Walmart project?**

The project name is **Walmart Dynamics 365 & Power Platform Transformation**.

---

## **5. What is a Model-Driven App and what is a Data-Driven App?**

- **Model-Driven Apps** are data-first applications built on Dataverse where UI is automatically generated based on the data model. Ideal for complex business processes.
- **Data-Driven Apps (Canvas Apps)** allow full control over UI with drag-and-drop components and can connect to multiple data sources.

---

## **6. What are the major differences between Model-Driven and Canvas Apps?**

- Model-Driven: Data-first, structured UI, built on Dataverse, suitable for enterprise workflows.
- Canvas: UI-first, pixel-perfect design, connects to many data sources, flexible user experience.

---

## **7. What are Model-Driven Apps and Canvas Apps?**

- **Model-Driven Apps** rely on Dataverse entities and relationships.
- **Canvas Apps** are highly customizable apps with a free-form interface.

---

## **8. What is PowerApps?**

Power Apps is Microsoft’s **low-code platform** to build Canvas Apps, Model-Driven Apps, and Custom Pages using Dataverse or external connectors. It supports advanced logic with Power Fx, custom connectors, and integrations with Power Automate.

---

## **9. Tell me about your current project.**

I lead Dynamics 365 CRM, Power Platform, and integration work for Walmart. My responsibilities include **custom plugins, JavaScript, custom pages, Power Apps, Power Automate flows, Azure-based integrations, data migration, DevOps pipelines**, and omnichannel/retail solutions.

---

## **10. What is your tech stack?**

My stack includes:

- **Dynamics 365 CRM, AX/F&O**
- **C#, .NET, JavaScript, Plugins, HTML, CSS**
- **Power Apps, Power Automate, Dataverse, Power Pages**
- **Azure ADF, Logic Apps, Service Bus**
- **SQL Server, SSRS, SSIS, KingswaySoft**
- **Git, Azure DevOps CI/CD**

---

## **11. Was your customization mostly complex or out-of-the-box?**

A mix of both.
I use OOB features where possible, but most enterprise scenarios require **complex customization**, including plugins, JavaScript, PCF controls, integrations, Liquid templates, and Power Automate flows.

---

## **12. Do you have experience with Liquid, Liquid Templates, Bootstrap, and CSS?**

Yes.
I use **Liquid** for dynamic Power Pages, **Bootstrap** for responsive layouts, and **CSS** for custom styling. I also add **JavaScript** for validations and dynamic UI behavior.

---

## **13. Have you modified Authentication in Power Pages?**

Yes.
I’ve worked with **Azure AD, B2C, OAuth providers**, and customized login pages using Liquid, JavaScript, and custom redirects. I configured web roles, Dataverse security, and custom registration flows.

---

## **14. Do you have experience with Field Service?**

Yes.
I’ve configured **Work Orders, Bookings, Assets, Scheduling**, customized forms with plugins/JS, integrated Field Service with ERP systems, and worked with mobile app customizations and RSO.

---

## **15. When was the last time you wrote a plugin?**

Very recently.
I write plugins **weekly** in my current Walmart project for validations, integrations, auto-calculations, and business logic.

---

## **16. Scenario: Fetch 1000 Contact records and update State lookup. What steps do you follow?**

1. Fetch records using FetchXML + RetrieveMultiple.
2. Create an `EntityReference` for the “Maharashtra” state lookup.
3. Loop through the entity collection.
4. Create an entity object with the ContactId + updated lookup field.
5. Call `service.Update()` (or use ExecuteMultiple for batch updates).

---

## **17. Scenario: Send an Employee object (phone, email, address) to an Action. How can we achieve this?**

Actions only accept primitive types or EntityReference.
To send a complex object:

- Serialize the Employee object into **JSON**
- Pass it as a **string parameter**
- Inside the plugin, retrieve it and **deserialize** into a C# Employee object

This is the most scalable approach.

---

## **18. Have you written complex flows? When is a plugin better than a flow?**

Yes, I’ve built complex flows involving loops, parallel logic, API calls, and approvals.
A plugin is better when:

- Real-time validation is needed
- High-performance logic is required
- Large data volumes
- Pre-operation logic
- Complex server-side business rules
- Synchronization with external systems

---

## **19. What type of role are you expecting (Lead, Architect, Developer)?**

I’m comfortable with a mixed role:

- **40% Architecture**
- **40% Technical Lead**
- **20% Hands-on Development**
  And I’m comfortable working under a client architect with shared decision-making.

---

## **20. Do you use Git in your current project?**

Yes, daily.
I work with branching strategies, pull requests, code reviews, merge conflicts, CI/CD pipelines, and solution versioning.

---

## **21. Do you understand solution packing/unpacking and unmanaged solutions?**

Yes.
I use Solution Packager and Azure DevOps pipelines to pack/unpack CRM solutions, and I fully understand unmanaged vs managed approach. We use **unmanaged** for development in complex implementations.

---

## **22. Reporting, Data Management, and Data Migration Experience?**

Yes.

- **Power BI**, **SSRS**, Dataverse reporting
- **ADF, KingswaySoft, SSIS**, DIXF/DMF
- Data modeling, cleansing, mapping, pre/post validation, and large-scale migrations

---

## **23. How many years of experience do you have with Canvas Apps?**

Approximately **7 to 8 years** of deep, hands-on Canvas App development.

---

# **End of Document**

If you want, I can also:

- Format this as a **downloadable MD file**
- Convert it into **PDF**, **DOCX**, or **professional notes**
- Create a **short revision version** for last-minute prep

Just tell me.
