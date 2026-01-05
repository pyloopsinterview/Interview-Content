# Interview Questions & Answers (Exact Flow)

---

## 1. If I have to choose between React and Next.js, which one do you choose?
**Answer:**  
It depends on the project requirements.  
If the application is a client-heavy SPA with minimal SEO needs, I choose React.  
If the application requires SEO, server-side rendering, faster initial load, or structured routing, I choose Next.js. Since Next.js is built on top of React, it provides additional performance and architectural benefits when needed.

---

## 2. Have you heard about the recent Linux security attack and why updates are required?
**Answer:**  
Yes. Recent Linux kernel vulnerabilities have been actively exploited, mainly privilege escalation flaws. These allow attackers to gain root access if systems are unpatched. Updating Linux ensures security patches are applied, preventing ransomware and system compromise.

---

## 3. Can you break down your Research Grant application architecture?
**Answer:**  
The application had a single React frontend (not micro-frontend) and a backend built using multiple Node.js microservices. The frontend was modular but deployed as one app, while the backend services were separated by business domains.

---

## 4. Was the backend built in Node.js with REST APIs?
**Answer:**  
Yes. The backend was built using Node.js and Express, exposing RESTful APIs.

---

## 5. How was the application deployed to object storage/cloud?
**Answer:**  
The React frontend was deployed as a static build to Azure Blob Storage.  
The Node.js microservices were Dockerized and deployed to Azure-managed container services with CI/CD pipelines.

---

## 6. How did you deploy Node.js REST APIs?
**Answer:**  
Each microservice was packaged as a Docker container, pushed to a private container registry, and deployed using Azure’s container services. Configuration was handled using environment variables, and deployments were automated through CI/CD.

---

## 7. When multiple microservices need to interact, how do they communicate?
**Answer:**  
We mainly used REST-based synchronous communication for direct calls and asynchronous event-based communication for workflows. Service-to-service calls were secured, and timeouts and retries were implemented.

---

## 8. How many microservices did you have? Can you name them?
**Answer:**  
Approximately six to seven microservices:
- User & Access Management  
- Grant Request Service  
- Approval Workflow Service  
- Notification Service  
- Audit & History Service  
- Document Management Service  
- Reporting Service (optional)

---

## 9. Did you separate microservices from the beginning?
**Answer:**  
Yes. We identified business domains early and separated microservices accordingly, ensuring clear ownership and loose coupling from the start.

---

## 10. Have you heard about the Backend-for-Frontend (BFF) pattern?
**Answer:**  
Yes. BFF is used to aggregate backend microservices and provide a frontend-optimized API, reducing complexity on the client side and decoupling UI from internal services.

---

## 11. How did you handle large document uploads (500MB–1GB)?
**Answer:**  
The frontend validated files first, then requested a secure, time-limited upload URL from Node.js. Files were uploaded directly from the browser to object storage. The backend stored metadata and managed permissions, not the file stream itself.

---

## 12. How did you show upload progress and validations?
**Answer:**  
Client-side validation handled file size and format. Upload progress was tracked using browser progress events, and percentage completion was shown via a progress bar.

---

## 13. JavaScript puzzle: `for` loop with `setTimeout`. What was wrong?
**Answer:**  
The issue was using `var`, which is function-scoped. All callbacks shared the same variable. Using `let` fixes it because it’s block-scoped, giving each iteration its own value.

---

## 14. How do you use object destructuring?
**Answer:**  
I use object destructuring to extract values from objects cleanly, especially for API responses, function parameters, and React props. It improves readability and reduces boilerplate.

---

## 15. The intention was to print double of each number. Can it be done better?
**Answer:**  
Yes. Using `map` or `forEach` is cleaner and more expressive than a traditional `for` loop.

---

## 16. When do you use Redux vs Context API?
**Answer:**  
Context API is used for simple, low-frequency global state like theme or auth.  
Redux is used for complex, frequently changing business state.  
Using both together in one project is a good practice.

---

## 17. Have you built reusable components?
**Answer:**  
Yes. Examples include a reusable Data Grid, form input components, and modal dialogs used across multiple modules.

---

## 18. Data grid with pagination and sorting — how did you design it?
**Answer:**  
Pagination was server-side with API calls per page.  
Sorting could be client-side (within current page) or server-side (entire dataset), depending on requirements.

---

## 19. Was the data grid a function or class component?
**Answer:**  
It was a functional component using hooks like `useState`, `useEffect`, `useMemo`, and `useCallback`.

---

## 20. Excel-like column filtering with “contains” search?
**Answer:**  
Filters were defined per column. For small datasets, filtering was client-side. For large datasets, filter values were sent to the backend for database-level filtering.

---

## 21. When to use `useMemo` and `useRef`?
**Answer:**  
`useMemo` is used to memoize expensive computations and avoid unnecessary recalculations.  
`useRef` is used to store mutable values or access DOM elements without causing re-renders.

---

## 22. Which libraries did you use to connect Node.js to PostgreSQL?
**Answer:**  
Primarily `pg` for performance and control.  
In some projects, Sequelize ORM was used for productivity and migrations.

---

## 23. How do you handle schema and data validation for large forms?
**Answer:**  
Frontend does basic validation for UX.  
Backend uses schema-based validation.  
Business rules are handled at the service layer.  
PostgreSQL constraints act as the final safeguard.

---

## 24. Why do we use `"use client"` in Next.js?
**Answer:**  
To mark components that require client-side features like state, effects, browser APIs, and user interaction. By default, Next.js uses server components.

---

## 25. Have you faced memory leaks? How did you optimize them?
**Answer:**  
Client-side leaks were handled by cleaning up effects and avoiding unnecessary state.  
Server-side leaks were addressed by proper connection pooling, avoiding global state, and monitoring heap usage.

---

## 26. Do you follow Agile methodologies?
**Answer:**  
Yes. We follow Agile with two-week sprints, daily stand-ups, backlog grooming, sprint reviews, and retrospectives.

---

## 27. Have you worked in an onshore-offshore model?
**Answer:**  
Yes. I worked closely with both teams, ensured clear communication, overlap hours, code reviews, and alignment on requirements.

---

## 28. Programming exercise: Character frequency greater than 1
**Answer:**  
A single-loop solution using an object to count characters and return only those with frequency greater than one.

---

## 29. Are you prepared with the latest Next.js and unit testing standards?
**Answer:**  
Yes. I’m up to date with modern Next.js features and fully aligned with strict testing requirements. I’m used to environments where PRs are rejected unless test coverage meets benchmarks like 75%, especially in healthcare systems.

---
