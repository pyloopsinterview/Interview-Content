# Interview Q&A Summary

## 1. What you've been working on, and a little bit about your experience?

**Answer:**  
Sure, sure. Sounds good. So let me start with my experiences. I have more than 14 years of experience working as a Lead Full-Stack Java Developer.  
My core skills focus on **Java and Java frameworks** like Spring and Spring Boot. I’ve worked with both **monolithic** and **microservices architectures**, including migrating large-scale monolithic applications into microservices.

I’ve implemented **REST APIs** and also used **GraphQL** for queries and mutations. On the frontend, I’ve worked with **Node.js** and **React**.

In **AWS**, I’ve used around 25–30 services — such as API Gateway, Lambda, SNS, SQS, RDS, EC2, CodeBuild, CodePipeline, and CodeCommit. I’ve created CI/CD pipelines using **GitLab** and **GitHub Actions**.

I also have experience containerizing applications with **Docker** and deploying them using **EKS** and **ECS**.

Currently, I’m working with **Verizon**, leading a design and development team for an enterprise app platform supporting both customer-facing and internal operations.  
One of the projects involves a **Customer Order Orchestration and Fulfillment System**, which handles millions of transactions per day. I lead a team of six developers and an architect, migrating the system from monolithic to **microservices** using **Spring Boot, Kafka, and AWS EKS**, with **React** on the frontend.

---

## 2. Are you currently a contractor?

**Answer:**  
Yes, I’m a contractor. That’s right.

---

## 3. Is your contract ending or are you just looking for something different?

**Answer:**  
Yeah, my contract is going to end soon. That’s the main reason I’m exploring new opportunities.  
Things are pretty stable now, and there aren’t many new features being rolled out. Full-time developers are maintaining it, so I’m open to the next challenge.

---

## 4. What language did you use for your AWS Lambda functions?

**Answer:**  
I’ve primarily used **Java**, but I’ve also written some Lambdas in **Python**. The majority are Java-based.

---

## 5. How much experience do you have with Node.js?

**Answer:**  
I have strong hands-on experience with **Node.js**, **Express.js**, and **Next.js** for writing REST APIs and using middlewares.

---

## 6. How long have you worked with Node.js?

**Answer:**  
Around **7+ years** of experience with Node.js, including building REST APIs.  
Even though Lambda functions work a bit differently, conceptually they’re similar — we just need to define a handler and business logic.

---

## 7. How long have you worked with React?

**Answer:**  
Around **8 years**.  
I’ve worked with both **class-based** and **functional components**, used **Redux**, and leveraged **React Hooks** since React 16 for managing state.  
Currently, I mainly use **functional components** in my projects.

---

## 8. Tell me about the most difficult, challenging, or innovative thing you’ve worked on.

**Answer:**  
One instance was while building a **PUT API** for a campaign registration system.  
REST APIs typically shouldn’t allow partial updates, but we needed that flexibility. The team was stuck, so I proposed fetching the full record first (via GET), updating the necessary fields locally, and then sending the entire object back using PUT.  
This avoided partial updates while maintaining REST standards and clean code.

Another major challenge was **performance optimization** in report generation.  
We had multiple joins across tables, which slowed down performance.  
I:

- **Denormalized data** to reduce joins
- **Added indexes** after analyzing query plans
- Introduced a **read-only replica** of the database for report generation

This led to a **~40% improvement in performance**.

---

## 9. Why didn’t you use materialized views for that?

**Answer:**  
That’s a valid point. We considered it, but the data was **highly dynamic and real-time**, coming from multiple streams.  
Materialized views wouldn’t stay in sync with that level of frequent updates, so we opted for denormalization and a read-only replica approach instead.

---

## 10. Tell me about a weakness you have.

**Answer:**  
Sometimes I get **impatient** when things don’t work as expected.  
When that happens, I take a short break (10–30 minutes) to calm down and reset before returning to the task with a clear mind.

---

## 11. What would you like to learn more about?

**Answer:**  
I’m very interested in **AI and Machine Learning**.  
I’ve experimented with **training models**, **data preparation**, and even worked with **LLMs** personally.  
Although I haven’t implemented AI/ML in production yet, I’m actively learning and exploring that area.

---

## 12. Have you done much with code reviews?

**Answer:**  
Yes, absolutely. I’m involved in **pull request (PR) reviews** and **pair programming** as part of our Agile process.

During reviews, I focus on:

- **Function boundaries** and modular design
- **Naming conventions** and readability
- **Error handling** and **security checks**
- **Performance optimization**
- **Test coverage** to ensure regression safety

I also encourage my team to give feedback on my code to foster collaboration and continuous improvement.

---

## 13. How do you handle different types of error situations in your code?

**Answer:**  
I use a **centralized error-handling mechanism** — typically via **interceptors** or global handlers.

Types of errors and handling:

- **Business logic errors** (e.g., validation failures): handled with meaningful responses.
- **System errors** (e.g., DB timeouts, Kafka failures): handled with **retry mechanisms** and **circuit breakers**.
- **Unexpected errors**: logged in detail and return standardized **500 responses**.

Logging and monitoring are critical to troubleshooting and improving system reliability.

---

## 14. Do you have any questions for us?

**Answer:**  
Yes, I do.

1. What are your **expectations** from me in this role?
2. Will I get **ownership** of modules, or will it be more of a task-based execution role?
3. If I get ownership, can I decide the **best approach** to implement the stories and then get reviews or feedback later?

---

**End of Interview Notes**
