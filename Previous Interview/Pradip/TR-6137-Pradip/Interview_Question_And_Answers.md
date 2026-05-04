# Pradeep Das – Interview Q&A

## 1. Tell me about your background
Hi, this is Pradeep Das. I’ve been working with Dynamics 365 and the Microsoft ecosystem for about 11 years now, mostly in a techno-functional role.

Currently, I’m working with Health Book as a Lead Dynamics 365 and Power Platform Developer, where I mainly support a live production environment. My day-to-day work involves handling customer accounts, renewals, and revenue-related processes, so I’m very comfortable working on business-critical systems.

Recently, we went through a go-live and hypercare phase, and my main responsibility was to keep the system stable and quickly resolve production issues, especially anything impacting customer renewals or revenue.

For example, during a peak renewal period, customers were submitting renewals through the Power Pages portal, but the backend processing stopped. From the user side, everything looked fine, but the data wasn’t reaching Finance & Operations, so invoices weren’t getting generated.

I started troubleshooting end-to-end, tracing the flow from Power Pages to Power Automate, then Dataverse, and finally into Finance & Operations. I found that a service account used by multiple cloud flows had an expired authentication token, which caused silent failures and created a backlog.

I fixed the connection, reprocessed the failed transactions, and worked with the finance team to reconcile the missing invoices. After that, I set up proper monitoring and alerts to catch such issues immediately in the future.

Since then, my focus has been on ongoing operations—monitoring integrations, troubleshooting issues, supporting business users, and coordinating with Microsoft when needed.

I also mentor junior team members and contribute to reusable solutions to improve delivery speed.

Overall, my strength is handling production support during hypercare, quickly identifying root causes, and ensuring system stability while protecting critical revenue flows.


## 2. How do you handle post-production issues and troubleshooting?
In post-production, especially during hypercare, the first thing I focus on is understanding the impact and scope of the issue.

I start by checking if it’s a user-specific issue or system-wide. If multiple users are affected, it’s treated as a high-priority system issue.

Next, I try to reproduce the issue and trace the flow end-to-end—from UI to Dataverse, plugins, workflows, Power Automate, and integrations like F&O.

I check logs such as plugin trace logs and flow run history to identify where the failure is happening.

If it’s a configuration or data issue, I fix it directly. If it’s a code issue, I evaluate whether a hotfix or rollback is required.

If a recent deployment caused the issue, I roll back to the last stable version while fixing the issue in lower environments.

I also ensure proper communication with business users and implement monitoring and alerts to prevent future issues.


## 3. Tell me about a post-go-live stabilization project you led
One example is from my current project with Health Book during the hypercare phase.

During peak renewal time, customers submitted renewals through Power Pages, but the data was not reaching Finance & Operations, so invoices were not generated.

I validated that it was a system-wide issue and traced the entire flow—from Power Pages to Power Automate, Dataverse, and F&O.

I found that a shared service account used in cloud flows had an expired authentication token, causing silent failures.

I fixed the connection, reprocessed transactions, and worked with finance to reconcile missing invoices.

Then I implemented monitoring and alerting to prevent recurrence.

This ensured system stability and protected the revenue flow during a critical business period.


## 4. Give an example of a design-level issue you handled
At KeyBank, we had an issue with payment transaction processing.

The system design allowed multiple transaction records to be created during updates or retries, leading to duplicate and inconsistent data in production.

The code was working as designed, but the design itself was flawed.

I analyzed the system and proposed a redesign to maintain a proper transaction lifecycle—updating or deactivating records instead of creating duplicates.

I updated the plugin logic, tested it thoroughly, and deployed it in a controlled manner.

I also cleaned up existing data and validated results with business users.

Additionally, I updated the design documentation to reflect the changes.

This ensured long-term stability and maintainability of the system.


## 5. When can you join?
As per my current engagement, I would need to give a standard two-week notice period.

However, I understand the urgency and can be flexible. I can try to transition quickly and join within 1 to 2 weeks.

If required, I can also provide partial availability during the transition period to ensure a smooth handover.
