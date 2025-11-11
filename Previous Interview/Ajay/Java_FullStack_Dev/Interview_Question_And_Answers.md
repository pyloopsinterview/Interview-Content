Below is the complete Markdown (MD) file containing all questions you asked during the interview + strong, senior-level answers.
You can copy-paste this directly into a .md file.
✅ Interview Questions & Answers – Ajay Krishna Ratnavarapu

## 1. Brief Introduction

Hi, my name is Ajay Krishna Ratnavarapu. I’m working as a Java Full Stack Developer with strong experience in Java, Spring Boot, Microservices, React, AWS, and DevOps.
I have led and developed enterprise-scale applications, including the Roofing Warranty Registration & Analytics Platform at GAF, where I designed microservices architecture, integrated AWS services (Lambda, S3, RDS, API Gateway), built scalable frontends using React/Redux, and led an Agile team of 6 developers.
I bring a strong blend of hands-on coding + technical leadership + project management.

## 2. What is your core skill? Java or Frontend?

My core strength is Java and Spring Boot, especially building scalable microservices.
But I also work extensively on the frontend, mainly React (and Angular when required), so I operate as a true full-stack developer.
My backend experience is deeper, but I handle end-to-end delivery across both layers.

## 3. What is Redux?

Redux is a state management library used in React applications.
It centralizes the entire application state into a single store, allowing predictable and consistent state across components.
Core concepts:
Store → holds global state
Actions → events that describe what happened
Reducers → pure functions that update state
Dispatch → triggers an action
Selectors → fetch data from state
Why Redux?
Avoids prop drilling
Predictable behavior
Debuggable with DevTools
Good for large-scale apps

## 4. Difference Between React and Angular

React
Library, not a full framework
Uses JSX
Highly flexible (choose your own architecture)
Faster learning curve
Virtual DOM improves rendering performance
Best for dynamic UI-heavy apps
Angular
Full-fledged framework
Uses TypeScript by default
Has built-in services: routing, forms, DI, HTTP
Steeper learning curve
Great for enterprise-level, structured apps
Summary:
React is flexible and lightweight; Angular is opinionated and complete.

## 5. What is Elasticsearch / OpenSearch?

Elasticsearch / OpenSearch is a distributed search and analytics engine designed for:
Full-text search
Log analytics
Real-time indexing
Filtering large datasets
It stores data as indexes → shards → documents, making queries extremely fast across millions of records.

## 6. How do you fetch 50k records from OpenSearch?

We should never fetch 50k records in one shot (performance + memory issues).
Instead, use:
✔ Scroll API
Used for deep pagination and exporting large datasets.
We fetch data in batches (e.g., 2000 records each).
✔ Search After
Used for real-time pagination without maintaining scroll context.
Batch size recommendation:
2000–5000 per batch for safe memory usage.

## 7. What is a Batch Process? How much data at once?

A batch process means processing data in chunks instead of loading all records.
Why?
Prevents memory overload
Avoids timeout
Keeps system stable
Typical batch sizes:
DB: 1000–2000 per batch
OpenSearch: 2000–5000 per batch
Kafka: 100–1000 messages

## 8. Limitations of AWS Lambda

15-minute max runtime
10 GB memory limit
Cold start latency
Limited disk storage (512 MB–10 GB)
Timeout issues for heavy tasks
Deployment package size limits
No long-running tasks
Stateless execution
Concurrency limits
Large libraries not supported easily
Use Lambda only for short-lived, event-driven tasks.

## 9. What is Multi-Tenancy & How Do You Approach It?

Multi-tenancy means serving multiple customers (tenants) from one application while ensuring isolation.
Approaches:
Separate Database per Tenant
High security, expensive
Separate Schema per Tenant
Good balance
Shared Schema + Tenant_ID
Most scalable
Used by many SaaS systems
How I design it:
Tenant-based filtering (tenant_id in DB)
JPA interceptors for tenant isolation
JWT token carrying tenantId
Tenant-specific configuration
Monitoring & throttling per tenant

## 10. Kafka vs MQTT

MQTT
Lightweight protocol
Designed for IoT devices
Works in low bandwidth
Pub/sub only
Not meant for storage
Kafka
Distributed event streaming platform
High throughput (millions events/sec)
Persistent, replayable
Strong ordering guarantees
Ideal for microservices, analytics
Short answer:
MQTT → IoT messaging
Kafka → Big data streaming & event pipelines

## 11. What is Lazy Loading in Angular?

Lazy loading loads modules only when needed, instead of loading everything at once.
Benefits:
Faster initial load
Better performance
Reduced bundle size
Usage:
{
path: 'admin',
loadChildren: () => import('./admin/admin.module').then(m => m.AdminModule)
}

## 12. What is Virtual Scroll?

Virtual Scroll means rendering only the items visible on screen instead of rendering all items in a list.
If we have 10,000 records, virtual scroll renders only 20–30 at a time.
Benefits:
Faster rendering
Less memory usage
Smooth scrolling
Angular: cdk-virtual-scroll-viewport
React: react-window, react-virtualized
✅ If you want, I can generate this as a downloadable .md file using python — just say “create MD file”.
