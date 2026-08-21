0:01: OK. 
 0:06: And I was this lord. 
 0:14: 1 2nd. 
 0:29: OK, I'm, so I don't have your resume with me. 
 0:31: So can you start with introducing yourself and what's your total experience, current text stack, those things, like, my name is Amit Paul Sing money, and I like, I have over 13 years of experience in software engineering, with like a strong focus on Python full stack development and like cloud native applications, micro services, and I like solution architecture and DevOps also. 
 0:55: And currently, like, like recently, I worked with, as a principal Python developer with the Wisconsin Department of Health Services, where like my, my main focus was like, in back in architecture and like development for a healthcare application that manages, you know, like family relationship and relationship matching data. 
 1:15: And yeah, like I'm working with Python and fast API to build this APIs and microservices along with, you know, like SQL for data layer and like Docker and community for conation. 
 1:25: And like on the cloud side, like I have, you know, a strong hands-on experience with AWS, Lambda, API gateways, and like ECS and APS. 
 1:35: And before Wisconsin, like, I worked with a Medisource version as a lead Python developer and architect, and like that role like give me a lot of experience beyond just called coding. 
 1:47: So yeah, like I was involved in understanding business requirements, I would say defining service boundaries, like designing APIs and data models. 
 1:56: Yeah, like overall I describe myself as someone like who is comfortable owning a solution intern. 
 2:03: Yeah, that was a little about me. 
 2:06: OK. 
 2:07: what's the architecture of the current or recent project with which you worked on? 
 2:12: OK, so like the current recent project at like Wisconsin, Wisconsin Department of Health Services, we are using a cloud native microservices-based architecture. 
 2:20: So like at a high level, the front end is built with react and like that communicates back end through the APIs. 
 2:25: So that is architecture. 
 2:28: OK, and the database is sequel. 
 2:32: OK, and, can you explain me, or give me an example where, you, you faced, technical challenge and you how you come up with, so, you know, solving the problem. 
 2:48: So like, if I, if I would describe your typical challenge that I have faced, so like one good example was like in my current like Wisconsin DSS project, like where we had, you know, our performance issues around the family relationship matching functionality. 
 3:03: So, like the API was working correctly, but like as the amount of relationship. 
 3:08: Data increased at at an extent, but like some requests were like taking, you know, like noticeably longer than expected and like I started looking at the API matrix and like application logs, like I would say to determine like where the bottleneck was in the Python service or like it, it is in the database or like downstream processing and like later I found out that the main issue was on the database side and like some of the relationship queries were like doing more work than necessary. 
 3:38: Like, especially when we are, you know, like we are joining multiple tables and like retiring data, that the API didn't actually need. 
 3:46: So yeah, like I worked on restructuring those queries and like reviewing the data model and indexes, and I'll say also changed parts of the API logic so like we were only, you know, fetching the data required for that particular request. 
 4:01: So yeah, like after the changes, the response time was like much more consistent and I would say especially for the larger data sets. 
 4:08: So yeah. 
 4:10: OK, can you get a little detail into how did you solve that performance issue, in database side. 
 4:16: So you said there were two things you looked at the index and, projections, those things you looked at. 
 4:23: was the only two issues, that helped the performance? 
 4:26: Was there anything else? 
 4:27: Can you get deep into that, issue? 
 4:30: No, so like if I, like if I explain to you more about this issue and how I like resolved it, so no, I won't tell that like it wasn't just the indexes and projections. 
 4:40: So there were, I would say like there were two of the bigger improvements, but like, you know, I looked at the complete request part, for example, like after optimizing the SQL, I also checked whether we are like making multiple database calls like for the same request, and in a few like places we were able to like reduce unnecessary calls by like changing the service logic and like fetching only the, you know, the required data more efficiently. 
 5:08: And like I also looked at the page nation because this is one of the important concepts that we have to look up to and like because you know like returning a large relationship data set in a single API response like can create pressure on both database and also like on fastly paced service so like we made sure that like we were processing and like returning only, you know what the I would say the client needed. 
 5:32: And the next one I would say like in our Python side I reviewed some of the business logic like to make sure like we were even if we were not doing the expensive filtering or I would say transformation after that like the database had already returned the data and like wherever possible like I move that work to database or like simplify the processing and like the last thing that we have worked with. 
 6:00: like, I also, I'll say, looked at the connection handling and like API logging and monitoring. 
 6:06: So yeah, like I'd say it was a combination of like, query and index optimization and reducing like unnecessary database calls, pagination at the same time, and, like minimizing data returned and simplifying Python processing. 
 6:20: So yeah, I have looked at, you know, all of them, at the same time, asynchrony. 
 6:27: OK. 
 6:28: So how much improvement did that give you? 
 6:31: Before and after, yeah, like, talking about more specifically the number or like. 
 6:39: The time, yeah, OK, so like 2 more time, right, yeah. 
 6:43: Yeah, I mean, it was a noticeable improvement, but like in the slow, slower scenarios, I would say we were seeing API responses. 
 6:53: Yeah, pretty late, but like, it was roughly, I would say, 2 to 3 times improvement in the like slower scenarios, but like I wouldn't, I'd say I wouldn't look at it only as like raw percentage improvement. 
 7:08: like the bigger benefit that I got like was that the response time became, I would say like much more consistent. 
 7:15: As the like data set grew and before the changes like larger relationship queries could take I'd say a few seconds. 
 7:24: So yeah, like, so overall, like we saw mostly to be very specific, like 60 to 70% improvement in response rate, like for the affected API so. 
 7:36: OK. 
 7:38: So did you create this, architecture in from scratch or it's already there and you started to work on it, improvising it? 
 7:46: Oh, like, like, I would say it was a combination. 
 7:51: I did say to say whether you were, so the start of or you were, yeah, and yeah, like it was a combination of both. 
 7:57: I will, I will say like the overall enter enterprise environment and some of the like foundational infrastructure, like, we were already in place when I joined and like I wouldn't say like I created the entire architecture from scratch, but, but like what I did like. 
 8:13: What I did own was a significant part of the application level architecture. 
 8:17: Like as we added and like changed functionality, I worked with a team to like define the service boundaries, API contracts, data models, and specifically like how the services would interact with each other. 
 8:29: So yeah. 
 8:31: OK, if you had, started this project from scratch, what are the architecture change you would have suggested, for this particular issue? 
 8:39: Like, OK, you know, these guys would have done this way. 
 8:43: In that case they would have not faced these kind of issues. 
 8:46: So like that, what are the architectural changes you would have suggested if, if it's your project and we start from scratch? 
 8:52: Got it, got it. 
 8:54: so like that's a pretty good scenario to be in, I would say. 
 8:58: like, if I were designing this from scratch, like I would try to prevent that, you know, performance problem, I would say at the architecture level rather than, you know, fixing it after the data has grown. 
 9:10: And like, 1st, 1st thing is that I would do, like I would spend more time on the data access patterns, before finalizing the excuse the schema, for, for the relationship and matching use case, I would identify like high volume queries up front. 
 9:25: I like designing the tables and I'll say the indexes, specifically, you know, around those access patterns. 
 9:31: And yeah, like I would also, I would say. 
 9:34: Yeah, I would also like to avoid overly broad joints and like make sure that the APIs are like like designed to request only the data they actually need. 
 9:44: And the second thing that I could do is like I would make Pation part of the API contract from like D1. 
 9:51: And yeah, like I wouldn't design an endpoint that like assumes it can be done a potentially say a large relations of data set in one response. 
 10:00: I'm looking for two things, OK, I'm looking for two things. 
 10:05: One from the high perspective, like, OK, I would still stick with the SQL server. 
 10:09: I would still stick stick with, you know, my APA or deploying this particular services somewhere. 
 10:17: It will be, was it a monolithic application or a microservice? 
 10:21: No, it was a micro. 
 10:25: So I still speak with the microservice architecture. 
 10:27: So this kind of thing from high level I'm asking, and what are the other things which you felt the one thing you said the agation which you would have added from the beginning, likewise, what other things you would have added from the beginning so that you would have had more control? 
 10:41: OK, these are the two factors I'm looking for for this case. 
 10:44: Yeah, yeah, I got it now. 
 10:46: Like, yeah, OK, so like if I explain it from a high level architecture, like I'll still keep the microsource architecture. 
 10:53: And like I don't think like the performances were were like caused by choosing microservices or like a skill server or like I would say the deployment model. 
 11:01: The issue was like more around how data access and like API layer were designed within that architecture. 
 11:06: So like if I were starting from scratch, my like high level architecture would be something like, like the react on the front end and like the API gateway in front and like Python API based microservices on the back end. 
 11:21: like, SP server as a primary relationship with the database, you know, because like the relationship data needs strong consistency and I'd say like transaction support, yeah, like I would still continize the services Docker and like deploy them through Kuberities or like, you know, the appropriated this container platform, and yeah, like I keep the CIC decentralized logging and monitoring, you know, as a part of platform day from day one I would say. 
 11:48: And like where I would make a difference is like in the, I would say like boundaries and detach patterns. 
 11:55: like, I would make sure like each service has, I would say, like well defined responsibilities. 
 12:01: And like APIs are designed like around I'd say actual use cases and like the data is schema and I'd say the indexes are designed based on the expected query patterns and data volume. 
 12:11: So yeah, like at a high level, like I would not change the fundamental architecture just because, you know, this is a performance issue. 
 12:20: rather, I would like to keep the microservices and SQL server like fast API, whatever I'm using and a continuous and cloud deployment. 
 12:27: Like I would improve the way those components are were designed and like connected. 
 12:32: Like we don't create the same bottleneck as I would say in the data grows. 
 12:38: So this is what I can think of from a high-level perspective. 
 12:45: OK. 
 12:48: so was there any, testing, you know, testing, integration testing was done in your project? 
 12:55: yeah, like I have. 
 12:56: Like you know testing in my project like we, yeah, like we both already. 
 13:04: Yeah Yeah, how did you approach, unit testing and integrative integration testing, because in your case it's a microsurface. 
 13:11: So how, how did your unit test and integration testing were evolved? 
 13:15: Yeah, like, if I talk about the testing part, we like both, we have like both unit and integration testing and like it evolved quite a bit as the project matured. 
 13:25: Initially, the, I would say the focus was mostly on unit testing and I'd say Python business logic and like making sure, individual functions and like APII behaviors were correct. 
 13:35: And as the application like became more complex I'd say like we added more micros services and like we expanded the integration coverage and yeah like we started testing the actual interaction between like fast API points and like server logic and like the databases because I'd say like yeah that's where some of the real issues can show up things like I would say incorrect queries, let's say transaction behavior or data mapping and like or you know you can say like unexpected repay responses. 
 14:05: And yeah, like we also became more disciplined about like what what belongs in each type of test. 
 14:11: I prefer keeping unit tests fast and I'd say, mostly isolated. 
 14:17: So like we run on every change and integration tests are like a little bit heavier. 
 14:23: So like say, I would say like they focus more on like critical parts and interaction between components. 
 14:30: So yeah, like as we, I would say. 
 14:34: Yeah, then we like we incorporated those tests into like CICD pipeline. 
 14:38: So I'll say a typical change would go through a unit test first. 
 14:42: And like, this is followed by integration testing and like only after those checks passed, would we move forward building the Docker image and like deploying it to the next environment. 
 14:53: And yeah, like as we encountered production issues, we also use them to like to I would say improve the test so for example, after the database, I would say, after the database performance issue like we added more realistic data data and scenarios around like large relations and data sets so like that we, you know, couldn't catch similar problems earlier. 
 15:16: Oh yeah, like, OK, OK, I like to understand, imagine you just have a simple AP, OK, which, takes some input from the user, and, searches something in the database and it turns, in some format or something, OK, I'll does some. 
 15:32: Business logic and then returns to the user simple API that can be, getting, patient data or something like that in that if that is if you have to do the unit test or integgratration test for that particular flow, how did you handle in your project. 
 15:48: Or did you connect to the real database or did you connect, how, how that, you have handled the test? 
 15:55: OK, so like in that particular scenario a manual test. 
 16:01: Good. 
 16:02: Yeah, so like in that particular scenario, I would, I, if I would give you the flow of like unit or whatever like integration testing, say for a simple API like that, I would test the flow at two different levels first, and for the unit test like I would isolate the party pain point from the, I'd say actual database. 
 16:22: And like after that I mark the database or like the repository and like provide control input. 
 16:28: for the example, if like if the API, I'll say like receive, like if, if, for example, like suppose we have a good patient ID in point, like I would mark the repository or database layer, I'd say just like I said and provide a known patient record. 
 16:46: And then like afterwards I will verify like that the service, you know, that correctly validates the input causes the repository with like right parameters that is more, most like necessary. 
 16:57: And that applies the business rules and to returns the expected response. 
 17:02: So yeah, like I just cause like an invalid patient ID, patient not found, I'd say validation failures and like most importantly the expected exceptions that we can have people. 
 17:15: For example, if the database like returns a patient object, I want the unit test to verify that the service converts that into like, say a correct API response because you know, the database is marked and say like test stays fast and isolated. 
 17:32: yeah, like after the further step I that I can do, then for the integration test, I will test more of the actual flow. 
 17:40: I would like to, you know, call the FASi painpoint using, I would say your test client. 
 17:45: I'll send the request and like connect it to, I would say a test database or a, you know, controlled database environment. 
 17:51: And I'll insert some representative patient data, particularly, and call the API and afterwards they verify that that request is that like actually go through that API layer. 
 18:02: And that business logic also and like we have afterwards we have data access layer and like data and database and comes back with the like correct response. 
 18:11: So yeah, like, and so the simple distinction I use is that, you know, testing tells me that, you know, what, what Python logic works correctly in isolation. 
 18:22: And on the other side, integration testing tells me that the components actually work, you know, correctly together. 
 18:28: So yeah, in our CSCD pipeline they need test run like very frequently I'd say, because you know they were fast and like why the integration test cover, you know, the critical end to end interactions before we promote the service to the next environment. 
 18:42: So yeah, like that's how we can have like integration and new testing in that particular scenario. 
 18:51: You must be aware of the middle words, right? 
 18:53: So, if you build an APA, what are the middle words you add for your endpoints so that, whatever the performance issue which we are discussing, those things can be handled better. 
 19:05: So what are the middle vessel you add? 
 19:07: Or commonly just not don't stick with the typical ones what you add and your API so that you have more control of, everything. 
 19:17: Yeah, so like talking about the middleware part like the main idea of like I. 
 19:23: Yeah, like when I add a new API, I want the common controls to be like handled by the application framework. 
 19:29: So like the developer doesn't, you know, have to reinvent them for every endpoint. 
 19:33: For example, if I add a new patient search API, the endpoint should get, you know, like mainly responsible for valid validating the request and calling the appropriate service. 
 19:42: I would say applying the business logic and returning the response later on. 
 19:46: So like authentication, correlation ID, logging, and like common exception handling. 
 19:51: And, like, most importantly, codes and like other cross-cutting concerns like should already be handled through middleware or shared components. 
 19:59: And like one middleware that I can remember of is, I'd say like. 
 20:05: Like it was the the specific name I don't remember, but like we can use like correlation ID middleware. 
 20:14: In that particular scenario. 
 20:17: How do you, what's the purpose of it and what's a use case for? 
 20:24: OK. 
 20:25: So, like, the main purpose of I say correlation ID is like to trace one request across the entire system and like especially in like when you have multiple microservices. 
 20:35: For example, imagine a patient search request comes into in our API, right? 
 20:40: And like we generate a correlation ID, like say like the request 1234, whatever. 
 20:46: And like attach it to that list and if that API calls another microservice, then like that service talks to the database or like another downstream service and like we propagate the same ID like to do those calls I'd say. 
 21:00: And now it's like, how do you propagate, how do you propagate this correlation. 
 21:07: So like, the, the important part is like that we propagate the same coalition ID instead of generating a new one at every service. 
 21:15: So like it's the request starts at API gateway within like, I'll say like request X. 
 21:20: The fast API service receives it and like, they passes that ID to a downstream service. 
 21:26: So I would say like request headers and like each service then includes the same ID in its logs. 
 21:32: And that way, like, when I search for like request X, then I can follow that request across the entire chain. 
 21:40: And yeah, like, yeah, like if there's a delay or like failure in one particular service, like I can quickly identify where like it happened instead of looking at each service independently. 
 21:50: And in a microservice architecture that you know that becomes really like valuable because you know a single user can request a single user request can, you know, say touch several services before that response comes back, yeah. 
 22:05: How comfortable you are in writing Python codes. 
 22:11: OK. 
 22:12: So, can you write this middle where, where you, you, you know, log, not log, attach the correlation ID. 
 22:22: To do any any NBA. 
 22:24: Yeah, sure. 
 22:26: So like you can share your notepad. 
 22:29: And. 
 22:42: I Yes it is. 
 23:47: So, like, I have imported like WID4. 
 23:52: And yeah, like, OK, the like middle way is basically responsible for like obviously the creating and like propagating a correlation ID for every incoming request. 
 24:04: So yeah, so like first I check the expiration ID header. 
 24:45: When a request enters the API, the middleware runs before the actual endpoint. 
 25:02: After that, like we. 
 25:05: You can just check whether the call is I'd say like already sent up for relation ID. 
 25:12: the requested, in the requested mostly. 
 25:37: And that like, so every, I would say like every request gets I'd say a unique identifier. 
 26:06: From this request.station ID, I saw the ID in request of state. 
 26:13: be believed. 
 26:15: Let's see that typically makes the, you know, like core relation ID available, you know, anywhere inside the application during that request. 
 26:22: For example, like my controller or service or login code can access it. 
 26:26: So yeah. 
 27:20: Oh yeah, this, this will be the code for like the middle one that means like the coalitionality. 
 27:27: So you said your correlation is in the state, is that? 
 27:31: You you're setting, you're, you're settling the correlation. 
 27:34: I didn't state of the request is that. 
 27:45: OK, as you also open decorator, so, what's the decorators? 
 27:51: Can you provide an example of decorator? 
 27:54: Yeah, sure, yeah, sure. 
 27:56: So like decorators in Python, but first I have to write on screen. 
 28:02: You explain what's decorated and tell me what decorator you're gonna create for this, thing and then you can start selecting it. 
 28:08: yeah, perfect. 
 28:10: So like a decorator in Python is like basically, obviously a way to add additional behavior to function, like without changing the original function itself. 
 28:17: For example, like we can create a logging decorator that logs like when a method starts, when it finishes, and like how long I would say like how long it it took. 
 28:26: So yeah. 
 28:28: This is what decorator. 
 28:31: OK. 
 29:10: Hello 1 time from the death of the time. 
 29:34: Passing function as a parameter. 
 29:58: Oh, like, the, the decorator like receives the original function. 
 30:05: And and like then like wrap preserve the original function's name and metadata. 
 30:33: Inside the wrapper like can capture for the start time and like call the actual insurance to use it. 
 30:40: Yeah, I'm showing the result of it. 
 32:27: So you're like. 
 32:30: I like to calculate total Python, you know, I like the Python goes to the wrapper first. 
 32:35: Like it measures the, executes calculate total and. 
 32:41: Yeah, since the, until the vacation time and this is the result. 
0:01: getting the result. 
 0:09: Yeah, so like this is the coat that you can like to decorate this. 
 0:14: OK, you can copy paste the entire code in the chat window. 
 0:18: OK, the code, yeah. 
 0:36: Please stop sharing ice cream, huh. 
 0:41: You can keep it as long as you feel comfortable, you can keep it. 
 0:46: OK, so Yeah, tell me, like it is sent in the chat. 
 0:52: You received it, yeah, OK, fine, I got it. 
 0:55: So how do you manage state in, react applications? 
 1:00: Yeah, like state management in react and I would say like, yeah, this for like, for particularly like I would like usually manage the state based on how broadly that state needs to be shared. 
 1:11: like, for, particularly I would say for the component component level state like I use this use state hook, for example, you know, if I have a form where use into a patient ID and like I can keep that input and loading status in that local state and like for state that needs to be shared between several components, I like generally use a react context with like use context. 
 1:35: And like yeah but like folks well with things like authenticated user like application settings or like shared information that you know like without passing props through many levels and so like for more complex applications where manual components need to read and like update the same state I use the state management library like redux so like depending on like which project requirements that we have. 
 2:01: So yeah You know We had meetings. 
 2:07: OK. 
 2:08: In which scenario you would not prefer to use any local, state management, rather stick with the server state? 
 2:16: like, if I would say like in like big application and like, I'd say like if the data is owned by the back end and can change change like independently of the UI I would generally prefer in that case I, I, I would generally prefer to treat it at a server state or rather than, you know, like dropping it into the local EI state. 
 2:37: like, example, like in our like recent healthcare application, suppose like React UI, you know, request patient for relationship data from a fast API. 
 2:45: So like I wouldn't take that response and like duplicate the entire data set into multiple local states just for the convenience part so like the server remains the source of truth. 
 2:55: And like instead I like I would use a solar state approach with like something I'll say like a react or react query or like a 10 stack query to handle like fetching and like caching I can like refetching and like loading states and lately but error handling so yeah like I have to still use local state for things that are like trulyI specific. 
 3:19: And yeah, so like. 
 3:21: I would use the local state in this scenario. 
 3:26: OK. 
 3:27: do you have any insight on how, memory management works in Python? 
 3:33: You're talking about memory management, right? 
 3:36: entitled. 
 3:38: Yeah, yeah, I'm familiar with that. 
 3:40: So yeah, can you, yeah, little insects, so like Python, like it handles memory management automatically, mainly through like reference counting and like garbage collection, and the primary mechanism is like reference counting, I'd say, because, you know, like every Python object keeps track of, I'll say, like how many references pointed to it and like, like when that count reaches 0, like Python can immediately, you know, release that object's memory. 
 4:07: that could help us a lot. 
 4:09: And the second mechanism is, again, like, from the garbage collection we have a garbage collector like they can handle cases that reference counting alone can, I would say cannot clean them, especially, you know, circular references in like that particular case. 
 4:24: For example, like if two objects reference like they reference each other but like nothing else references them. 
 4:31: in that case, the garbage collector can detect that cycle, and I'll tell, I'll reclaim that memory. 
 4:37: So yeah. 
 4:41: OK. 
 4:43: so, You worked on lambda on the OK, which cloud provider you are using, like I'm. 
 4:53: Yeah, like I, yeah. 
 4:57: So like my family cloud experience has, has been, I'd say with AWS. 
 5:01: Yeah, so OK. 
 5:05: So, We have containers, we have, EC2 instance, and we have lambda. 
 5:16: So, and in which case, case you choose, which option? 
 5:22: OK So. 
 5:25: Like if we have multiple options, we have lambda and like. 
 5:30: And the side like for lambda, like I prefer it for like short-lived event driven or I'd say a lightweight workloads where like I don't want to like manage servers, for example, like processing an S3 event and like I can say or running in small background operation or like exposing a lightweight API through API gateway. 
 5:48: And for the containers part, like, like ECS or like the Joker Services ETS, I prefer them like when I, I have a, you know, like, let's say a long running application or like multiple Python microservices that like need more control over the runtime. 
 6:04: And for like what like what else you have mentioned like EC2, am I correct? 
 6:10: Yeah, yeah, so like for EC2 like I'll choose like it's when I need more direct control over the operating system or I'd say like yeah like or infrastructure or like when I have a workload that doesn't fit well into a I would say a server or container of all the station. 
 6:28: OK. 
 6:29: Lambda got this problem called a cold starts. 
 6:33: Yeah. 
 6:35: Are you aware of it? 
 6:37: Yeah, I'm aware. 
 6:38: Yeah, yeah. 
 6:39: How, how do we reduce that? 
 6:42: Like a cold start typically happens, like in case when like, you know, if like there are, I would say like. 
 6:51: Like, to resolve that, like I, I would keep the lambda package as small as possible, like to particularly to resolve that, that issue or to cool a that issue, and like I would remove unnecessary dependencies and like avoid importing heavy, heavy liabilities unless they, they are actually required. 
 7:09: Secondly, I've moved reusable initialization outside the lamb lambda handler. 
 7:13: For example, like if database clients or like SDK clients, can be initialized at the module level so that like when AWS reuses the same execution environment, like we don't recreate those resources, like for every invocation. 
 7:29: And like if the application has, I would say a pre like predictable latency requirements, I would in that case, like I would use a provision concurrency. 
 7:38: And yeah, like that keeps the number of lamb execution requirements initialized and ready. 
 7:46: OK, what is cereal? 
 7:48: Sorry, yeah. 
 7:51: So you can get. 
 7:55: CNN content delivery network. 
 7:56: Oh yeah, so like, yeah, CDN, as you mentioned, like, content delivery network. 
 8:00: So it's, I would say, basically a distributed network of service that helps deliver content to users from a location that is, you know, I would say geographically closer to them. 
 8:11: For example, like if our application is hosted in an AWS region in the US and like a user is accessing static content. 
 8:19: Or like, you can say JavaScript or like CSS images or like front-end assets from another location. 
 8:26: So like in that case I can use a CDN such as like Amazon Cloudfront, you know, because in that case Cloudfront caches that content and like I'll say like at any locations closer to the user. 
 8:38: So like instead of like every just going all the way back to the original server, I like like the user can get cache content from like nearest edge locations. 
 8:48: So yeah, and, I can think of that that really reduces like latency. 
 8:56: OK. 
 8:57: And what is the disadvantage of having Non-clustered index to me not cluster index to be more specific. 
 9:07: Yeah, so like, a non-cluster index has like a few, like a few disadvantages, mainly around I would say like a storage and like right performance, and the biggest one that I can remember of is like the index is stored separately from the actual like table data. 
 9:23: So like when I query using that index they're like. 
 9:27: You know, that like the database may 1st find the matching index entries and then like perform a look back to the underlying table, like two particularly, you know, like to retrieve columns that are not included in the table, including the index, sorry. 
 9:40: And another disadvantage is that like it's like additional storage. 
 9:45: Like if I create a server non-clustered indexes, like each one requires its own storage, then this is also a disadvantage. 
 9:53: And yeah, right over it, right over it is like also a disadvantage disadvantage of like non-plus index like when we insert update or like daily data, the database may need to update like multiple non-clustered indexes as well. 
 10:06: So yeah. 
 10:08: OK. 
 10:09: What's the deciding factor to select SQL or no SQL? 
 10:14: OK, so, like, so like the most important factor would be like it stores data in like like through and column manner, structured data. 
 10:25: So like I prefer I feel when the data is like highly structured, a relationship between like entities are important. 
 10:32: Because, you know, like a scale maintains relationship between, like components, entities, and like we need a strong, like, you know, consistency and like transaction guarantees, for example, like we had in my project like previously we had a structured relationship of data like that were needed, I would say, reliable joints and like filtering task and constraints. 
 10:52: So like a skill was a good fit, you know, like because like, I'd say like the data relationships that are like very defined. 
 11:00: And on the other side about that like no scale side, like when the data is more flexible or like semis structured. 
 11:07: So in that case I would use no scale database you know that the schema changes frequently or like we need very high scale access with like simple key-based lookups. 
 11:17: So like in that case I can use NoSQL over scale database. 
 11:23: OK, so you, you're aware of Captain. 
 11:26: No, Captain, yeah, I am available. 
 11:30: OK, fine. 
 11:31: So, we know it will provide, which two of these on camp. 
 11:38: Like, put my name, please. 
 11:41: OK, theorem, what is? 
 11:44: Can you explain first? 
 11:45: Yeah, so like, yeah, yeah, the theorem basically is that stands for consistency, availability, and like, the third one is speed and is partial tolerance. 
 11:57: So like consistency shows that, like every lead gets the like most recent right. 
 12:03: And availability ensures us that like every request gets a response, even if, you know, like some notes are, I would say unavailable. 
 12:10: And like the third one, the speed that stands for partial tolerance, the system continues operating despite, you know, like network communication failures if that happens between nodes. 
 12:20: Yeah. 
 12:24: OK. 
 12:25: imagine a situation like, It should have been a SQL database, but you guys started with an OSQL, and now we have to, you know, maintain the asset property of SQL in NoSQL database. 
 12:41: How do we do that? 
 12:43: OK, so like if in that scenario if I started, like with sequel data and like I would like to use a sequel right. 
 12:51: I'll first check whether like the specific move. 
 12:52: So yeah, the scenario is like you cannot go to a SQL because it started application production and some reason they are not OK to migrate as of now or some reason. 
 13:02: So how do we ensure that, the consistent consistency there anything related to that it's a transaction related stuff they decided the wrong architecture. 
 13:11: So how do we ensure that, OK, this database at least gives maximum of asset properties. 
 13:20: So like in that scenario of like architecture, if like it if it is like already in production and like migrating to SQL isn't an option like as you said, then I would work within the more scale model and like explicitly designed for like transactional consistency and like if we are using database like Dynamo DB, the first option is like native transactions that I can look up. 
 13:42: Like for operations that must succeed or like fail together, I would use like a term for transaction right items. 
 13:51: For example, like if one business operation like needs to update a patient record and like a related rela like relationship record, both rights like could, you know, go into the same transaction. 
 14:03: And like if that operation fails, I say that the whole transaction is rolled back. 
 14:08: And after that, like I would also use, I'd say a conditional right and like optimistic, locking. 
 14:15: For example, like each record can have a version number for speed and like when updating it, like I can see essentially, you know, like update this record only if the version is still 5, like if another process already changed it to version 6, the update in that case that update, fails instead of silently overwriting the like a newer, newer data. 
 14:36: And yeah, so that's like the approach, my, the approach that I would follow is like native transactions wherever possible. 
 14:43: And conditional rights and optimistic locking for like concurrency control, that we that we should have. 
 14:50: And like, the one thing that I can remember of is like I don't put in the operations and like controlled retries. 
 14:58: So yeah, that gives us like a strong consistency like where we need it without changing the production database architecture. 
 15:08: Bos canary and Bluere deployments. 
 15:14: It scary and a bit of it like, yeah, yeah, yeah, yeah, so like, yeah, they, they are deployment strategy. 
 15:19: I'm aware of it. 
 15:21: OK, explain, yeah, so like, which one you, you, in your project have you used? 
 15:27: OK, so like, yeah, firstly explain, like explaining like group deployment, it means that like we maintain two environments. 
 15:36: So blue is a current version, production version, and like the green is the new version. 
 15:41: So like we deploy the new application to green and like run over validation and smoke test and then like then afterwards like you know if like we'll switch traffic from blue to green and like if in that case if something goes wrong in that case we can quickly switch traffic back to blue. 
 15:59: for example, like we, like with other containized Python services, in that case, like we could have the current version running in one environment and like deploy the new docker in it separately. 
 16:09: And once green is validated, like we typically move the traffic over and the second one that is candidate deployment is like more gradual, I would say, and if we deploy the new version alongside the existing version. 
 16:24: like, but you know, like, but initially send only a some percentage of traffic to, or let's just 5%, so like we monitor error rates, latency, and I'd say like application behavior. 
 16:36: So yeah, like if everything from that side looks good, we gradually increase it to like, say 25% or like 40, 50% and like eventually, like 100%. 
 16:46: So yeah. 
 16:50: which one, is used in your recent project, it cannot be, I, it might be, other than this strategy, but, what deployment strategy are you using? 
 17:01: Like in my recent Wisconsin DSS project, I used, yeah, like I used, blue-green. 
 17:10: OK. 
 17:14: No experience on canary deployment, right? 
 17:17: No, just a little bit of it, yeah, OK, that's fine. 
 17:24: OK, one second, I, I just got your resume very late, so I'm not looking at your resume. 
 17:31: I'm just looking at the change and try to see if I covered all the topics, one second. 
 17:49: Is it a 13 years experience, right? 
 17:53: OK. 
 18:05: OK. 
 18:06: Any experience towards CA? 
 18:10: Any experience towards AAI? 
 18:12: Yeah, I have worked with AAA. 
 18:17: Yeah, what kind of experience have you used as an assistant or you built any, AA system? 
 18:23: like, yeah, I have used assistance also like, I have used clot. 
 18:26: I have used, a co-pilot for like automating our application, like, yeah, yeah, like, yeah, efficiently, like for efficient working and like. 
 18:37: Yeah, for the like hands-on experience side with AI and like I have hands experienced AI as well and generative AIM. 
 18:45: So like talking about more recently, I, I have been working with, I, I'll say like open AI, land change and entic AI patterns like mainly, you know, like looking at how we can use them in, enterprise applications rather than, you know, just like experimenting with chatbots. 
 19:04: OK, those were on your application or it's your own personal exploration. 
 19:09: No, like I have used it in like, the, the booking. 
 19:12: OK, then give me, yeah, give me one slogan you've used, to automate something or improvise something or created some agent. 
 19:22: On pipeline did so like one for example, for if I will give you an example like I explore energetic workflow using open A and land chain where like, you know, the agent receives some business or let's say or technical request that determines like what information it needs and like, you know, using the appropriate tool or I'd say like API to like retire that information and like then produces a structured response. 
 19:49: So like the idea was, let's say not to, like, you know, let the model directly change production systems. 
 19:56: I kept the actual businesses operations behind controlled in Python or you can say like fast APIs with validation and like authorization in place. 
 20:04: Yeah, like from an architectural perspective, I was like mainly focused on mostly like how the agent interacts with tools, tools and like how we pass context and like how we handle errors and retries and like how we keep the workflow say controlled and like auditable. 
 20:23: So yeah, like I have worked with the concept of creating an agents and like automating workflows using OpenAI or Latin. 
 20:33: OK. 
 20:35: Yeah, I, I'm sorry. 
 20:41: Yeah, I'm done with my questions. 
 20:42: Do you have anything? 
 20:43: Yeah, like, I have two major questions. 
 20:46: The first one would be like, what will be the rules and responsibilities like, if I would be hired for this role. 
 20:54: OK. 
 20:55: Well, Here, like this is the first round, OK, when we do the screening to after that you'll be, given to client, and they'll be screening you. 
 21:08: That's a process and, Looking at your JD of 10+, mostly it's either be senior engineer role and what of IC is what they're looking at, Python developer who can do them, who has well versed knowledge on the architecture in an application. 
 21:25: And, Yeah, that's a JD I got. 
 21:29: So what's your roles and responsibility would be that I'm completely not because that client is, it's not the client I'm working for. 
 21:36: So I don't have much idea. 
 21:38: And, they are in, film tech insurance, I guess. 
 21:44: actually is something the client name is, maybe, yeah, maybe you can, ask more of these questions with the recruiter. 
 21:54: They'll be able to, give you answers like what's the time zone, what's your, roles and responsibilities, and, what are the, product they have. 
 22:03: and I think it's a product company only, but you can ask, those details with, recruiter. 
 22:08: I think next question also I might not be able to answer, but you ask me if I know, I'll tell you. 
 22:13: OK, perfect. 
 22:13: That works. 
 22:15: so like, one major question that I have, like how many rounds like would be there in that process. 
 22:22: Like a specific number, that's a recruit a specific question. 
 22:28: So that's what I usually like we do, when I got into this company, so I got 3 roles, one with the screening which is from Missurient other two were from the, client. 
 22:39: So, I cannot say the same. 
 22:40: It happened with you, because one of my colleagues or just one room with a client and they got selected. 
 22:44: So based on the seniority and, other, situations, the client, how they like it, they might take one or two rooms, but I'm thinking mostly it won't be more than 3 rounds. 
 22:56: Yeah, so like that works for me, that makes sense. 
 23:01: It was OK. 
 23:03: But again this question if you ask a recruiter, OK, they'll be answering you. 
 23:10: Yeah, OK, thanks, Ari. 
 23:12: I'll share the feedback with the regulator, and, we can disconnect it. 
 23:18: Yeah, thanks. 
 23:19: Like, have a good day. 
 23:19: Bye-bye. 
 23:20: See you. 
 23:21: You too, yeah. 
