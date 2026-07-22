0:00: White swimmers did. 
 0:01: I was about to just drop off maybe just 5 or 10 seconds. 
 0:05: I would have, I, that's why I thought, let me explain. 
 0:08: I just left the bridge. 
 0:09: I was about to leave the bridge. 
 0:10: Sorry, so we'll get started without any further delay, 6 week break, but I will try to pick up the pa and cover everything on time. 
 0:20: This is Rugbo. 
 0:21: I'm going to be our technical panel for today's discussion for this profile. 
 0:24: It's all about for the goal back in technology. 
 0:27: So yeah, what do you, you can go ahead and start with your introduction. 
 0:31: Sure, sure, thank you so much, Raul. 
 0:32: So my name is Ovid, and I have a 12 years of experience as a senior Java for developer. 
 0:38: We'd like a strong expertise in the, like building cloud native microservices based, enterprise application. 
 0:44: And like, on, on EWS also and my core skills like, includes the Java, Spring boot, Spring framework, Microservices, rest API, EW services such as like Lambda, Dynama DB S3, also like, IM and other technologies related like, TypeScript, Angular, and like, SQL, no SQL database like MS SQL to the Mongo DB databases and also like in my current role I'm at Health Partners like I have been working on like a large scale healthcare platform that like supports the provider and member and like claim management systems. 
 1:28: So one of my key projects is more like modernizing a legacy monolithic application into, you know. 
 1:36: scalable microservices architecture using like Java, Springboard, AWS EKS like that, and also like I have designed and developed like restful microservices responsible for like member eligibility, claims processing, and also like. 
 1:54: Provide a data management while like ensuring high availability and performance and also like as part of my project like I, I have built the usable Java components and API following like industry standards designing like using the design patterns integrated with them with the with Dynamic DB for. 
 2:13: Or like high-speed data access and Amazon S3 for document storage. 
 2:18: So like all of these services I have used and I worked extensively with IM to, you know, implement the secure access control, like across the EWS resources and collaborated with like, DevOps teams to deploy patronized application on. 
 2:36: EKS or using the Docker or cos so like that I have used plenty of technologies here so this is my proper interaction. 
 2:46: OK, so can you pick up on, creational one structure and one behavioral pattern and explain me how you have implemented creation of structural and behavioral design pattern and with respect to the software design. 
 2:58: OK, OK. 
 2:59: So, if I talk about like creational structural and behavioral, so like starting from the, if I, I would start from the factory pattern like I use it extensively in my like, current healthcare, health health partners project while like developing like minor services. 
 3:16: We, we had like different types of claims that, you know, required the different validations and Processing logic like instead of, you know, creating objects directly using the new keyword, throughout the application, we, we implemented our factory class and that, you know, decided which, which claim processor to, you know, instantiate based on that claim type. 
 3:39: So plan for if I talk about that for adaptive pattern, we, we use it like while integrating our microservices with external healthcare systems, Each, each system's exposed APIs in slightly different formats. 
 3:52: So you know, instead of you know changing our internal business logic every time, we need to like adaptive classes that, you know, converted the like external request and response format into our like standard internal model. 
 4:05: So you know this allowed our business to business, and services to, you know, to work with our consistent data structure like regardless of. 
 4:14: Like whichever the external provider we we were communicating with. 
 4:18: So like that and other than that we, I can also talk about like for strategy pattern like we use, we have used it in our claims processing module like different claim categories hardly, you know. 
 4:30: different validations rules or like, processing algorithms. 
 4:34: So like that for that purpose instead of, you know, writing a large ifLs or such cases statements, we have created like a separate strategy implementation for each claim type so like that. 
 4:47: the quality is, I mean, I understood. 
 4:49: It seems you're more of a full stack developer, less on the back end developer, when that can be percepted from the quality of your answer. 
 4:57: OK. 
 4:57: Anyhow, let's move on. 
 4:58: let's understand on the internal locking mechanism of panel stream and sema cos in Java. 
 5:04: OK, so if I talk about the, like, working, working mechanism of that balance tree and, semaphones, so, like such as like, if I talk about like, the main goal is to, you know, avoid the tree becoming screwed or because it, it, it, if it's like, becomes like a screwed that. 
 5:27: Time complexity degrades from, you know, omega log and to, to omega N. 
 5:32: So for example, if I talk like in Java, like pre-market researchers, like, internally, use a red black tree. 
 5:40: So which is, you know, self-balanced binary search tree whenever when we insert or delete an element, the, the tree automatically performs, rotation and color changes, to like, like, you know, the automatically like, color changes to maintain its balance. 
 5:59: So, so like because of this, balancing mechanism, operations like search, insert, or delete, consistently take, omega log and time. 
 6:08: So, so, in, in my projects, I have mainly used the tree map, whenever like, Needed and like sorted sort like needed to sorted the data with with the fast lookup and insertion performance. 
 6:21: So if I talk about the semaphones, semaphones, so it is a synchronization mechanism provided in the Java util conquering package. 
 6:29: So, for that like sema4 controls, how many threads can access. 
 6:35: Shared shared resource at at the same time using like a concept called permits. 
 6:40: So like internally some who like maintains a permit count whenever a like a threat was acquired and It also tries to obtain a permit. 
 6:51: If, if a permit is available, the account is, like, demented and, like, and, and that like that continues the execution. 
 7:00: So no permits if there is no permits available. 
 7:03: The thread is like, blocked or like wait until other, another thread, releases a permit. 
 7:09: So that's the, that's about the samples. 
 7:12: What about the executors and completable future? 
 7:14: How executive service and completable future operates in general. 
 7:17: OK, so for that like executors and like computable, so starting with executive service, so if it's a threadpool framework like Provided in like Java Util Concurrent. 
 7:30: So, like instead of like creating a new thread for every task, it maintains like pool of reusable worker threads when, when, when like when we submit our task like. 
 7:43: using methods like submit or execute, that task is like placed into, you know, internal queue. 
 7:48: So if a vocal thread is available, it, it like immediately picks up the task and executes it. 
 7:55: And if our threads are busy, then, then the task reads it, in the queue until our thread becomes, free, free like. 
 8:03: So, and after that, like in my current, like health, health partners project, we use the executive service to, you know, process the multiple independent backing like, task and parallel. 
 8:14: So, such as like, fetching data from like, different services simultaneously instead of like executing them one after another. 
 8:22: So like that and for if I come to the, Compatible future than, like, it is, built, like it is built on the top of the asynchronous exhibition and provides, like much more powerful way to, you know, manage, asynchronous workflow like internally like. 
 8:42: we, we call like methods like, supply sync, or like running sync. 
 8:47: So the method, the task is like, submitted either to the, folk joint pools, like, through the common thread pool whereby like default to, to a custom executive service if we provide one. 
 9:00: So this is, Yeah, exactly 15 minutes or 5 minutes. 
 9:06: I want to spend more on the conception and then I'll be not to coding. 
 9:09: So when it comes to the springboard and microservices, can you explain to me how do you implement, lazy loading and pagination during the entity management? 
 9:16: And also, you can explain me with respect to the security and caching. 
 9:21: How do you implement or what whoever it is? 
 9:23: OK, so, like for this, exactly the particular scenario, so, yeah, I would say like, starting with, with the lazy loading, I would say like we use the spring, spring data JPA with with hibernate. 
 9:37: So by default like, Our relationship like one too many or many too many, we configure them like as lazy whenever like possible and the, the idea is that related entities should only be, you know, loaded when they are actually needed. 
 9:52: So that's how it, it works and like for paging nation we use the Spring same Spring data JPS pageable interface, Instead of, you know, returning thousands of records in a single response, we use, we expose APIs that, exact like, except the parameters like page numbers or, or like, page size or like sorting. 
 10:16: So internally like JPA like, generates the SQL and, like SQL with a limit or offset. 
 10:22: So you know, so only like required records are, are like retrieved from the database and regarding the. 
 10:30: Entity management we follow like proper GP practices like each table is mapped to an entity like using annotation like entity or or table or, or like or or annotation like ID or like. 
 10:46: Or maybe some, some sometimes relationship annotation like one too many or many to one like that. 
 10:51: So we also like exposing entities directly to APIs instead of you we use DTOs and mapping layers to separate the database models from the API contract. 
 11:05: Yeah. 
 11:07: Couple of quick questions. 
 11:08: When it comes to the microsurfaces, how do you deal with the service registration and the load balancing? 
 11:14: Sorry, Microservices and the load balancing. 
 11:19: How do you achieve this in the micro architecture? 
 11:22: So for service registration, yeah, so we use the Eureka server as service registry, and whenever a new microservices starts, it automatically like, registers itself, with the Eureka server by, by like signing up its, service name, IP address, or like code or like health status and Or like it also like sends the periodic heartbeat request like so, so if our service instance goes down or becomes unhealthy Eureka automatically removes it from the registry. 
 11:53: So this way our services always know which instances are like Currently available. 
 11:59: And if I talk about like for service discovery like instead of like calling a service using a fixed URL we we simply use the service name so that the client first like requires the Eureka server then gets the list of available instances and then chooses one of them to send the request and, for load balancing like earlier we use the ribbon with, with like a spring cloud, but in our recent Spring boot application we use the, like Spring boot load balancer so that Spring cloud load balancer. 
 12:32: So like, since ribbon is now like deprecated, so when, when multiple install. 
 12:37: chances of the same microservices are running and load balancer like distributes the incoming requests across those instances and typically use the round robin strategy by default. 
 12:48: So this prevents any any single instance from becoming overload and improves the scalability and availability. 
 12:58: Exactly 11 minutes left. 
 13:01: So one few questions and then I'll move to hands. 
 13:03: Can you explain on the CQRS and Saga implementation and microservices? 
 13:07: How do you implement CQRS and Saga? 
 13:09: OK. 
 13:10: So if I talk about CQRS and Saga, so first of all, I would start from the, CQRS, like, CQRS is like, common query, responsibility, segregation, and when the like, right operations and lead operations have different business requirements. 
 13:27: So like with CQRS we separate, these responsibilities, the common side handles the create, update, and delete operations along with like, All business validations. 
 13:39: So the query side is optimized only for the, reading data and the separation improves scalability and performance and saga pattern, if I talk about like we use the Saga to like to manage the distributed transactions across multiple microservices. 
 13:53: So for example, suppose a member of my. 
 13:57: It's a healthcare claim and the request goes through multiple services such as claim service, member service, provider service, and payment service. 
 14:04: So like that and each microservices completes its own local database transaction and publishes and like even to trigger the next service and this is, there is no like single Global transaction across all services. 
 14:20: So if every step succeeds, the entire business process is complete successfully like that. 
 14:28: Sure, that's great. 
 14:30: we'll go over a handsome coding now. 
 14:50: Yeah, is it visible? 
 14:52: Mhm. 
 14:55: To confirm slowly. 
 14:56: Yes, I can see it. 
 14:57: Thank you. 
 14:58: So let me quickly explain you one scenario with the chat. 
 15:02: So what exactly we need to do, we wanted to create a water simulator factory in Java, and that, water simulator factory will have two pipelines sources, hydrogen and oxygen pipeline. 
 15:13: And these are more of an input source pipeline. 
 15:16: And the simulator is supposed to assimilate this hydrogen and oxygen in the ratio of 2 to 1, from the external simulate, from this pipelines, by maintaining a max capacity of 5000 atoms, and we we really wanted to ensure that it should generate water molecules continuously. 
 15:34: I will put maximum 9 minutes, at 12:30 will come into closing moment. 
 15:40: And I want the solution to be realistic, not something that AIH. 
 15:49: The news move back, we have the solution over the OK. 
 17:57: Kindly explain me why you are writing that code, OK, not what, what I can see in front of my screen. 
 18:02: I wanted to understand the why portion of the code. 
 18:05: Sure, sure. 
 18:06: So, of course, like, For this question, let me start first with a bit, then I can maybe, or maybe I, I don't feel it correct, then I, I can change it. 
 18:19: So give me a few seconds. 
 18:35: Hm. 
 18:36: If I talk about this, let me write it. 
 19:02: Like Basically I have here like created the two cues so like this queue stores the incoming hydrogen atoms and it sends multiple threats can access it safely yeah. 
 20:32: They are like this method represents the. 
 20:35: Hydrogen pipeline. 
 20:37: OK Right. 
 22:03: So yeah, this is the new method like. 
 22:08: Like this method represents the oxygen pipeline and before that like, if capacity is available, I insert the one hydrogen atom into the hydrogen tube, and like this capacity that acquired is like before adding an atom I check whether like before there is space available if factory is full this chart is going to reach so yeah let me write it down. 
 22:46: So yeah, this thread is the water generator, yeah. 
 23:59: So yeah, we could like. 
 24:02: Thank you for your time. 
 24:03: Based on the discussion we have, I will generate the feedback report. 
 24:06: You hiring manager. 
 24:08: You can come to the phone, OK. 
 24:15: Should I complete this? 
 24:18: We can close the, you can leave the bridge, and we close the meeting. 
 24:22: OK. 
 24:25: Thank you so much. 
 24:26: Have a nice day. 
 24:34: No. 
