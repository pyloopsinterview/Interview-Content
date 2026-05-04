# Interview Questions & Answers (Dynamics 365 / Power Platform / Plugins)

_Source Transcript:_ fileciteturn10file0

---

## 1. Tell me about your experience in Power Platform.
**Answer:**
I have around 11 years of experience working in the Microsoft ecosystem, mainly focused on Dynamics 365, Power Platform, and building enterprise solutions including plugins, workflows, and integrations.

---

## 2. What are plugin execution stages?
**Answer:**
- Pre-validation: Before security checks
- Pre-operation: Before database commit
- Post-operation: After data is committed

---

## 3. Explain a plugin you developed.
**Answer:**
I developed plugins for business logic automation such as validations, integrations, and workflows, ensuring real-time execution and consistency.

---

## 4. What plugin exception did you face recently?
**Answer:**
I encountered a null reference exception due to missing object initialization and resolved it by adding proper null checks and validation.

---

## 5. How do you integrate external APIs in Dynamics 365?
**Answer:**
Using plugins or Power Automate to call external APIs, handling authentication, request/response processing, and ensuring secure communication.

---

## 6. Why async plugin causes timeout but sync works fine?
**Answer:**
Because async runs outside transaction and depends on system resources, queue delays, or retries. Timeout may occur due to heavy processing or service delays.

---

## 7. How to call external API securely in Power Automate?
**Answer:**
Using authentication mechanisms like OAuth, API keys, Azure Key Vault, or secure connectors.

---

## 8. Difference between HTTP action and Custom Connector?
**Answer:**
- HTTP: Quick and direct API call
- Custom Connector: Reusable, structured, secure, and scalable integration

---

## 9. Explain Dataverse security.
**Answer:**
- Business Units define data boundaries
- Security Roles define permissions
- Access levels: User, BU, Parent-Child BU, Organization

---

## 10. Do you have CI/CD pipeline experience?
**Answer:**
Yes, I used pipelines with Azure DevOps for solution deployment across environments (Dev, QA, UAT, Prod).

---

## 11. How do you implement rollback in managed solutions?
**Answer:**
By maintaining versioning and redeploying previous stable solution versions.

---

## 12. What are next steps?
**Answer:**
Interview feedback will be shared and next steps communicated accordingly.

---

