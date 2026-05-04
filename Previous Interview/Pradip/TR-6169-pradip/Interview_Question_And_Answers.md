# Interview Q&A – Pradip Das

## 1. Which Dynamics apps do you mainly work with?

I primarily work with Dynamics 365 Customer Engagement apps, especially Sales and Customer Service. In recent projects, I’ve focused more on building custom model-driven apps on Dataverse tailored to business processes like patient onboarding and case management. I also use Canvas Apps for mobile and field users, along with Power Automate, Power BI, and Azure integrations to extend the platform.

---

## 2. Have you used plugins or do you rely on Power Automate?

I use both plugins and Power Automate based on the requirement. For real-time, complex, and performance-critical logic, I use Dataverse plugins in C#. For business workflows like approvals, notifications, and integrations, I use Power Automate. I follow a balanced approach instead of relying on one tool for everything.

---

## 3. Why not always use plugins vs flows?

I avoid plugins when the requirement is long-running, integration-heavy, or business-driven workflows. Plugins are not ideal for visibility and maintenance in such cases. I use flows for automation and integrations. However, for real-time validation, transactional consistency, and high performance, plugins are the better choice.

---

## 4. Have you worked with Azure Functions?

Yes, I’ve used Azure Functions extensively as a middleware layer. In my project, I used them to handle data transformation, validation, and secure integration with external healthcare systems. They also helped in error handling, retries, and scalability.

---

## 5. When do you use Azure Functions vs Power Automate vs Logic Apps?

I use Azure Functions for custom logic, scalability, and complex integrations. Power Automate is used for business workflows and quick automation. Logic Apps are used for enterprise-level integrations requiring monitoring, orchestration, and scalability across Azure services.

---

## 6. How do you handle logging and error handling?

In Logic Apps, I use scopes and built-in run history along with Application Insights. In Power Automate, I use scopes and log errors into Dataverse or external systems. In Power Apps, I handle UI-level errors using IfError and log issues into Dataverse or APIs.

---

## 7. What about Application Insights?

Application Insights is my preferred centralized logging solution. I use it to track exceptions, performance, and end-to-end transactions. I integrate it with Azure Functions and sometimes push logs from flows or plugins via APIs. It provides a unified monitoring system.

---

## 8. What is your experience with KQL?

I use KQL to query telemetry data in Application Insights. I use it for troubleshooting, analyzing failures, tracking performance, and building dashboards. It helps in filtering, aggregating, and correlating logs efficiently.

---

## 9. How do you use Azure DevOps?

I use Azure DevOps across the full lifecycle—Agile tracking, repos, code reviews, and CI/CD pipelines. I automate solution deployments across environments using pipelines and Power Platform CLI. I also manage ALM, versioning, and environment governance.

---

## 10. Have you worked with deployment settings files?

Yes, I use deployment settings files to manage environment-specific configurations like connection references and environment variables. This helps in automated, consistent deployments across environments without manual intervention.

---

## 11. What document storage approaches have you used?

I mainly use SharePoint integration for document management. For large-scale or high-performance storage, I use Azure Blob Storage. For lightweight needs, I use Dataverse file columns.

---

## 12. How do you manage deployments to client environments?

I follow a structured ALM approach using Azure DevOps pipelines. Solutions are developed in Dev, exported, and deployed across QA, UAT, and Prod using pipelines. I use deployment settings files, approval gates, and rollback strategies to ensure controlled releases.

---

## 13. Have you handled solution architect-level responsibilities?

Yes, I’ve led technical discussions with stakeholders, translated business requirements into technical solutions, and guided teams. I handled challenges like requirement gaps, migration risks, and changing priorities through clear communication, demos, and structured planning.

---

## 14. How do you handle tight timelines and changing requirements?

I prioritize based on business impact, keep solutions modular, and maintain constant communication with stakeholders. I clearly explain trade-offs and risks to ensure alignment and avoid surprises.
