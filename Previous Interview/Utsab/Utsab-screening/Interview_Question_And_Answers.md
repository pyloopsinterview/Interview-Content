# Interview Q&A

## 1. Are you aware of GraphQL? What is it?

**Answer:**
Yes, I’m familiar with GraphQL. GraphQL is a query language for APIs that allows clients to request exactly the data they need instead of receiving fixed responses like in REST APIs. This helps prevent over-fetching and under-fetching of data. In GraphQL, we define a schema with types, queries, mutations, and subscriptions, and resolvers handle how the data is fetched from databases or services.

---

## 2. What is Apollo Federation?

**Answer:**
Apollo Federation is an architecture pattern used to build distributed GraphQL systems. Instead of having one large GraphQL server, the schema is divided into multiple smaller services called subgraphs. Each microservice manages its own schema and business logic. An Apollo Gateway then combines these subgraphs into a single unified GraphQL API for the client. This approach works well in microservice architectures because each team can independently manage their services while exposing a single endpoint.

---

## 3. What are GraphQL subscriptions?

**Answer:**
GraphQL subscriptions are used for real-time communication between the client and the server. Unlike queries and mutations, which follow a request-response pattern, subscriptions allow the server to push updates to the client whenever certain events occur. Subscriptions are usually implemented using WebSockets so that the client can maintain a persistent connection with the server.

---

## 4. What are the main operation types in GraphQL?

**Answer:**
There are three main operation types in GraphQL:

* Query – used to fetch data from the server.
* Mutation – used to create, update, or delete data.
* Subscription – used for real-time updates when data changes.

---

## 5. Can you give an example of where GraphQL subscriptions are used?

**Answer:**
Subscriptions are commonly used in real-time applications such as chat systems, notifications, or live dashboards. For example, in a chat application, a client can subscribe to a newMessage event. Whenever a new message is created, the server publishes the event and all subscribed clients receive the update instantly.

---

## 6. Do you have experience with cloud services?

**Answer:**
Yes, I do have experience working with cloud services, mainly in deploying scalable backend applications. In my current project, our backend microservices are deployed in a cloud environment using containerized deployments with Docker. We use cloud infrastructure to run microservices, manage databases, and store application data.

---

## 7. How do you deploy applications in the cloud?

**Answer:**
We typically package applications using Docker containers. These containers ensure that the application runs consistently across development, testing, and production environments. We also use CI/CD pipelines integrated with Git. When code is pushed and pull requests are merged, automated pipelines build the application, run tests, create Docker images, and deploy the services to the cloud.

---

## 8. How does cloud infrastructure help in enterprise applications?

**Answer:**
Cloud infrastructure provides scalability, reliability, and monitoring capabilities. It allows services to scale based on traffic, manage large datasets, and ensure high availability. This is especially important for enterprise applications such as healthcare platforms where performance and reliability are critical.
