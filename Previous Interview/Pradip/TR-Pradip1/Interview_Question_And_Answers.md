# Interview Questions and Answers – Dynamics 365 CI Journeys

## 1. What are POCs?
**Answer:**  
POCs stand for **Proof of Concepts**. A POC is a small, focused implementation used to validate whether a specific tool, technology, or approach will work for a business requirement before committing to a full-scale rollout.  
In Dynamics 365 Customer Insights – Journeys, a POC typically validates segmentation, journey triggers, communication orchestration, consent handling, and CRM integrations to reduce risk and confirm feasibility.

---

## 2. Suppose a customer upgrades mid-month and the billing looks correct but the revenue is overstated. How do you debug?
**Answer:**  
I would separate billing accuracy from revenue recognition and trace the full lifecycle:
1. Validate contract terms, upgrade effective date, and pricing rules.
2. Compare billing events against revenue schedules.
3. Review proration and revenue recognition logic.
4. Reconcile revenue day-by-day to detect double counting.
5. Verify deferred versus earned revenue postings.  
This approach usually identifies whether revenue is being overstated due to incorrect proration or recognition timing.

---

## 3. How do you design a meaningful customer journey in AI Journeys rather than just a linear campaign?
**Answer:**  
I start with the business outcome, not the tool. I define clear entry criteria based on events or behavior, design journeys as decision trees with conditional branching, use timing and throttling intentionally, embed consent and compliance checks, and connect journeys to downstream CRM actions.  
A meaningful journey is adaptive, event-driven, and outcome-focused—not a simple send-and-forget campaign.

---

## 4. What are the key differences between outbound marketing and real-time journeys in Dynamics 365 Customer Insights?
**Answer:**  
Outbound marketing is batch-driven and schedule-based, relying on static or scheduled segments and linear flows.  
Real-time journeys are event-driven and behavior-based, reacting instantly to customer actions, using dynamic branching, contextual personalization, and continuous consent checks.  
Outbound marketing suits planned campaigns, while real-time journeys support lifecycle, onboarding, and personalized engagement.

---

## 5. How would you integrate CI Journeys within an existing Dynamics 365 CRM setup?
**Answer:**  
I treat CRM as the system of record and align the data model first. I use Dataverse events to trigger real-time journeys from CRM actions, integrate consent and preference management, enable two-way data updates between Journeys and CRM, and handle external integrations via Azure services.  
I validate the setup through PoCs and establish governance to ensure scalability and compliance.

---

## 6. Are we done with the questions, and what happens next?
**Answer:**  
Yes. The recruiter indicated they would submit the resume to the client and follow up afterward. I acknowledged and expressed appreciation, confirmed availability for next steps, and readiness to provide additional information if needed.
