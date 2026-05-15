(Transcribed by TurboScribe. Go Unlimited to remove this message.)

[Speaker 1]
I am also working extensively with the Postgres SQL and the MongoDB for handling the large-scale transactions and analytical data and also involving optimizing API performance, implementing the monitoring using Datadog, AWS X-Ray and improving overall system reliability and throughput. And apart from that, on the front-end side, I have a great experience in React, Vue, a little bit on Angular also, and so, yeah, that's pretty much all.

[Speaker 2]
Okay. So, you're currently working in which company? Sorry, I did not get that.

[Speaker 1]
I'm very source version.

[Speaker 2]
Okay. Okay. Got it.

So, okay. Take one of the recent project, right, whichever, the project which you recently, like, just, you can tell me, like, what was your role and what was the architecture of the project and how did you contribute, right? What was the themes?

[Speaker 1]
I just wanted to understand, like, how, what was your contribution and how do you fit in our team, right? So, we can take one recent project and tell me, like, what was your role and what was the architecture for the project and et cetera. Yeah, sure.

Like, so, like, one of my recent project was with a very source version was, like, I worked as a lead project developer and architect. Like, the project was mainly focused on pharmaceutical order processing, pricing, and, like, validations, compliance check, and, like, supply chain operations across the U.S. And, like, when I joined the project, like, the application was mostly on, like, monolithic, and we are, like, facing scalability and some, like, performance issues, especially, like, during the, we can say, high-volume order processing. So, like, our team, like, decided to redesign the entire platform, like, into the microservices-based and even-driven architectures. So, from the architecture side, like, we used Python with the fast API, like, for developing the backend microservices, and each services has its own responsibilities, like pricing services, order validation services, and also, like, we have inventory services and some, like, fulfillment services.

And for communications between services, we used Kafka as a, like, messaging system. And so, like, instead of, like, direct synchronous communication everywhere, like, services were, like, we can say, like, publishing and consuming events are synchronously, which is, like, which improve the scalability and reduce the system's dependencies. For deployment and infrastructure, we use AWS extensively, like, the services were, like, contentized using Docker and deployed on, like, Kubernetes, EKS, and ECS target, and we also use AWS Lambda for lightweight event-driven processing.

For the database, like, we used PostgreSQL, like, for transactional and relational data and MongoDB, like, for the handling, same structured operational data. Generally, like, my role in this project was mainly focused on, like, designing the backend architectures, designing the REST APIs, developing the fast API-based microservices, Kafka integrations. And I've also, like, worked closely with the front-end team, like, over using Vue.js dashboards, like, for internal operations. And, like, the team's eyes was with around, like, six to eight members of the team, like, we have backend developers, front-end, one BA, QA, and one manager. So, these are, like, things. Okay.

So, were you far away? Is there a team behind you? Or, like, you are, like, working as, like, people who are contributing?

I don't know. Like, in that project, basically, like, there was a team working along with me. Like, I was not working individually.

In this project, like, we worked as a, like, collaborative Agile team. Like, since, like, I was working as a lead partner developer. So, apart from my own development task, like, I was also guiding the backend teams, technically.

[Speaker 2]
So, in the project that you've told me, right, like, can you tell me, like, what are the biggest bottlenecks that you've faced and how did you resolve them?

[Speaker 1]
Generally, there are, like, some bottlenecks here. Like, we faced a lot, like, it's, like, project was related on performance and scalability. So, like, since the platform was handling large volumes of pharmaceutical orders in real time.

So, like, during the business hours, like, we stated, like, started seeing the API latency, like, high API latency, slow database queries, and days in downstream processing between the services. Initially, like, the system shows, like, partially monolithic and many services, like, were tightly coupled. So, because of that, like, F1 services become slow, it impacted the entire workflow.

And, like, one major issue was synchronous communications between the services. For example, like, order validations, pricing, compliance, what, like, happening sequentially, like, which increased the overall response time. So, like, to solve that, like, we generally, like, redesign the workflow into an event driven architecture using Kafka.

Instead of, like, direct service to service blocking calls, services start publishing and consuming the event asynchronously. So, like, that significantly improved throughput, like, and the, like, reduced the dependencies between the services. And...

[Speaker 2]
So, how do you manage this service discovery? Like, you have all these services, right? Yeah, yeah.

How do you discover and do the inter-service communication, like, what is the standard in the different?

[Speaker 1]
Like, for managing the service discovery, like, what I generally do, like... So, like, for, like, instead, service discovery and inter-service communication, like, we mainly followed the Kubernetes native services discovery, like, along with the API-based and event-driven communication patterns. So, since our, like, microservices were deployed on Kubernetes EKS, so each services was exposed internally using Kubernetes services.

So, services, like, services cloud communicates with each other, like, using internal DNS names provided by the Kubernetes. For example, like, if the pricing services wanted to communicate with the compliance services. So, like, it would call the internal service and one using the Kubernetes service, like, name, instead of, like, hard-coded IP addresses.

So, that made the system scalable and dynamic, like, because pod IPs keep changing. And for synchronous communications, we mainly use REST APIs built with the fast API. Internal APIs, like, were, like, secured using authentication tokens and the gateway-level policy.

And for asynchronous, like, we used Kafka. So, how did you...

[Speaker 2]
What kind of, like, for this authentication, do you think the fast API and the best APIs, like, what kind of middleware and dependency injection patterns do you use in production?

[Speaker 1]
Talking about, like, middleware, like, generally what we did in the, like, we heavily used, like, middleware and DI patterns because we had multiple microservices and needed centralized handling, like, for authentications, logging, request validation, and database management. Like, for authentication and authorization, we mainly used JWT-based authentications, integrations with OR2 standards. In fast API, like, we used dependency injections through the depends mechanism.

Like, for example, like, we create reusable authentications dependencies, like, that validate JWT tokens, like, extracted user information, checked roles, permissions, and then, like, injected authenticated user context into API routes. So, instead of, like, writing authentication logic in every API, we centralized it as, like, reusable dependencies, something like token validations or database sections dependencies, rules with access dependencies. So, one more is request validation dependencies.

So, that caps the code modular and maintainable. For middleware, like, we implemented, like, several production-level middlewares, such as, like, authentication middleware, coarse middleware, rate-limiting middleware, request-response logging middleware. So, like this, and for the database handling, like, we used dependency injection for, like, SQL alchemists sessions, like, each request receives as, like, a managed DB session set.

Sessions were, like, properly closed after request completion to, like, to avoid the connection leaks.

[Speaker 2]
And also, in terms of versioning, right, like, whenever you create the backend API, like, how do you do usually the versioning part? How do you take care of it?

[Speaker 1]
For, like, taking care of, like, that, like, generally, for, like, usually we follow the URI-based versioning, like, which is, like, most commonly used in the production-friendly approach, for example, like, slash version 1 slash order slash version 1 pricing. So, like, whenever we introduce breaking changes or, like, major contract modifications, we created a new API version, like, instead of, like, diagonally modifying the existing one. So, like, that helped us to, like, to maintain the backward compatibility for existing consumers.

In fast API, like, we structured versioning at the router level, and we maintained the separate router, and sometimes, like, separate modules, like, for different API versions. For example, like, V1 routes handle older business logic and need to introduce optimized schema for, like, new workloads. So, these approach allowed frontend teams and the other dependent services, like, to migrate gradually without impacting production users immediately.

[Speaker 2]
So, your experience, do you have experience in using LLM-related frameworks or anything in the back-end, like, for placing another part, like, any experience with the AI engine, AI frameworks in terms of observer?

[Speaker 1]
Yeah, like, I have great experience in, like, I have been involved in projects, like, where we integrate AI journey and capabilities into the back-end systems. Like, my experience is, like, more from the back-end integration and productionizations, like, rather than the building the foundational models. But, like, we are, like, I work on, like, integrating LLM-based workflow, like, for intelligent document processing, semantic search, and, like, from the framework side, like, I work with a lank-chain for orchestrating the LLM workflow with open APIs, and I show open AI, like, integration, hugging-face models, like, for NLP, integrated tasks.

I have also experience in vector databases, like, PyCon and FAI-WS, like, for the semantic search, animatics, and also, like, some exposures to the RAG architectures, and, like, one use case, like, involved, we can say, processing large operational and compliance documents, like, where, like, users could ask natural language questions and retrieve the contextual answers from the enterprise documents. So, in that implementation, like, like, FAI CPA was used as the back-end orchestration layer.

We also implemented lank-chain, like, for handling the prompt workflows and chaining. Embedding were, like, embedding so generated and stored in the vector databases. Post-ware SQL and MongoDB, like, were used for metadata and operational storage.

So, like, I was mainly responsible for the back-end AI integrations, authentications and security integrations, also, like, implementing some, like, LLMs and work on some little bit on the RAGs. So, yeah. I think I'm good.

Okay.

[Speaker 2]
I'll talk to you for this. Okay? Yeah.

Thanks, everyone. Thanks for your time. It was nice speaking to you.

[Speaker 1]
Bye-bye. Thank you.

(Transcribed by TurboScribe. Go Unlimited to remove this message.)