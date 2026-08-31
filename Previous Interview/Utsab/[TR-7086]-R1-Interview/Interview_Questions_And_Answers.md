0:02: Yeah, what's up, just give me one minute. 
 0:05: Other panel will be joining so that we can continue with the interview, OK, sure, sure, take your time. 
 0:17: Bye. 
 0:19: Yeah. 
 0:24: Hi sir. 
 0:25: How are you? 
 0:25: Oh, I'm good, ma'am. 
 0:26: How about you? 
 0:29: That's great. 
 0:30: Mhm. 
 0:31: So am I speaking here, OK, I'm uttering your name properly. 
 0:37: What's up there. 
 0:41: Yes, can you start off, sir? 
 0:45: Yeah, so nice bag room. 
 0:48: Hope I also see you. 
 0:51: Yeah, definitely. 
 0:55: I just sit. 
 1:00: Yeah, so, I mean, can you tell about yourself? 
 1:04: Mhm, sure, like, as you know, my name is. 
 1:06: I have 3 cloud native, also the, public cloud platforms and the enterprise application modernization plan currently. 
 1:24: health fund like where I'm developed the, the modernization project and, like my primary focus is on, developing and modernizing, back end services, using Python API, class and go, like the building rest APIs and microservices and integrating the enterprise healthcare systems and, like one of the key responsibilities has been the modernizing existing application into we can say. 
 1:53: More scalable cloud native microsurfaces and I have worked on like with AWS services such as EC2 S3 lambda, ECS IM, cloud Watch and SNS SQS along with Docker and And apart from that, like I have also a strong hands-on experience with Taracom and infrastructure at school and like for distributed and even driven processing. 
 2:20: I work with Ache Kafka, implementing like Python and do producers and consumers and. 
 2:27: from like, software engineering perspective, like I'm actively involved in architectures and, design discussions, code reviews, unit and, indication testing, debugging, and the production supports, and, apart from this, like I'm also comfortable using the enterprise, approved AI tools such as the get a co-pilot, cloud, GI platform. 
 2:50: So that's all about me. 
 2:52: Great, great. 
 2:54: So, we'll take this interview in 3 parts. 
 2:56: First, we'll be discussing about the system design, next to the cloud architectures and all. 
 3:01: And the third one is like, kind of, integrations you have done, are kind of, failure. 
 3:08: Mechanisms are test integrations, whatever testing integration, everything, OK, so coming to the system design, yeah, coming to the system design, so you mentioned about the modernization of the application, right? 
 3:18: So what kind of modernization it is? 
 3:21: So what, what, what, what, what's your role and what's the teching involved there? 
 3:25: Oh yeah, I like talking about like the modernization like in this, basically, absolutely the modernization is like we are doing. 
 3:34: is mainly around taking existing enterprise healthcare applications and moving them like like like we can say moving them like towards a more scalable or we can say the cloud native architecture like basically the existing application has some like tightly coupled components. 
 3:53: So one of the things like we looked at is like identifying the business functionality so that. 
 4:01: Can be like separated into like independent services and also like we then build those services like using a Python mainly using fast AP and Flask and go like we are we need services that benefits from both performance and the concurrency here like my role is primarily on the application and the back end side but like I'm also involved in the architectures and the cloud side and like I participated in the. 
 4:32: designs data flow, and so yeah, that's the things and like we also have the event driven processing where the Kafka is used for a synchronous communication. 
 4:41: Yeah, we'll go into those into those, we'll go into those later. 
 4:45: So coming to the modernization, so you said it is a some kind of legacy application and it's tightly coupled. 
 4:50: What do you mean by tightly coupled and how you are, like, separating out the models and what is the, mechanisms of the principles involved. 
 5:00: to separate out the models and how would they communicate. 
 5:04: And I, I'm assuming that the database schema will also change as you're separating out. 
 5:10: Correct me if I'm wrong, yeah, yeah, yeah. 
 5:12: So how do you like, the like, the application has to work with the legacy data and the legacy users as well, right? 
 5:19: So how do you do all these things? 
 5:21: OK, sure, like, firstly, when I say the tightly coupled, I mean different part of the application have like we can say strong dependency on each other. 
 5:29: For example, in a legacy application. 
 5:33: one module like might directly call another module access the same database tables and depend on its internal logic. 
 5:41: So like we can say even like a small change in one area can potentially impact several other areas and in our modernization approach we like first understand the existing application and identify the actual business. 
 5:55: Business capabilities rather than just splitting the code randomly. 
 5:59: For example, if an application has functionality around member information, claim processing, notification, or even like reporting, we look at those at separate business capabilities. 
 6:13: We identify the depend dependencies between them and the APIs or data like they need. 
 6:20: And then, like define reasonable services boundaries and once like we have those boundaries. 
 6:29: We like expose the required functionalities through like well defined rest APIs or as synchronous events and the new services are like developed like primary the past you can go like used where it makes sense. 
 6:44: So the good question is like, so, so when you are separating out the modules, so first you need to identify the modules, right so. 
 6:53: Some principles involved to identify the modules and the second thing is, so, sometimes we cannot, like if the business model of module we need to separate out the business logic as well, right? 
 7:08: So for example if I'm in, let's say e-commerce website, so, I, I might build the orders module payments module. 
 7:18: car module as a separate things and so in order to use all of them I need to separate out the business use cases to separate levels. 
 7:27: So how do you like do these things and what kind of communication mechanisms you will be putting in. 
 7:33: , so that these models will communicate and how do you handle the failures of one module. 
 7:40: So definitely all the modules won't be sitting on a single server. 
 7:44: So mostly they'll be sitting in different servers. 
 7:46: So how do you handle that distributed mechanism? 
 7:50: Yeah, those are my questions. 
 7:51: Like, I would look at it from a domain and responsibility perspective, like rather than simply taking the existing code and like splitting it into the multiple services first, like. 
 8:03: I tried, I, I try to identify the business capabilities and bounded context like, in an e-commerce system like, order, payments, inventory, and like the customer management or like different business capabilities. 
 8:15: So I look at things like the, business ownerships or data ownerships, and like how frequently the functionality changes are. 
 8:24: Transactions boundaries and like depend dependencies between like the areas so those are like good indicators for deciding where the service boundary should be and then I separate the business logic from the technical concerns. 
 8:39: I don't want like the business rules makes like directly into the API controllers database. 
 8:46: Codes or like we can say messaging for code for example like with with with an order service stuff like API layer like might receive a request to create an order so the API validates the request like at a basic level and pass it to the application or like use case layer so the use case layer. 
 9:09: coordinates the actual business operations and the domain layer like contains like rules such as whether an order can be submitted or whether the items are like valid or like then the infrastructure layer handles the things like database access or like the external integration so. 
 9:28: That separation like makes the code easier to test and also makes it easier to change the technology underneath like without changing the business rules and like for communication I generally look at like whether the interaction needs to be synchronous or as synchronous. 
 9:45: So if I need an immediate response, like for example, checking, checking whether an order can be created, I would typically use a rest API or another synchronous API. 
 9:59: But for like something like order has been created, now modify inventory or the payment and the notification systems, like I would prefer an event-driven approach where the order service published and even through the TAFCA or the messages service such as like the SMS or SQS so the downstream services can consume that independently. 
 10:22: OK, good, so, yeah, coming to, the legacy, I'm assuming that the legacy application in the production, so currently as you are modernizing, so you need, you need to document whatever the functionality is doing and that. 
 10:37: Then you need to do the code changes, right? 
 10:41: And also whatever the modern application you have written that need to be on par with the like the functional device if you should be on par with the legacy system, right? 
 10:51: So how do you ensure all these things. 
 10:54: to generally ensure all these things like we treat like that as one of the important part of like modernization, like. 
 11:04: We don't want to modernize the application and accidentally change business behavior that the users are like depending on like. 
 11:13: Generally the first thing we do is to understand and document the existing behavior like we, we look at the existing code API contracts and the database interactions, configurations, integrations and also like talk with the business or subject matter experts like where the code alone does not clearly explain the business rules and then like we like. 
 11:40: the functionality like we are going to move and like define the things and also, like, after that, like, generally that gives us something like we can actually evaluate against, and the next important, piece is like testing the legacy behavior like before making the change and generally. 
 12:01: Existing test is like where they are available like and for like the critical workflow like we add the additional unit and the integration test around the current behavior and basically we want to establish a baseline before like we replace anything and then we build the modern service. 
 12:19: You just just like test whether the new code works like we, we test whether it produced the same expected business outcome and for like the same scenario so that includes like the positive cases. 
 12:33: , validation failures, edge cases, and the integration failures, like, for example, like if we are like moving a particular business workflows like from a, a legacy application into the pattern-based service, we can take like representative inputs like from the existing system. 
 12:51: So or like execute the, corresponding workflow and the new service and, compare the important outputs and the side effects so and. 
 13:03: we also, use an incremental migrations like. 
 13:08: we can say, approach like we don't, like switch everything over the one and, we deploy the new functionality or alongside the existing systems validated like on the lower environments, like the perform integration and regulation testing and like, then gradually move traffic or the constanttiator. 
 13:31: OK, so, coming to the documentation, so, so you will be understanding the business from the old, old legacy system, and you will be documenting, right? 
 13:42: So what kind of, documentation mechanism you will be using up? 
 13:45: Will you be using, user stories or what kind of thing it is? 
 13:50: Oh, yeah, like, see. 
 13:51: For like the documenting, it generally use the combination like, rather than relying on the user story, only on the user story like, for the modernization work, I would first document the current state behavior of the legacy, application and I also want to capture like what the system actually does today, business rules, workflow where we can say inputs, outputs, or, integration of dependencies. 
 14:18: Error scenarios and like other important data flows and for the requirements and the business visa we can use epic and the user stories in the backlog and generally a user story like captures the business requirements from like the we can say. 
 14:36: like we can say, like the user's perspective and we are the acceptance criteria. 
 14:42: So there is a clear definition of what the, modernized functionality needs to support and, like for the technical side, I would maintain the API documentation, architectures, diagrams, sequence diagrams, integration documents, so yeah. 
 15:01: OK, so what would be the format for like format, for the business rules? 
 15:07: How do you like, keep the business rules? 
 15:10: So as you mentioned, there will be. 
 15:13: the legacy system is coupled in our like tightly coupled. 
 15:17: So how do you like, by writing the business rules itself, will you be keeping the coupled business rules or, isolated business suits? 
 15:25: So how do you document that? 
 15:28: Oh yes, like, for business to, like I prefer a structured technology independent format because. 
 15:33: If, if we document them directly into the terms of legacy classes or we can say database tables we carry the legacy coupling into the new design like for each rule I normally capture, we can say a rule ID or business. 
 15:49: capabilities, description, inputs, conditions, expected outcome, outcomes or, like a source of source or like owner, like for example, like PR 101 eligibility validation, like, given, given a member that, and the state and. 
 16:08: If, if, if like member has an active coverage for that date, the request is like eligible otherwise return the appropriate rejection season. 
 16:19: So then we document as case separately and, it's like, one legacy function contains 10 different rules. 
 16:30: I don't document that as like one large rule. 
 16:34: basically I decompose it, by the, business responsibility, so that helps us like later map each other to appropriate, a boundant context for the microservices. 
 16:49: So, is it, is it the monolithic or, microservice based, see, like, basically in this it is a microservices like primary is like a monolithic application, with some like external integration around it. 
 17:05: So that actually one of the like the main reason we are modernizing it. 
 17:09: So, like currently it is in our, microservices. 
 17:15: OK, so as, it is a monolithic, so far coming to the microservice, the complete principles will be different, right? 
 17:22: So what kind of principles you'll be following in at the level of integrations with the different modules from module to module, like, see, like moving from a monolithic to microsurfaces changes the design principles significantly, especially around the integrations like. 
 17:41: The first principle I follow is the loose coupling and the clear ownership. 
 17:45: Like each service should own a specific business capability and ideally like its own data. 
 17:52: Like other services like should access the capability like through the designed contract rather than directly accessing its database. 
 18:02: And for integration I choose between synchronous and as synchronous communication based on the business requirements and if I need. 
 18:11: And immediate response like valid validating eligibility, I use, rest APIs with well-defined open API contracts and, if the downstream, processing can happen independently, I prefer Kafka or messaging so the like services are like not, run, run time dependent on each other. 
 18:31: And another important principle is designing for failure, like, in a monolithic internal method called usually succeeds or through immediately, like across services, networks and downstream, systems like can fail. 
 18:47: So we like implement time of controls with trials with the exponential backup, circuit breaker, item potency, and the dead letter handling. 
 18:58: OK, so, let's say for example, there is a model one which is depending on another model and it is, it is communicated, The other module and so there is no response from the module to so you're saying if you'll be using the circuit breaker so how much time will you be keeping so that the client the customer or the client won't think so it doesn't look like a latency and it doesn't look like waiting like how do you handle. 
 19:29: But how do you balance both the exponential backup, the render mechanism and all? 
 19:34: The second question is, see, let's say for example, you have, triggered a request and, within a, given time, the response didn't come. 
 19:45: So you, with the exponential backup you the question again. 
 19:48: So suddenly the 22 responses have come. 
 19:51: So how do you handle that item potential. 
 19:56: see, generally in this type of, scenario like, like what I do, like one distinction I would make is that for truly asynchronous communications like I normally would not keep the customer waiting for module 2, module 1, except the request generates as like a correlation of the transaction ID persists like the states as something like a pending or publish the message and returns like an acknowledgment to the client. 
 20:29: So circuit breaker are more. 
 20:32: Applicable to the synchronous downstream costs and for retrials like I don't use one fixed number everywhere we define the timeout or any and like retry policy based on the downstream services sorry. 
 20:48: Yeah, understood, understood. 
 20:50: Yeah, consider this, this scenario itself like you are doing the synchronous communication and you are expecting the response from the other module, but you're still not getting and you try, you retried it and you got the response from the both the requests. 
 21:04: So how do you handle the responses and how the module one will be like doing the things. 
 21:11: see, like whenever like we are like, doing these things like that can like definitely happen in synchronous communication like like at a timeout only tells like a module one that it did not receive the like we can say response within the expected time, so it does not necessarily mean module two did not process the request. 
 21:34: So like I handle this like primary using an item potency. 
 21:38: Like when module one sends and like the first request, like it generates a unique transactions or like the request ID. 
 21:46: So if it's like the times are like out and retrials, it sends the same ID or like not a new one. 
 21:54: And on module two like. 
 21:56: We maintain the processing status for that ID. 
 21:59: So like if the first request has already completed, the retry does not execute the business operation again. 
 22:07: So it's simply. 
 22:10: returns, the previously stored result and if it's like still processing, we can, return the current status on like the, we can say on like the weight based on the APR contract. 
 22:23: OK, I'll give you one more perspective, like, module, from the module 2 perspective. 
 22:30: So let's say for example, module 2 guard the two requests from the module 1 concurrently. 
 22:34: So how do you handle that situation and what are the tech techno, the kind of techniques involved? 
 22:42: OK, like talking about the techniques, like, like, yes, like from module two's, perspective, the important point is that two concurrent requests can pass a simple like check whether the ID exists, logic and exact the same, like time. 
 22:59: So the application level like, checking alone is like not sufficient, and I would, also use the, same potency key from module one. 
 23:10: But like enforce the uniqueness at the persistent, like, persistent like storage level, for example like Module 2 can have the item potency or the transaction table like where that the key has unique rights. 
 23:26: So like when both requests arrive concurrently, both may attempt to create the transactions, but only one can successfully acquire ownership. 
 23:36: So depending on the database, we can like use a unique contracts like Aomic inserts, conditional update or the row levels locking and like. 
 23:47: Basically, the winning request marks the transaction as processing, executes the business operations, and like finally stores the success along with the response. 
 23:59: Understood. 
 24:00: Yeah, so some, some DBS won't be having that whatever the capability you are saying, the logging capability. 
 24:07: So how do you, get the log login capabilities to that application or to that, resource which is sensitive to those concurrency related things, let's see, generally for like the like. 
 24:22: I normally try to put the concurrecing control as close as possible to the resource that owns the state, which is usually the database rather than like implementing only like application level for example like if two instances of module 2 are like. 
 24:41: Trying to update the same transaction so we can use like a pessimistic locking such as like select or like select for update and inside like a like a short database transaction so. 
 24:54: The first request obtains the row log, completes the critical update and commits, and the second request waits and then like reads the update straight. 
 25:06: And another option is the optimistic locking which, which I prefer when the condition is relatively low, like. 
 25:15: We maintain like, we can say like, we maintain a version number of on the record and yeah yeah yeah let's go to the next one anyways, so yeah, let's say for example there is one more use case like you, you have modernized the application let's say, so everything is modernized now you want to change the database from MySQL to no SQL SQL to NoSQL. 
 25:42: So how do you handle, like How do you like, plan it so that database like, storage layers can be easily modified. 
 25:54: , yeah, like, generally, Like if I know the storage technology may change later, like, I try to make sure the business layer like never depends directly on my skill specific, implementation details. 
 26:11: Like I normally, follow like hexagonal or the clean architecture pros like the, like the, the domain of the service layer works, with an abstraction for, for, for example, like a member repository or, order repository with like. 
 26:27: With operations such as like the get fr update, so then like the infrastructure layer like pro provides the actual manscale implementation. 
 26:35: So if later like we move to like Dynamo DB or another like no escalator is like we, we create another adapter implementing the same repository content and the business logic like should require like minimal change changes and also like. 
 26:53: I would not say changing SQL to new SQL is simply replacing a driver. 
 26:58: The data model and the access patterns are like fundamentally different, like before migration, and analyze the, query pattern patterns relationship, or the transactions consistencies requirements, indexes. 
 27:12: Also then I designed the new escal model around those access patterns, and, like, yeah, yeah, yeah, let's go to the, so. 
 27:25: Buddy. 
 27:34: Yeah, so coming to the, testing, so we need to do a lot of automation testing, right? 
 27:40: So, so how do you write, the automation test, test, and how do you keep the business logic simple so that, writing unit test will be easy? 
 27:51: What kind of principles you would be following for each business unit or business logic, whatever you say. 
 27:59: yeah, like, totally understood. 
 28:01: Like, basically, for me, like testability starts with the application design itself, and if the business logic is tightly coupled with the database, STTP calls or the AWS services, union test becomes quite difficult. 
 28:15: So, like, generally I follow the solid principles depending, dependencies in, inversions and separation of concerns. 
 28:22: Like, I keep the core business logic in a small, small service or the domain classes and inject external dependencies to the interfaces, for example, like, repositories, payment lines for the message publisher, so that allows me to replace those dependencies like, with mocks or the fake during the unit test and, for like each business rule I, I try to keep the function focused on, one responsibilities. 
 28:48: Then I write the test using an arrange. 
 28:51: Assert a style like basically prepare the input, execute the business rule and verify the result like I covered the happy path or the boundary conditions, validation failures, and I in Python like I typically use P test with the, with pictures and mocking of the required. 
 29:11: Great, so, So this is about the new test. 
 29:16: So coming to, we will be doing APR test, test also, a snapshot test kind of thing and the integration test. 
 29:24: So what would be the structure of snapshot testing and, So what will you be mocking there and what will you be testing there, and, coming to the integration testing kind of flow testing essay so irrespective of what kind of client it is, so we need to test the the entire packet according to the business flow, not the business logic. 
 29:48: So what kind of tools are the services are the tech you would be using there, like generally in this. 
 29:56: basically, I separate like these into the API contract or the snapshot testing and integration of the business flow testing like. 
 30:06: like for API snapshot testing, my goal is to like, detect, unintended changes in the API, contract, and I call the fast EPN point using the test drive and the, capture stable parts of responses, status code, Jason architecture, or like the, Jason structure, field names, and generally I avoid, snap, snapshotting dynamic values like, timestamps or generated IDs and this. 
 30:34: And for the integration testing, I reduce smoking significantly. 
 30:39: I prefer running real dependencies in a like isolated environment and for like Python, I typically use like fire test of RTPI, the test client or the STTP client and Docker-based test environments and in CICD these tests are automatically like, before the deployments. 
 31:01: OK. 
 31:02: OK, so there's one more, yeah, like I'll give you one use case like, so in the back end, mostly we need to do, kind of, mostly, most of the cases we need to keep it backward compatibility and sometimes we'll be pushing the few features ahead and giving it to, to few customers or few people only. 
 31:24: So like how do you handle such things. 
 31:29: generally, like for handling these type of things, like I. 
 31:34: Angle, those are two related concerns the backward compilability and the control feature rollout like for like. 
 31:41: For the backward compatibility, I try to make API changes addictive. 
 31:44: For example, like adding an optional field is safer than renaming or removing an existing field. 
 31:51: So if we need, like a breaking change, I use API versioning such as like V1, V2 and keep V1 available, until existing consumers have migrated. 
 32:03: I also use, contractor and CI CI to make sure like a chain does not accidentally break existing consumers. 
 32:11: And like for the reusing functionality only like to select the consumer so I use the feature flex so the new code can be deployed to the production but remains difficult by by default and also like for large infrastructure level changes, I, I can combine with with like this with the canary or the Blue game deployments with the by like the feature flex control the actual business function is exposed to the user. 
 32:44: So that would be like this is client level versioning of the compatibility so sometimes we need to be compatible with the databases chemo might be changing. 
 32:55: We need to do a number of things with respect to database. 
 32:58: So how do you handle the application level things and then maybe there won't be any changes with respect to the client or. 
 33:07: Yeah, yes, it would be a change in the package, yes, so yeah, so that is more difficult, right, yeah, exactly, the database backward comparity is like equally important, especially when like old and the new applications. 
 33:23: At the same time during deployment, I like, I normally follow the expand and contact pattern like the for schema changes like example like if I need to rename a follow on like I will not directly rename or drop it because the older application may still depend on it. 
 33:40: First, like in the expenses, like I add the new column, in the backward compatibility way, usually like the, null or with like a safe default, and then the new application versions can support, but, we can see. 
 33:56: Old and the new schemas like if necessary we temporarily write to both fields or like use a migration process to keep them synchronized and after that like we back back the historical records and validate the data to reconciliations and once like all application instances and, depend dependent consumers have moved to the new schema we like just. 
0:00: One only in a later release the contract phase, do we like remove the old field or or like a contract. 
 0:08: OK, OK. 
 0:11: So yeah, let's go to the text and so this is think about architecture. 
 0:17: So coming to the Python and the cool and. 
 0:19: So which one do you prefer and, what's your like pro what do you say about the pros and cons considering this is a large scale application, a complex application. 
 0:29: see, Kumar, like I would not say I always prefer one over the other. 
 0:34: Like I choose between Python and go based on the characteristics of the service like. 
 0:38: For like most business, APIs and the integration service, I usually prefer Python because like the development is faster. 
 0:46: The ecosystem is very mature and the frameworks like fast API, make API development, validation and testing, straightforward and I prefer go when the like services is more competency heavy performance in the city or the infrastructure oriented and go routines and channels like make like concurrent workloads easier to handle and go give us like like a strong performance like relatively low memory consumption. 
 1:18: OK, so yeah, coming to the goal, goal depends upon the hardware like hardware you are running the application, right, whereas Python, yeah, Python run time also works, but like, let, let, let less dependent on the hardware more or less like. 
 1:35: So how do you handle such things? 
 1:37: So we may not know the hardware upgradations of the OS upgradation as going slightly compared with the OS and hardware. 
 1:45: So how do you handle the situation and how do you make sure that your application is running properly? 
 1:51: basically I would make like one distinction. 
 1:54: Like Go produces a major binary for the target OS and the CPU architecture. 
 2:00: So the dependency is mainly at build time. 
 2:04: I would not build a binary on a developer laptop and assume that the same artifact will work everywhere. 
 2:11: So, in practice, like we handle that through a standardized, CIC debate, is it something. 
 2:20: Yeah, I think I, like the CRCD build process and like and the containers and we exactly, like, like we explicitly define the target using the booze and the goats or like for example Linux on the AMD 64 and ERM 64 so like the, generally, the binary is like built inside the control building image tested and then packaged into the document so production modes, run the val validated container rather than, locally compiled artifacts and. 
 2:56: I also tried like to keep who services as portable as possible like pure Go dependencies are like easier because we can often build statically with the CGO enabled because zero we use CGO or the native libraries like then LIBCROS compared with like require additional testing. 
 3:20: Yeah, that's it from my side, I said. 
 3:22: So actually if I get any questions I need to ask, but, we have like less time, so I have another, thing to do, other call, call help. 
 3:33: So yeah, prepare for that as well. 
 3:35: So yeah. 
 3:37: Yeah, that's it. 
 3:38: OK, sure, like, yeah, I will get back to you. 
 3:43: Sure, yeah, like, I, I, I just asked some questions like, apart from this round, is there, any technical round or any other round for this room? 
 3:54: Yeah, yeah, this is, this is just a screening round, so the time we'll be doing the technical thing again. 
 4:00: We'll be it is just a screening round. 
 4:11: no, no, not a lot. 
 4:15: OK, thank you so much. 
 4:17: thank you, Erwin. 
 4:18: Have a good day. 
 4:18: Nice to meet you. 
 4:20: Bye-bye. 
