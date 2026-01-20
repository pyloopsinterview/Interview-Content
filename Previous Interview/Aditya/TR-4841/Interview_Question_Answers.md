# Interview Questions & Answers – Senior Backend Wagtail Developer

---

## 1. How do you host your Django and Wagtail applications?

**Answer:**  
We host our **Django** and **Wagtail CMS** applications on **Google Cloud Platform (GCP)**. The applications are fully **containerized using Docker**, ensuring **environment consistency** across **development**, **staging**, and **production**. Deployments are automated using **CI/CD pipelines with Cloud Build**, which handle **testing**, **migrations**, and **rollouts** in a controlled and repeatable way.

---

## 2. Are these websites or apps? What kind of platform are you building?

**Answer:**  
These are **web applications**, not mobile apps. We’re building **server-rendered Django and Wagtail websites** that manage **public-facing healthcare content** and **internal editorial workflows**. The platform is dynamic, supports **multi-site architecture**, and serves multiple business units from a **single codebase**.

---

## 3. What type of content do you manage in Wagtail?

**Answer:**  
It’s a mix of **articles**, **informational pages**, and **highly structured healthcare content**. Most of the value comes from **custom content models** and **StreamField blocks** used for **plan details**, **FAQs**, **provider information**, and **regulatory disclosures**. This ensures **consistency**, **compliance**, and **reusability** across sites.

---

## 4. How many editors use these applications?

**Answer:**  
I don’t have exact numbers, but there are **dozens of active editors** across multiple business units. Editors are spread across **authors**, **reviewers**, and **publishers**, often working in parallel. The system is designed to support **concurrent editorial activity** and scales as new sites are added.

---

## 5. Are the Wagtail blocks shared across multiple sites?

**Answer:**  
Yes, the **StreamField blocks** are **multi-site and reusable**. The **data structure is defined once** in shared Django apps, while **rendering and styling** can vary by site. This provides **consistency** and **maintainability**, while still allowing **site-specific presentation**.

---

## 6. Do you handle front-end development, or is there a separate team?

**Answer:**  
It’s a **collaborative effort**. I’m very **hands-on with front-end work** related to **templates**, **component structure**, and **content rendering**. Design and UX teams provide **mockups and branding**, and a front-end team helps with styling, but I own the **integration between Wagtail content and the UI**.

---

## 7. How do you handle different themes or styling across sites?

**Answer:**  
We separate **content structure from presentation**. Components are shared, but each site has its own **theme layer**, including **colors**, **fonts**, and **layout rules**. This is handled through **base templates**, **site-specific templates**, and **CSS**, allowing each site to look distinct while sharing the same backend logic.

---

## 8. Are these sites for sub-brands or subsidiaries?

**Answer:**  
No, all sites are for **Molina Healthcare** itself. They support **state-level organizations**, **business units**, and **audience-specific experiences**, all under the same brand, with **localized content and compliance requirements**.

---

## 9. What admin customizations have you done in Wagtail that you’re proud of?

**Answer:**  
I built **custom editorial workflows** in the **Wagtail admin**, including **multi-step approvals**, **role-based permissions**, and improved **versioning and auditability**. I also added **custom validations**, **admin panels**, and **editor guidance** to reduce errors and support **healthcare compliance**.

---

## 10. How do you host static assets and media assets?

**Answer:**  
We use **Google Cloud Storage** for both **media assets** (images, PDFs, documents) and **static assets** (CSS, JS). A **CDN layer** sits in front to improve **performance and caching**. Wagtail stores only **metadata** in PostgreSQL, keeping the system efficient.

---

## 11. Do you deal with large volumes of documents?

**Answer:**  
Yes, absolutely. We manage **hundreds of gigabytes** of documents, including potentially **hundreds of thousands of PDFs**. **Cloud Storage** is ideal for this scale, offering **durability**, **cost efficiency**, and **easy access control**.

---

## 12. What kind of RAG or LLM work have you done?

**Answer:**  
We focus on **internal use cases**, such as **intelligent search**, **content discovery**, and **editorial assistance**. Using **RAG-based approaches**, we allow users to ask **natural language questions** over approved documents and get **grounded answers**. We also explore **content summarization** and **automation**, always prioritizing **accuracy and compliance**.

---

## 13. Can you walk through your code release pipeline?

**Answer:**  
We follow a **feature-branch workflow** with **pull requests and code reviews**. Approved changes trigger **Cloud Build CI/CD pipelines**, which run **tests**, build **Docker images**, and deploy to **dev → staging → production**. Releases follow a **planned cadence**, with monitoring and rollback strategies in place.

---

## 14. Do your websites have forms?

**Answer:**  
Yes, but they’re **carefully controlled**. Forms are typically **contact**, **feedback**, or **request-based** forms. We use **Django forms** and **Wagtail form pages**, with strong **validation**, **CSRF protection**, and **rate limiting**.

---

## 15. Where does form data go?

**Answer:**  
Form data does **not live long-term in Wagtail**. The CMS acts as an **entry point**, and submissions are **routed to downstream systems**, such as **internal APIs**, **ticketing systems**, or **secure workflows**. Wagtail is not used as a **system of record**.

---

## 16. How big was your engineering team?

**Answer:**  
The backend team was around **4–6 engineers**, including me as the **lead**. We worked closely with **2–4 front-end engineers**, plus **QA**, **product owners**, and **content teams**. It was a **cross-functional, collaborative setup**.

---

## 17. How would you describe the team overall?

**Answer:**  
It was a **very strong team**—technically solid, collaborative, and reliable. Everyone took **ownership**, communicated well, and understood the importance of **stability and compliance** in a healthcare platform.

---

## 18. Do you have any final questions?

**Answer:**  
I feel I have a **clear understanding** of the **application**, **technical expectations**, and **team structure**. I’d just like to know the **next steps**, including **timeline** and **feedback process**.
