0:00: Because with the A world right and with the a tools evolving right we want to have that we, we take this in with too much of transparency, yeah. 
 0:11: OK, the customers are expecting the same. 
 0:14: OK. 
 0:15: OK, thank you. 
 0:19: yeah, before starting, can you take the photo? 
 0:21: hey, I'm not showing the photo ID, just give me a second. 
 0:25: Like it was in the, other room. 
 0:27: OK, sure, sure, yeah, just. 
 0:40: Got it. 
 0:42: That's My idea. 
 0:48: Copygu. 
 0:49: Yeah. 
 0:51: Yeah, one second, yes. 
 0:55: I'm picking up. 
 1:00: Yeah, I don't, thank you, yeah, Thank you so much, sir. 
 1:09: OK, we can get started. 
 1:11: you want to brief yourself quickly for two minutes? 
 1:14: Yeah, sure. 
 1:14: Like, my name is Susan Mohammad. 
 1:17: like I have, 10 years of experience like as a senior back in, full set. 
 1:22: Data and like AI engineer, primarily like my background includes, building the enterprise applications, cloud native, solutions, data platforms, and like mostly, more recently, like the GI and Agentic AI systems and also like I completed my bachelor's in the computer science from like Osmani University in India, like, like later on my other masters in, CAS and currently like. 
 1:47: I'm working with this other health as a like lead data, developer. 
 1:52: My primary focus is on like building the AI powered healthcare solutions using the Python fast API, OpenAI GPT, also the, land chain Pinecon Cuban Aids, and, cloud technologies also. 
 2:06: And one of the like major projects I worked on was the AI Power clinical knowledge system. 
 2:12: Basically, the goal was to help the healthcare professionals quickly the access medical guidelines, patients, care procedures and operational documents like through, manual, language conversions and also like I, I design and develop a racks, rack-based architectures using the, Python fast API, OpenAI, Lang chain Pinecon and we like. 
 2:38: process the thousands of healthcare documents generated embeddings, and store them in the vector databases. 
 2:44: And apart from that implementing the semantic search capabilities like to retrieve the higher relevant information and we also like implementing multi-agent workflows using la chain agents like where the different agents handle document document retrieval, so and the compliance validation. 
 3:03: So the significantly improve the knowledge, accessibility and reduce the manual effort like across the departments and. 
 3:11: from the infrastructure side, like I work extensively with the Cubans Roger, data form, CIC department, and, like, cloud native, deployments also, and I collaborated like closely with the data engineers, data scientists, architects, and some business stakeholders like to deliver, secure and the scalable AI solutions. 
 3:31: And before such help, like I worked, worked with the, America Bank,, like the Paxel, and, I gained like a strong experience in the data engineering, so yeah, that's pretty much helped me. 
 3:46: Thank you. 
 3:46: Thank you for that, Jose. 
 3:48: OK. 
 3:49: So I will get to 3 parts. 
 3:52: OK, so I want to 4 parts in fact. 
 3:55: OK, I will just, get into a web development phase, then cloud, then MLAA ops, but then, then, dev ops, infrastructure site. 
 4:07: OK, that's how I will schedule this interview too and not take much of your time, but quickly, OK. 
 4:13: So coming to, first thing, right, you know that, you were working on. 
 4:19: I correct. 
 4:21: OK, so tell me something. 
 4:23: Then, you will use the fast API. 
 4:25: Then you will use better. 
 4:27: When you use class. 
 4:28: Any use cases. 
 4:29: Can you give me? 
 4:30: Yeah, sure. 
 4:30: Like, like, basically on these, these three, like I worked extensively on that like Django, class or the fast API, and basically, when I use the fast API, it's like we have the, like, work on the, like the APIs things and, like, basically, I typically use fast API like when building high performance APIs, microservices, and the AI applications, and the, we can save the real-time, back end services, OK? 
 5:02: For example, in my the current, project, like we build an AI powered clinical knowledge system. 
 5:09: are using fast API like since like we were like integrating open AI models, lang chain, Pinecon and the red pipelines, like we, we needed like the as synchronous processing and the like fast response times and the fast, fast API was like best choice like because it provides the asking supports, Automatic API documentations through Swagger type validation. 
 5:34: So like whenever like I'm building AI services, LLM applications or microservices, I generally prefer fast AP and I use flask when the application is relatively lightweight and does not require a lot of like built-in features. 
 5:50: For example, in, in some like. 
 5:53: internal tools and the proof of concept projects we use Flash to like quickly expose ML, models like through rest APIs. 
 6:01: So Flas is like, simple, flexible, and easy to set up. 
 6:05: Like if the application is small and we, we want complete control over the architecture. 
 6:09: Sola there's like good options and this, and I use general, I like building large enterprise application that that like require many features. 
 6:20: like, out of the box, for example, like, if, if we need, users authentications role-based access control, admin dashboards, and ORM supports, so, like, and the data integration, so Jan will help us like to build these features quickly, suppose like, we are like developing a healthcare management portal or the banking applications. 
 6:42: So like we have multiple modules like user's permissions and also the, so in that case, Django is usually preferred choice because it's like follows the the batteries include the approach. 
 6:57: And OK, see, so you have to productionize this, OK, so there is something for for authentication, right? 
 7:05: Authentication you need, right? 
 7:06: Which one do you generally prefer, for authentication. 
 7:10: Oh, like for the authentication perspective, like, we generally, in the recent project, like the approach depends on like the type of applications we are like building. 
 7:21: In most, my recent past TPP enterprise and the application have like primary use JWT and along with over 2.0 like for authentication and authorizations, for example, like in the clinical knowledge, assistant projects, users authenticated, and say secure login mechanism. 
 7:40: And after like the successful authentication or GWT Access to like token was like generated. 
 7:48: That token was like then passed in API request and the fast API evaluate the token before allowing access to like protected endpoints and like for enterprise applications, we often integrated with SSO providers such as Azure, AD Opta or like Google identity with the OR 2.0 and Open ID Connect. 
 8:09: so these, these allow centralized authentication and the better security management. 
 8:14: OK, so there is something called when you use Python, right, there is something called async and await, correct? 
 8:20: You heard of it, right? 
 8:21: So, how these two works under the hood, do you know, a sync, a synchronized, yeah, basically for like, talking to her like a sing and it like I use for Python for a synchronous programming generally, basically which allows multiple input on put bound operations like 2. 
 8:41: Run the concurrently without blocking the application. 
 8:44: So under the hood, like Python uses an event loop typically provided by the async IO library. 
 8:52: And when I like define a function using async D, Python creates a core routine instead of like executing the like the function immediately. 
 9:02: So, like, basically the asking dev get data things like these function returns the core routine object. 
 9:09: So when a code reach an await statement, Python like temporarily forces that the core routine and gives control back to the event loop and like while the database call is like. 
 9:21: waiting for a response, the event loop can execute other core routines instead of like keeping the thread, ideally. 
 9:29: So once, the database response arrives, like the event loop, resumes the paused kind of core routine like where the, where it is stopped. 
 9:38: So main, main benefit is that the single thread can efficiently handle thousands of like input output operations such as the if they calls, database queries, and like file operations without like. 
 9:52: without creating a thread for like, each request. 
 9:55: OK. 
 9:57: OK, so, OK, suppose you're designing an APA. 
 10:00: OK. 
 10:01: There is something called how you handle variation, filtering, questioning, sorting kind of things. 
 10:06: How do you handle this? 
 10:06: How do you design this for all these 4, any APA, when you build that, these 4 are very important. 
 10:12: OK. 
 10:12: Regulation is important. 
 10:13: Sorting is important. 
 10:15: so, filtering is important, and washing is important. 
 10:19: These things, have. 
 10:20: , we'll give you a quicker time when you do a get, get request or a pull request, however, whatever you do, right? 
 10:28: So how do you handle, how do you design these four? 
 10:31: Absolutely, like, when designing the production APIs, I always considered the pages and sorting because, returning large data set in a single response can impact performance and the user experience. 
 10:43: So like. 
 10:44: The most common approach I use in paging nation, I use a limit and offset paging nations. 
 10:50: if there are like 1000 records, we are like only returns the small subsets such as like 20 or 50 records per request. 
 10:58: like for large data set, I prefer cursor-based paging nation because it, it performs better than offset paging nations and avoid like, issues with the newly inserted records and, and the filtering. 
 11:11: generally I, I usually implement filtering through query parameters, like in healthcare. 
 11:17: users often like need to filter reports by like department, date range, status provider also, location. 
 11:25: So the back end dynamically builds the query like based on the provided filters and for the sorting like I generally allow users to sort data using query parameters. 
 11:36: Like generally it helps to drive the data in order they need without additional processing on the front end in in like fast API. 
 11:45: I typically define these as the query parameters with validations like fast effect automatically validates inputs and like generates swagger documentations. 
 11:57: OK. 
 12:00: Then, you know, what is concurrency in paraism when you use in Python, like how do it works, OK, basically, talking to our like concurrency, concurrency, basically, it's like we can say. 
 12:15: Like both are like a related concept, but the like means like conferencing means handling multiple tasks at the same time by like switching between them efficiently. 
 12:27: like the task may not actually run simultaneously instead the system manages them in a way that makes progress or like on multiple tasks. 
 12:39: for example, Like in in fast TP application, if, if one request is, like waiting for the database response, the event loop can process another request instead of like, like setting ideally. 
 12:52: So this is concurrency, and, parallelism is basically means, multiple tasks are like actually executing at the same time using multiple CPU cores or the processors like, if, if I'm training, training machine learning model or processing large data sets I can use. 
 13:14: Multiple pro processes like running on the different CPU cores and simultaneously. 
 13:20: So like in a simple analogy like multiple chefs are like, we can say cooking different dishes at the same time in the same kitchen. 
 13:29: So these are like the, good example for this. 
 13:32: And in, in Python like for like input output, bound workload such as, API calls, database queries like. 
 13:41: network because I usually use asking a very fast depend since this gives like concurrency can improve the throughput. 
 13:48: But So see, for example, I'm working in Cigna.com. 
 13:52: OK, when I do a Cigna.com from India or something, right, it, it takes time to load this, OK. 
 13:57: This is what something called as, there is a time lag. 
 14:01: OK. 
 14:02: How do you, my question to you is, how do you. 
 14:07: This latency, OK, what are the name may be the common, how do you diagnose it, basically, for, for avoiding the latency, and, let me add also, OK, then after, it tries in somewhere in the world, it times food also, OK, the pain does not come, yeah. 
 14:27: It's like if, if users in India India like accessing an application hosted in the US like there will naturally be like the network latency because every request has to like travel like the thousands of miles between the clients and the server. 
 14:44: So to reduce the latency, like I would look at the multiple layers like the CDM, the like for like the static content such as like images, CSS Java and document like. 
 14:56: I would use a CDN like the cloud CDN and the cloud front so the the person next to door, the person next to your door, it's the same situation. 
 15:05: What you will do. 
 15:07: sorry? 
 15:08: The person next to your door goes for Cigna.com. 
 15:11: He also faces the same issue. 
 15:14: Latency, what might be occur? 
 15:16: or how do you digress it? 
 15:17: OK, if it's like next to door, like, what, what I usually do, for like if, if both like I and the person like sitting next to me are like expecting the same latency like issue while accessing the app, the 1st, 1st assumption would be like the problem is like probably not user specific. 
 15:39: First, like check where the latency is happening. 
 15:42: Like I would open the browser developer tools and look, look at the network tab. 
 15:46: Like I would check the DNS lookup time or TCP connections times, SSL, like handshake time or TTFP. 
 15:54: So basically this helps to identify whether the delay is like coming from network or like from the server. 
 16:01: And second, like check it if like a printed on the back end like if STML loads quickly, but APR like slow, then then the back end maybe the model neck so. 
 16:10: If APIs are like fast but the page renders slowly, then it would be the front-end issues such as the. 
 16:16: Large JavaScript bundles, unoptimized asset, and too many AP calls and also like the check server side mattresses, like I would look at the monitoring dashboards such as the CPU utilizations, memory usage request latency. 
 16:30: So if CPU is like, constantly high, higher requests and like queuing up, then the application servers may be overloaded and also I checked the database performance like. 
 16:41: I would investigate the query, execution times, log contentions, and after that, like check the external dependencies like open AI APIs, third party services, authentication providers. 
 16:56: so, OK, coming back to database, right, you know something called N +1 problems, query problems, n +1 query. 
 17:04: So what is that? 
 17:05: How do you address that? 
 17:07: Yeah, how do you like the, it's a common one. 
 17:09: It's a very, very common one, like the famous problem, the lead code basically like it is a, common performance issue in like application we can say, like. 
 17:21: using the ORMs like the SL Alchemy or the Django environment, basically it happens when the application execute, execute one query to fetch the main data and then executes and additional queries to like fetch related data for like each record. 
 17:35: For example, like suppose I fetch 100 patients, OK, and now for like each patient if the application separately queries the doctor information. 
 17:45: Then like for the 100 patients, the application will like execute like 1 query for patient, 100 queries for doctor, so total is like 101 queries. 
 17:54: So this is called the N + 1 problem. 
 17:57: basically, why is it bad because Every database calls involves like network round there like query executions, connection users. 
 18:06: So, as data grows, performance degrades significantly. 
 18:10: For example, like 10 records gives the 11 queries, 100 records gives the 101 queries, and 1000 record gives 1,001 queries. 
 18:19: So latency increases dramatically. 
 18:21: Easily to solve this like. 
 18:23: The most common solution is either loading or using the joints. 
 18:26: Like instead of making separate queries, I fetch related data in a single query. 
 18:33: Oh, OK, thank you. 
 18:35: So, you know, there are different isolation levels, right, when you design up a, a, a database, right? 
 18:41: Do you know, how those transaction, those works actually using different how database works when you use a different isolation level? 
 18:50: Do you know? 
 18:51: Yeah, basically. 
 18:53: Isolation levels are like the part of like the asset properties for of the database transactions. 
 19:00: And they control like how multiple transactions interact with each other when they run concurrently. 
 19:06: So, the main goal is to balance the data consistency and the performance. 
 19:11: Like there are some four common isolation level like first is, read and committed. 
 19:15: Like this is the lowest isolation level. 
 19:18: Like the transaction can read data that another transaction has modified but like not yet committed. 
 19:23: So this can, lead, to the dirty read. 
 19:27: And there was read committed like this is the most commonly used isolation level like a transaction can only read committed data and also the repeated, repeatable read like. 
 19:40: These guarantees that if, if I read a row once, I will get the same value through throughout the transactions and also the 4 was like 41 is like the serializable like this is the highest isolation level like the database behaves as if, if transactions are like executed one after another. 
 20:00: OK, thank you. 
 20:01: So, see, generally in database like that you do indexing to improve the performance of a, given application or a given database to, to fetch, good. 
 20:11: But in this case, right, suppose you have set up an index, it instead of improving the performance, it is hurting the performance. 
 20:19: What might be the potential issues? 
 20:20: What you have seen. 
 20:24: For the performance perspective, like indexing, I'm just doing the indexing, OK? 
 20:28: You have, you have put index on certain columns. 
 20:30: You have a database of around, thing that has around 3 or 5 million records, for example, you have placed indexing so that retrieval is faster and the read is faster and everything, but it is hurting that what would be the main cause and how do you address this, well, like. 
 20:45: indexes usually improve the read performance. 
 20:48: Like, I see the situations where, like, adding indexes like actually hurts overall the database performance. 
 20:54: So first issue is like the two main indexes. 
 20:56: Like every time we, we perform an insert update or delete the database, like not only updates the table, like, but also updates like the associated indexes. 
 21:07: For example, like, if, if, if, if a table has 8 or 10 indexes, every insert operations like maintain all those indexes. 
 21:16: So as a result, like insert operations become slower, update operations become slower. 
 21:21: So in the storage like increases. 
 21:23: So this, this is like one of the most common issues like I have seen. 
 21:27: And second is, index or low cardiotic columns. 
 21:30: Like sometimes developers create indexes or like the columns that have like very few unique values. 
 21:37: Thank you. 
 21:38: OK, so, and, I'm closing on the subject, right? 
 21:41: So when do you choose a microservice stuff a monolithic? 
 21:45: So not always it is recommended you have to go to microservices architecture, OK, because that is a little expensive. 
 21:50: OK, so it, it can be monolithic itself. 
 21:53: Give me a use case of both the things, like I don't start with microservices by default. 
 21:59: Like the job depends on the business requirements, team size, deliverability needs, and those like system complexity. 
 22:06: So, when I would choose monolithic, like if, if application is like small, small to medium size, build, build by the small team also has tightly coupled the business logic. 
 22:17: Or does not require the independent scaling it, then I would like to start with the monolithic. 
 22:22: Like a monolithic is basically it's like easier to develop, easier to test, easier like to deploy and debug. 
 22:28: Like for many business applications, a, a well designed monolithic is like actually the right choice initially. 
 22:36: And for like a microservices, I usually considered microservices when. 
 22:41: Independent, scaling are like requirements like different modules have the different traffic patterns, for example, in a healthcare platform, authentication service, patient service, clinical document service. 
 22:53: so these AI service may receive the significantly more traffic and require the GPU resources. 
 22:59: So like instead of like scaling the entire application, like I can scale only the AI services and also for like the large and the complex application like, as, as system grew, maintaining a single like code base becomes difficult. 
 23:13: So microservices allow us to break the system into the smaller business domains, for example, like the US services, billing service, notification service, and each service are like the clear ownership. 
 23:24: And also like if several teams are like working simultaneously, microservices like enable independent development and deployment. 
 23:32: So one team can deploy changes to the service without affecting the bill billing service. 
 23:40: I get it. 
 23:40: OK. 
 23:42: So have you, have you heard about rate limiting like it's a rate limiting rate platform? 
 23:49: Yeah, like,, like I was work on, on the, rate limiting. 
 23:53: Like it's a mechanism that used to control like how many, requests a user, client, or like API consumer can make, within like the specific time period, so. 
 24:05: The primary goal was like to prevent abuse, protect the APIs like from excessive traffic, avoid the videos like the situations, and show the see what will happen when you decide right. 
 24:17: So these are all agreed, OK. 
 24:19: So if I, if I, I'm a genuine user, I hit 100 times. 
 24:22: OK, I hit 100 times, OK, and you have implemented, rate limiting on it, but I'm a genuine user. 
 24:28: How do you handle that, Basically, like for handling these types of situations, like, generally, what I do, like, like, it's like, like I start with the security things actually, like if, if I was a genuine user, like hitting the, the API 100 times, like I would not immediately assume it, it's abuse. 
 24:52: Like first, I, I would understand the business use cases for, for example, like If it is a like healthcare application and like AI chatbot or like a reporting dashboard, legitimate users might generate like large number of requests like in a short period and in such cases like I usually implement thyroid rate limiting rather than the single hard limit. 
 25:14: OK. 
 25:14: And another approach is like using the token bucket algorithm like suppose the limit is 100 requests per per minute. 
 25:23: But we allow the bust capacity is like 150 requests, so a genuine users can occasionally exceed the normal rate without like getting blocked immediately. 
0:00: And in such cases, like I usually implement thyroid rate limiting rather than the single hour limit. 
 0:06: OK. 
 0:07: And another approach is like using the token bucket algorithm. 
 0:11: Like, suppose the limit is 100 requests per per minute, but we allow the bus capacity is like 150 requests. 
 0:19: So a genuine user occasionally exceed the normal rate without like getting blocked, immediately. 
 0:25: Thank you, thank you for that answer. 
 0:26: OK, I'll quickly, I'll quickly move on to, do you use AWS workshop or what is the cloud which you have used? 
 0:34: Oh yeah, like, basically I will work on all three like your GCP, and, AWS, yeah, like I also I I worked on with AWS. 
 0:43: OK, so, so, our customer is fully AWS workshop. 
 0:47: I would ask you one question. 
 0:48: How do you? 
 0:49: They send a scalable application development on AWS. 
 0:51: Just a simple thing. 
 0:53: You can pick up any application. 
 0:54: You, you tell me what services use a simple scalable application deployment on AWS. 
 1:01: when, when designing the scalable application on AWS, like I typically like focus on availability, scalability, security, performance, and, and last, like very important, the cost optimization. 
 1:13: OK, so, basically the high level architectures like users access the application through the, like route 53. 
 1:20: Then we have the load balances application layer and last we have the database layer. 
 1:24: So like for front end, like for front end application, I, I would like host static assets in the S3 or the cloud front. 
 1:31: Like cloud front act as a CDN and the soft content like from edge locations closer to users, reduce the latency and like for back back end services. 
 1:42: I would typically use ECS or like EKS for containize application. 
 1:46: EC to like for like auto scaling the groups, lambda for like surless workloads and like for the fast EPI based application, I would conronize the application using Docker and deploy it into the ETS or like ECS and and application load balances distributes traffic across the multiple instances. 
 2:06: And like if traffic increases auto killing automatically launches additional instances and for like the database layer for like transactional workloads, Amazon RDS like for both and the Myers like and for like very high skill workloads Dynamo DB like I would configure the. 
 2:27: read replicas, multi, easier deployments like to improve the availability and the scalability. 
 2:34: And also like I use elastic cache, for like the caching layer, Amazon S3 for the story layer, and IM rules and the policies like for the security. 
 2:46: OK, thank you for that OK. 
 2:48: See, one final question, I don't want to go too, too technical. 
 2:51: How do you handle it? 
 2:52: OK, so I made an application. 
 2:54: AWS. 
 2:54: My monthly cost for this application is $300,000. 
 2:57: OK, I have been asked to bring down $200,000. 
 3:00: How do you approach it? 
 3:02: OK. 
 3:03: generally, In that type of scenario, like, usually, my approach was like, we can say. 
 3:13: very common, like, generally for that, Usually, we can say Like I start with Like starting the cost analysis, like I would use the AWS Cost Explorer, AWS budgets, CloudWatch, on my devices, and to identify the top, cost drivers, typically the major contributors are like, easy to guess, compute, RDS database, data transfer cost, S3 storage, load balance, and the third party services. 
 3:47: So the first question, like I ask is like which, which services are consuming the majority of the, like the, $3000 because usually 70 to 80% of the cost comes from the few services. 
 4:00: And right sizing resources like one common issue is like over overprovisioning like for example, large ECT stands running at the 10 to 15% CPU utilizations, oversized pins notes on the databases with unused capa capacity and I would like to analyze utilizations devices and Downsize resources were like appropriate. 
 4:23: So these alone like can often reduce the cost significantly and also we have water staining. 
 4:29: Sometimes the resources run 24/7 even when the traffic is low, so. 
 4:35: I would implement all scaling groups you a cluster or scaler like also the horizontal for scaler like so infrastructure grows and sing based on the demand. 
 4:46: OK. 
 4:48: OK, so going on to the next topic, data engineering, right, which is your core, right? 
 4:53: That's what you said, right? 
 4:54: So, I have a data set, OK, which is around, 300 GB, OK. 
 5:01: it is available in Oracle, OK. 
 5:02: I have been asked to bring it to cloud and process it, for example, you know, data bricks. 
 5:10: OK, I've been asked to, consume data from our database. 
 5:14: OK, then, target player, OK, live with all the ET logics, CFP logics, and all, OK. 
 5:19: The target player is going to be database. 
 5:21: How do you do it? 
 5:22: And your cloud provider this database, generally. 
 5:29: It was like for the 100 GB oracle data set like I would avoid the extracting everything manually like through the application code. 
 5:37: I would use a data injections pipeline designed for like the large scale transfers first, like I would analyze the source tables, data volumes, the frequencies, and like whether this is like one-time migration or an ongoing incremental load. 
 5:53: And for the initial load, I would extract data from Oracle in the parallel batches and land it into the cloud storage like such as Azure Data Lake storage. 
 6:04: From there, the data bricks can read the data and perform transformation logic using the Spark, which is like, designing for large scale scale scale distributor processing and for like ongoing loads, like I would, implement the incremental injections using time stamp columns, CDC, or like primary the key base tracking, so we are like only processing new or the team reports instead of like, reloading the entire, 300 GB every time and in data breaks. 
 6:34: like, I would implement validation checks, data quality rules, cleansing, and like right processes data into the data lake tables like for downstream, consumption, and finally, and last like I would like, orchestrate the workflow using this scheduler, implement monitoring and the, failure handling and maintaining like audit logs through like track successful and the failed loads. 
 7:00: Oh OK, moving on to see, you use, what to say. 
 7:17: What do you use for injection generally injection from unlike my database unlike databases to different targetla, for example, Oracle, SQL no legacy databases to RDS Dynamo DVR, whatever it is. 
 7:32: What are all injection patterns you use. 
 7:35: you know, like for the details to cloud like I use JDVC connectors for the direct integrations and in Azure environments like I also, also like work with the Azure data before like orchestrating data movement within the systems and the cloud platforms and like for the data breaks especially data can be integrated using JDBC connections, breaks like connector schedule the pipelines or like. 
 8:00: Cloud destroyer like handling zones where the data is like first loaded and then processed by the spark jobs and like. 
 8:07: For like the large data sets, I prefer incremental loading or like the CDC based approaches rather than like full loads of imp improve improved performance and reduce the processing cost. 
 8:20: I OK, OK, so, coming back to Kuberneti, right, so you also know Kuberne is correct. 
 8:32: So how do you choose say, for example, right, you do you you use OpenShift yeah. 
 8:42: OK, so you generally provision parts for this, right, in a micro, services architecture, right? 
 8:48: So certainly, there is some bottleneck. 
 8:50: OK, too much of parts are getting provisioned and unnecessary is there. 
 8:54: It is impacting the other application and the environment, OK. 
 8:57: So in in a given environment there will be 4 or 5 applications. 
 9:01: OK, so. 
 9:06: 2nd year. 
 9:08: It's not. 
 9:10: So 00, I'm gonna call one second. 
 9:15: OK, sorry. 
 9:16: So, so, go ahead with that answer. 
 9:17: OK. 
 9:20: like you did not ask the question. 
 9:22: So, like, oh, I will not ask. 
 9:24: So there are, too much of ports is there, OK. 
 9:27: So usually you'd, deploy an application in a, in, in a containers, OK. 
 9:35: So, a lot of provision, the same environment, right, for example, you take the, a lot of parts are getting, a lot of parts are getting, provision, OK, because of that, the existing application which you are trying to launch, it's not launching, it's failing, OK, for example, in the, Jenkins pipeline, OK, how do you handle this. 
 10:00: I really like, what I do for like handling these type of scenarios, like, firstly, they're like that, the first thing I, I, I would like to do is like verify why the deployment is failing. 
 10:13: Like I, I check the board events deployment status and the scheduler messages using the Cubs or OpenShift commands and if the error shows, insufficient CPU or the memory, then the cluster is like likely the source content. 
 10:30: Next, I identify like which name spaces or deployment of supports are like consuming most of the resources. 
 10:37: So in many cases I've seen application over request. 
 10:41: CPU memory or like having unnecessary replica accounts and also I would, I would remove the report requests and the limits, remove the like unused workloads and the right size deployments and like if the cluster is like generally running out of the capacity and, and the workload is very then I like scale, scale the work workload so like expand the cluster capacity and long term like I enforce the resource quotas and, consumes the excessive resources and impact other things like sharing the cluster. 
 11:16: Thank you. 
 11:17: OK, moving on to a certain, I'll move on to, MLOs. 
 11:22: OK, you know what is an MLOps? 
 11:24: What is an ML flow? 
 11:26: Why do you have that? 
 11:27: It's very important in current day's work, right? 
 11:30: Like it's, like machine learning operations like is the like practice of application develops principles to the machine learning life cycle. 
 11:38: Like the goal is to like automate and manage the processes of building, training, and deploying the monitoring and the maintaining ML models in the production like just like, DevOps helps to manage the software delivery. 
 11:52: analogs helps to manage the end to end, you can say life cycle of ML models like which ensure the reliability, scalability, governments, and the reproducibility. 
 12:02: And also in my recent project like my involvement was like. 
 12:07: Primary on the conceptions and deployment side. 
 12:10: So data scientists like would train the model and data breaks and like all the backroom services would consume the model outputs and expose them like through fast you can as well. 
 12:20: So I also work with the CICD automation, containers deployments, monitoring authentication and, and, and integration layers that help, operationalize those ML-driven services. 
 12:34: Oh, OK. 
 12:36: OK. 
 12:38: see, you, you actually, how do you develop a new model? 
 12:43: OK, you have a data set, OK, you do, Do you know how you develop the model for a given use case you have, you, you take a sample data set some you do training and testing, then you perform, various hyperparameter tuning at the at the last ray you are implementing a model when you implement that model, right. 
 13:05: that that is a machine learning model, OK. 
 13:07: Take a healthcare or taken any use case, OK. 
 13:10: But when you, when you, fruit of the world production, I said, OK, it is not giving whatever is decide performance or whatever is expected. 
 13:21: How do you handle that, sir? 
 13:24: generally, model development starts with like understanding the business problems. 
 13:30: Collecting and preparing the data sets, handling the missing values and outliers. 
 13:34: So performance feature engineing and splitting, the data into the training and the test data sets. 
 13:40: Then the data scientists like select an appropriate algorithm, train the model, evaluate like using the relevant methods, tune the parameters and like evaluate the results. 
 13:50: And once the like model is approved, my enrollment like usually around the deployment CP indications. 
 13:57: consuming the model outputs, authentication and making like model to available to downstream application through the production services. 
 14:05: Oh, OK, so my, my, my question is you implemented, but it is not after feature you're doing everything you picked up, you picked up those features which is not which is required, which you know which is not required, which is not of least importance, OK? 
 14:19: You got a a perfect accuracy score. 
 14:21: You, you got a perfect, all those 4 parameters what we used to do, right? 
 14:24: So all those things, right, false negative, all those things you have done, that conversion matrix, right, correlation matrix, everything you have done it, but when you implement it, it is not working aspect. 
 14:37: OK, like For generally what I do for these type of scenarios, like if, if model shows, you can say excellent matterss during the training and the validation but performs poorly in the production, then first thing I would use suspect, is like the gap between the training model and the real world data. 
 14:56: So the model may have been trained on historical data that does not accurately represent the current production patterns, and, this is like the often called the. 
 15:08: Data drift or like a concept drift and I would like to compare production input like within the training data set review the feature distribution and verify that the some preprocessing and the feature engineering steps are like being applied consistently and I will also check whether the the like the missing field system might change in current transformation or data quality issues in the production pipeline. 
 15:31: I'm addicted. 
 15:32: OK. 
 15:33: OK, moving on to the next one, right? 
 15:36: What do you understand really about agent AI? 
 15:39: Over it? 
 15:40: What do you understand right now on agent AI? 
 15:45: generally for like the agentic AI is basically does beyond the traditional AI model that simply responds to, prompts and agenttic AI is like make make decisions, plan multiple steps like use, external tools or APSs gather the gather information and. 
 16:04: Execute actions to like achieve a goal with limited human human interaction. 
 16:08: For example, like we can say like instead of just answering the question, an agent could retrieve data from multiple systems, analyze the results, like all APIs generate a report, and then provide the final output. 
 16:22: So the key difference is that the Agenticge is goal-oriented and can take action, whereas the traditional LM primarily generates responses. 
 16:31: OK, fantastic. 
 16:33: When you use a generative one gene I use case, when you do an agentic AI use case, just a small thing, like I would usegen AI when the output needs to be created, dynamically rather than the selected from the predefined rules. 
 16:50: Differ. 
 16:51: My battery is getting over here. 
 16:53: So, my next question is, what are embeddings? 
 16:56: How are they used in semantic search? 
 16:58: Means that, embeddings, right? 
 17:01: You use in semantic search, right? 
 17:02: How they are used to embeddings are basically, are like numerical vector representation of data. 
 17:09: Such as text, documents, images, or like the other content. 
 17:13: So the idea is that content with similar meaning gets represented by vectors that are like close together in the vector space, unlike the keyword search em medics capture. 
 17:25: And like semantic meaning. 
 17:27: So two sentences can use completely different words but still have similar embeddings if, if they convert the same intent. 
 17:37: OK. 
 17:39: OK, you said that you're using light chain, is that correct? 
 17:42: OK. 
 17:43: So how would is different from custom orchestration Lang chain. 
 17:48: Langchain is a general thing which you can use, but how it is different? 
 17:54: Langin is like essentially a framework that helps to orchestrate the LLM application by providing, we can say, built-in components for like prompt chains, agents, memory, tool calling, and integration with vector databases, so. 
 18:08: If we build custom organization, we write all of the logic ourselves, so managing prompt flow, tool executions, state error handling, and the integration. 
 18:19: So the advantage of language chain is like faster development and a standardized way of like building the AI workflow. 
 18:25: So the advantage of like custom orchestration is greater control, so lower dependency on the framework and potentially better performance like for specific use cases. 
 18:37: When you build an agent, right, there are certain sequence steps. 
 18:40: You first just the data set. 
 18:41: Then after that you do, chunking. 
 18:44: Then you do bedding. 
 18:46: Then you doveization. 
 18:49: You will do racks. 
 18:50: Everything is there, correct? 
 18:52: OK. 
 18:53: My thing is, OK, my one question is, how, see, after all you do, right, so now you go and you have an agent ready, OK. 
 19:01: You say that my name is, for example, my name is Mechan R. 
 19:06: You give it, OK, in the front, OK. 
 19:08: It gives my, details first what I read, yeah, 90 days how much that lives here, OK. 
 19:12: He is, qualified as this. 
 19:14: He works in here and all those things. 
 19:16: Second time I, type the same thing, right? 
 19:19: It gives me 90 days how much of that I don't. 
 19:22: Why did this happen? 
 19:24: Mhm, basically, like you like, basically what I'm saying, right, for is a current for right is so uncertain, OK, you don't get whatever it is. 
 19:37: So how do you streamline, to ensure that it perfectly matches 95%? 
 19:43: It can never be 100%. 
 19:45: It can be like, to my knowledge, OK, to have an open discussion. 
 19:49: So how do you do it's only 85% to 95%. 
 19:51: The first like I checked was the. 
 19:54: Like the retrieval step is returning the same document, documents both times and like in the rack system, like the answer is only as good as the retrieve retrieved context. 
 20:05: So if, if relevant chunks containing the date of birth was not retrieved during the second period, the like the model may respond that it does not know. 
 20:14: And second, The chunking strategy can be a factor. 
 20:19: If like important information is split across the chunks or the chunk of like, containing the date of the birth like has low similarity score, so retrieval may become inconsistent. 
 20:29: And third, the immediate, embedding, like the embedding quality or retrieval parameters may need tuning. 
 20:36: For example, the top key result returned during the results may have differ from the, first query. 
 20:43: And another possibility is like the prompt design. 
 20:45: Like if, if prompt instructs the model like to answer only for like retrieve contents and the date of birth is like not present in the retrieve document. 
 20:55: So the model like should correctly respond that it does not know. 
 21:03: OK, so there's always, like, we're all in health care, right? 
 21:06: There's a security concerns. 
 21:07: OK, if I do case number, it should not give my PIA information or PHI information to the board. 
 21:14: How do you control that? 
 21:17: for controlling that, like I usually do like pro like in healthcare environment, protecting, PLL or the PHI is critical. 
 21:26: Like I would not rely on the LLM alone like to protect sensitive data. 
 21:30: the, like the first layer is access control. 
 21:32: Like you should only be able to like, retrieve information they're like authorized to access using the authentication and rule-based authorization. 
 21:41: Second, like I would implement data masking or the redactions before the data reaches the model. 
 21:48: Sensitive fields, such as Social Security numbers, patient IDs, date of birth, address, or. 
 21:55: medical record numbers can be like masked or removed and also after that like I would apply the guard rails and the prompt restrictions so the Model is like instructed not to expose sensitive information and I would also implement the output filtering like to scan responses before returning them to the user. 
 22:16: So if PI or the PHI is detected, the response can be blocked, masked, or modified and finally, like all the access should be logged and the audit to the meet healthcare compliance requirements. 
 22:30: OK, sir. 
 22:33: OK, thank you. 
 22:35: the last question, you use the off, right, for the insurance, correct. 
 22:39: Abortion controls. 
 22:41: I'm sorry. 
 22:43: A Russian control. 
 22:46: Yeah, yeah, like, basically for the version control, like the concurrency control is like a mechanism used by the database like to ensure that the multiple users or transactions can access the same data simultaneously without causing data inconsistencies. 
 23:03: Like if, if two users try to update the same record at the same time, conferencing a role ensure that one of them does not accidentally override the other. 
 23:12: And databases achieved this using techniques such as like locking, transaction isolation levels, MVCC and the optimistic or like the pessimistic locking. 
 23:24: So the goal is like to maintain data integrity while still allowing high concurrency and the good performance. 
 23:32: Thank you. 
 23:33: Thank you for your time, sir. 
 23:34: I'm done. 
 23:34: Do you have any questions for me? 
 23:36: no, not yet, yeah. 
 23:38: Yeah I'm sorry to, yeah, go ahead and, could you please show your, photo ID please photo ID alone is also, they use a screen share was not good. 
 23:50: Yeah. 
 23:53: can you keep it closer to the screen with camera, yeah. 
 23:58: little book. 
 24:00: Oh yeah. 
 24:05: yeah, I did good. 
 24:08: OK, and can you check or something photos you are more chubby. 
 24:14: Like, now, currently I'm going to, like going for my weight, weight loss journeys of that so it's like a sick, like it takes, To Do you, do you have any other photo ID? 
 24:38: Maybe not just wait. 
 24:54: That when we Same for me. 
 25:01: I want to see you and select the image. 
 25:05: Could you keep like that? 
 25:08: Since it's a different support. 
 25:11: he's saying, don't hide your face. 
 25:13: show your face and as well as, the photo. 
 25:16: Sorry and which take us. 
 25:21: Now it's good. 
 25:23: little inside, can you keep it left side and the front, photo ID alone keep front. 
 25:29: No, no, yeah, but bring the photo ID, right, and as well as you, you come close to the camera. 
 25:38: No, no, no, no, 4 years ago. 
 25:43: Now your face is no keep left or right side of your yes like if photo alone bring it closer to the camera. 
 25:54: yeah, please hold, please hold. 
 25:56: So why there is a, not in, there are too much difference on the case. 
 26:00: That's why, basically it's like old photo, like it's a sexy ago that. 
 26:08: OK. 
 26:13: It could. 
 26:15: I don't have anything. 
 26:15: Thank you. 
 26:16: OK, yeah, thank you. 
 26:16: Thank you so much for. 
