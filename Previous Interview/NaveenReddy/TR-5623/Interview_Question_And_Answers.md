# Full Stack Interview – Questions & Answers

## AFETR INTRODUCTION

## 1. How much time have you spent developing using React or Next.js?

**Answer**

In my recent project at Gilead Sciences, my primary focus was on backend development using Node.js microservices, but I also spent around **30–40% of my time working on React-based frontend development**.

I worked on building reusable UI components, integrating REST APIs, and implementing dashboards that allowed research teams to visualize clinical study data. I collaborated closely with the frontend team to design efficient API contracts.

I also have experience with **Next.js**, mainly for **server-side rendering and performance optimization**, although most dashboards were built as **React SPA applications**.

---

## 2. Have you used Next.js or classic React.js?

**Answer**

Yes, I have worked with **Next.js** in previous projects. We used it mainly for **server-side rendering, improved routing, and performance optimization**.

Next.js provided features like **file-based routing, server-side rendering, and optimized page loading**, which helped improve application performance.

---

## 3. If a page’s content changes frequently, what rendering strategy should be used?

**Answer**

If the page content changes frequently and must always show the latest data, the best strategy is **Server-Side Rendering (SSR)**.

With SSR, the page is rendered on the server for each request, ensuring users receive the most up-to-date content.

In Next.js, SSR can be implemented using **getServerSideProps**.

---

## 4. How do you enable Server-Side Rendering in Next.js?

**Answer**

In Next.js, SSR is enabled by exporting a function called **getServerSideProps** inside the page component.

When this function is present, Next.js automatically renders the page on the server for every request.

---

## 5. When using Static Site Generation, when are files generated?

**Answer**

With **Static Site Generation (SSG)**, pages are generated during the **build time** when running the build command such as **next build**.

Next.js pre-renders the HTML files and serves them directly from the server or CDN.

---

## 6. How is routing implemented in Next.js?

**Answer**

Next.js uses **file-based routing**.

Routes are automatically created based on the files inside the **pages directory**. For example:

* `pages/about.js` → `/about`
* `pages/product/[id].js` → dynamic routes like `/product/1`

Navigation is done using the **Link component**, and route parameters can be accessed using the **useRouter hook**.

---

## 7. What state management strategy did you use?

**Answer**

We used a combination of:

* **Redux** for global application state
* **React Context API** for lightweight shared state
* **React hooks (useState, useReducer)** for component-level state

Redux helped manage centralized state such as authentication and shared application data.

---

## 8. How does Redux work?

**Answer**

Redux manages application state through a centralized store.

The lifecycle flow is:

1. User triggers an action
2. Component dispatches an action
3. Reducer processes the action
4. Store updates the state
5. UI re-renders with updated state

Redux ensures **predictable state management and unidirectional data flow**.

---

## 9. How do microservices communicate with each other?

**Answer**

Microservices primarily communicate using **REST APIs over HTTP**.

Each service exposes APIs which other services consume. In some cases, **asynchronous messaging** is used for background tasks and event-driven workflows.

---

## 10. Should Order Service call Inventory Service synchronously or asynchronously?

**Answer**

The call should be **synchronous** because the system must verify inventory availability before continuing the checkout process.

---

## 11. Should Order Service call Payment Service synchronously or asynchronously?

**Answer**

This call should also be **synchronous** because payment confirmation is required before the order can be finalized.

---

## 12. Should Notification Service and Warehouse Service be synchronous or asynchronous?

**Answer**

These services are typically **asynchronous** because they are not part of the critical checkout path.

Order Service can publish an event such as **Order Confirmed**, and these services process the event independently.

---

## 13. What if we don't want to use message queues?

**Answer**

If message queues are not used, services can communicate using **direct REST API calls**.

However, this approach introduces tighter coupling and reduces fault tolerance.

---

## 14. What is the flaw of using async API calls instead of message queues?

**Answer**

The main issues include:

* No guaranteed delivery
* Risk of request loss if service is down
* Tight service coupling
* No buffering for traffic spikes

Message queues provide **reliability, buffering, and fault tolerance**.

---

## 15. Do you have experience with caching?

**Answer**

Yes, we used **Redis** as a distributed caching system.

Frequently accessed data was cached to reduce database load and improve performance.

---

## 16. What caching strategy did you use?

**Answer**

We mainly used the **Cache-Aside (Lazy Loading) pattern**.

The application first checks the cache. If data is missing, it fetches it from the database and stores it in the cache.

---

## 17. What Azure services have you used?

**Answer**

I have worked with:

* Azure App Service
* Azure Functions
* Azure Storage (Blob Storage)
* Azure Service Bus
* Azure Monitor
* Application Insights
* Azure DevOps for CI/CD

---

## 18. How was the frontend deployed in Azure?

**Answer**

The frontend was deployed using **Azure App Service** with a CI/CD pipeline connected to the Git repository.

---

## 19. How were Node.js services deployed?

**Answer**

Each **Node.js microservice** was deployed independently to **Azure App Service**, allowing independent scaling and management.

---

## 20. How does the frontend call backend services?

**Answer**

Frontend applications call backend APIs using **HTTPS REST APIs**.

Requests are made using tools like **Axios or Fetch API**, and responses are returned as JSON.

---

## 21. Do you have experience with Infrastructure as Code?

**Answer**

Yes, we used **Azure Resource Manager (ARM) templates** to define infrastructure resources such as App Services, Storage, and messaging services.

---

## 22. What experience do you have writing pipelines?

**Answer**

We used **Azure DevOps YAML pipelines** to automate the build and deployment process.

The pipeline included stages for:

* Build
* Testing
* Artifact creation
* Deployment

---

## 23. Did you write YAML manually or use templates?

**Answer**

We started with pipeline templates and then customized the **YAML files manually** to meet project requirements.

---

## 24. Are there AI capabilities in your project?

**Answer**

Yes, the platform integrates **AI-based analytics for clinical research data**.

Machine learning models developed by data scientists were integrated into the platform via **Node.js APIs** and visualized in React dashboards.

---

## 25. What database technologies have you used recently?

**Answer**

We used both:

* **PostgreSQL** for relational data
* **MongoDB** for semi-structured or flexible data

---

## 26. Why did you use MongoDB?

**Answer**

MongoDB was used because it provides a **flexible document schema**, supports **JSON-like data structures**, and scales horizontally.

It works well with Node.js applications.

---

## 27. For user data, should we use MongoDB or MySQL?

**Answer**

For core user data such as authentication and roles, **MySQL or other relational databases are usually preferred** because they provide strong consistency and relational integrity.

MongoDB is better suited for **flexible or semi-structured data**.
