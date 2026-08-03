0:01: Hello. 
 0:04: Good morning. 
 0:06: Mhm. 
 0:10: Am I audible, right? 
 0:12: Oh yeah, yeah, both of you are audible. 
 0:14: Yeah, can we start? 
 0:16: Oh yeah, sure. 
 0:18: OK, so just start the recording, yeah. 
 0:21: So I have gone through your resume. 
 0:24: So can you tell me how much you rate yourself in Python out of 5? 
 0:27: at least 4.5. 
 0:30: Minimum. 
 0:31: OK. 
 0:32: OK. 
 0:33: And you almost have 122, 12% inspection in Python. 
 0:38: OK. 
 0:41: Can you explain me these different design patterns or different design patterns? 
 0:46: Yes, yeah, see, like the talking about and mainly work with the practical design patterns are like commonly used in the backend applications, like, one pattern is I use frequently in the, the repository pattern with SQL alchemy. 
 1:00: instead of like writing the database queries, directly inside the AP endpoints, I keep the data access logic, in a separate, repository layer. 
 1:09: So this makes the code like, basically the cleaner, easier to test, and like easier to maintain and Apart from that, like, I use the singleton, factory patterns, strategy patterns, repository patterns. 
 1:25: dependency injections are like used, like, injects the dependencies basically instead of like creating them, inside the class fast GPI depends, method is like a good example. 
 1:37: Like I use it for the services or database sessions. 
 1:41: authentication and also the observer pattern, decorator pattern, like decorator pattern basically adds functionalities like without modifying the original code in Python, and decorators are like commonly used for logging authentication, validation, and the middleware. 
 1:59: OK, what is the major. 
 2:05: What is method resolution order MRO? 
 2:07: Oh, MRO, basically, like what MRO does, like it's an order like which Python search for like methods or we can say attributes, when it's called, especially like in multiple inheritance like instead of like searching. 
 2:23: Parent classes randomly Python, like we can say follow the well-defined order using the C3 linearization algorithm. 
 2:32: So this ensures that we can say each class is visited like only once the inheritance hierarchy remains consistent. 
 2:44: OK. 
 2:46: would it depend on the injection in the first EPA? 
 2:48: like, In fast API, DI is like a way to provide the objects or like we can say service that an endpoint needs instead of like creating them inside the endpoints. 
 3:02: So this keeps the code like modular reusable and easier to test and fast APIDI. 
 3:08: Implemented using the depends function, like for example, instead of like creating the database session, like inside every API, I define the dependencies that provide the database sessions also and the fast DP automatically injects it into the endpoints. 
 3:26: OK. 
 3:29: you weren't fasting period. 
 3:32: So what is pedantic models? 
 3:34: see, like in fast API, basically, we use Bantic like we can say it's a Python classes like used to the structure of the request and response data. 
 3:44: They automatically, validate incoming data and post data like types and return the clear validation of errors like if the input is invalid, for example, if, like if an API expects a patient's name, age, and the email. 
 4:00: I define a pandemic model with those fields like when a client sends the request fast we evaluates the data against that model before the request reaches my logic, my business logic. 
 4:17: OK. 
 4:17: And what HTTP policy returns in case of failures? 
 4:22: generally we can say, like for a successful request, like, we can say I usually return the request, requested data along with the 200 OK or 2201, created if a new resource is created. 
 4:37: if there is a client side issue such as an invalid input like I return the 400 bad request or 422 unprocessible entity like which fast TP handles like automatically through the identic validation and if the requested resource does not exist. 
 4:56: I returned a 404 not found like for unexpected server side issues and also I return the 500 internal server error after logging the like exception. 
 5:09: OK. 
 5:11: Do you know N+1 query problem, yeah. 
 5:14: And extent and how you will fix that issue in general. 
 5:19: Yeah, basically the N+1 query problem is like, common performance issues in the ORMs like SQ alchemy or the Django RM. 
 5:27: Like, we can say it occurs when the application executes, one query. 
 5:32: Like we can say to fetch the parent reports and then like. 
 5:36: Executes an additional query for like each parent record to fetch related data. 
 5:41: For example, if we fetch 100 users and then access each user's order separately, so the application executes 1 query to get the users and 100 more queries to get the orders. 
 5:54: So, resulting in 101 queries, this is called the M+1 query problem and can significantly impact the performance and To avoid it, we use eagle loading instead of lazy loading. 
 6:09: In escal alchemy, we can use the joint load or the selecting a load to fetch the related data in advance and reducing the number of of like the database queries. 
 6:22: OK And in Django, how what are the different functionality we use to fix this, which function do we use in Django basically typically we use select related and the pre prefetch related to all the plus one queries and basically select related is used for like the foreign key and, like, 1 to 1 relationship. 
 6:46: it performs, like sque join and fetch the related objects in a single query and Prefetch is used to like many to many and reverse foreign key relationship like it executes separate queries and combines the result like efficiently in Python. 
 7:04: OK. 
 7:05: So I, give me one question here in the chat. 
 7:08: Can you open the chat? 
 7:09: Yeah, sure. 
 7:22: Yeah. 
 7:23: Can you please tell me the output for this? 
 7:25: Mhm. 
 7:26: Just give me a second. 
 7:37: Basically, He goes to sight like the. 
 7:43: The fastest is the set of like the braces, a set. 
 7:49: And Of. 
 7:53: Like both sets and dictionaries use hash tables, so Python can directly locate the element using its hash value and giving an average of one like lookup time. 
 8:03: So a list of stores element sequentially. 
 8:07: So Python has to like scan each element until it finds a match like which takes off in time. 
 8:14: OK. 
 8:17: How do you handle the circular dependencies? 
 8:20: for like, generally circular dependencies happens when two modules or like classes depends on each of them, like either directly or indirectly. 
 8:29: So these can lead to import errors or like make the code difficult to maintain, so. 
 8:36: The first thing I do is like check whether the design can improve or if two modules like depend on each other. 
 8:43: I try to separate the shared logic into the third module. 
 8:47: That like basically both can use, so these usually remove the circular dependencies and make the code cleaner. 
 8:55: And if it's only an import issue, like I sometimes move the import inside the functional method like where it's actually needed. 
 9:03: So this delays the import until runtime and avoids the circular import during the application setup and in larger application. 
 9:14: I also keep a cleaner separation between layer. 
 9:16: Like, for example, API service and the data access layer. 
 9:20: So this helps prevent the support dependencies like from, like happening in the first place. 
 9:26: OK. 
 9:28: can you please explain to me a sync of it in first DP? 
 9:31: Can you give me one example for this, a sync of your application? 
 9:34: Mhm. 
 9:35: like, see, like synchronous is basically like, determines how requests are like, both like synchronous and asynchronous, like how like requests are handled. 
 9:45: So a synchronous functions execute one task like at a time. 
 9:49: So if it's API is waiting for the database query or like the external API response, that request remains blocked until the operation completes and asynchronous function uses RSync and allowing the server to handle the other requests while waiting for like input output operations like the database calls, like files, uploads and the external API responses. 
 10:13: So these improves like throughout and makes the application more scalable. 
 10:19: And in my project, like I use our sync and it like by calling the external rest APIs, query database as synchronously, and, we can say and reading files since these are like input output bound operations, asynchronous programming reduce the, we can say reduce times and improve the through throughput when many users can access the API simultaneously. 
 10:44: OK. 
 10:47: OK. 
 10:49: can you explain me the microservice architecture? 
 10:53: There are two types of architecture like the generally the monolithic and the microservice microservices. 
 10:59: Microservices is like a design approach like where an application is divided into the small independent services. 
 11:06: It's like each service responsible for a specific business capability. 
 11:10: Each microservice can be developed, deployed, and scaled independently, and the service like communicate with each other through the through APIs and, like, in my project, like we build the platform like using the multiple fast GPI microservices, for example, like, one service like handle the data injections from like the CSV, Excel, and the FHIR sources, and, another like manage the patient and the provider data, and another handle the AI inference and the analytics, and each service had its own business logic and communicated with like other services, other services like through the APIs. 
 11:52: OK. 
 11:54: So, one of my first DP, it's a gate API, is, very slow in production. 
 12:00: So how to find out the root cause for the APIs of this. 
 12:04: generally in these types of situations, we are like if like an API is slow, like becomes slow in production, I would troubleshoot it like step by step, like generally instead of assuming the root cause, like first I check the application logs and monitoring dashboards like to identify like where the response time is increasing. 
 12:25: And next I had like determined whether the delay is in the API code like the database or in like the external services. 
 12:32: So if it's like we can say database issue, I'll review the SQL queries, check the execution plans, look for like the missing indexes, and verify like whether there is an end +1 query problem or any long long running queries. 
 12:47: And if the database is healthy, I check whether the API is like making slow external API calls or processing large files as synchronously. 
 12:57: And apart from that, I also reviewed the CPU, memory and the container utilizations like to see if the services like resource content. 
 13:09: OK, do you know a circuit breaker? 
 13:11: What is circuit breaker, talking to her like the cir circuit breaker. 
 13:15: Circuit breaker is like a design pattern like using the microsurfaces like. 
 13:19: generally to prevent repeated calls, to a service that is already failing and instead of like continuously sending requests to an unhealthy service, so the circuit breaker temporarily stopped those requests and allowing the failing service times, like to recover and preventing failures like from cascading to the other services. 
 13:42: Like, it has 3 states like closed, open, or half open, like closed is basically. 
 13:48: Requests are allowed to pass normally and like open is like after a certain number of failures requests are like blocked and the service fails passed and half open like after a timeout like a few requests are allowed through the check like whether the service has recovered and if they succeed, the circuit closes and otherwise like it opens again. 
 14:11: OK. 
 14:14: Can you explain me Kafka how Kafka works? 
 14:17: Kafka generally we use for like the distributed event streaming platform like used to generally exchange data between the applications like in a reliable way like instead of like one service calling another another directly or like a services publishes a message to a Kafka topic and like other service consumes those messages independently. 
 14:40: Like the main components basically are like producer which like send message to a Ker topic. 
 14:45: The topic like a logical channel where the messages are like stored and we have consumer like reads messages from the topic and then lastly we have the broker like Kafka server that is told that the manager manages the messages. 
 15:04: OK. 
 15:05: Can you go to the chart again? 
 15:07: can you please tell me in this block of code what are the different issues you see? 
 15:36: basically. 
 15:39: I see A Few issues in this implementation, OK, like, first, like, using the psychop G2 like inside the as sync endpoint. 
 15:50: So, Psychopy 2 is like a synchronous database driver, and since the endpoint is declared as as sync, these database like calls block or block the event loop. 
 16:00: And either the endpoint should be synchronous de like function or like async driver such as the asking asking PG. 
 16:09: So the Scalomy asking should be used and there is no exception handling like if the database connection fails or like a query throws an exception, the API will return the 500 error and also no no handling for like the missing records like the. 
 16:26: fetch, fetch one, returns none, then the dick row will raise an exception and I will check if the row is none and return like 44,040 and the database connection management like. 
 16:38: It appears to use a global connection in production. 
 16:41: I would use a connection pooling so we can say or dependency injections to manage the database session safely and the direct as well, the queries parameterized like, which is good help, which is good because it helps to prevent SL injection. 
 16:59: OK. 
 17:01: can you share your entire screen and, open any ID or maybe I can complain. 
 17:13: It's visible to you? 
 17:16: Just. 
 17:18: Yeah, yes. 
 17:48: Yeah. 
 17:50: Yeah, in the chat I have given you the problem statement. 
 17:53: Can you please write Python code for this and try to write the PI test as well, OK. 
 18:03: To design a common generator similar to the one. 
 18:18: Also write up, ma'am. 
 18:21: Yeah, yes, yeah. 
 19:44: Mhm Basically, I define a function that's similar to the Python builds in range, and it accepts the start to stop and, step like with step defaulting to one. 
 21:21: OK. 
 23:50: Yeah, like, here, like, I told you earlier, like, I define a function like it's one of the Python built-in range, like it accept the start stop and the step like with the step defaulting to the one, OK. 
 24:03: And like basically if a stopper like basically this handles the case where like only one argument is passed and then a stop equals to start and start equals to 0. 
 24:15: like if only one argument is given to treat it as like the stop value and set it start to zero, matching Python's range behavior. 
 24:26: And if the steps is equal to 0, like it validates the step value because the step of like 0 would cause an infinite loop and after that I raise a value error like just like a Python building game. 
 24:45: And after that I handle the case we are like we are moving in in the forward direction and then after like I continue the looping like until the current value like reaches the stock stock values and yield start like yield returns. 
 25:03: one value like at a time instead of like creating the entire list in the memory. 
 25:08: So this makes it like a generator and keeps memory like usage flow. 
 25:13: And like after yielding the current value, I increment it by the step. 
 25:19: So generally like these blocks that handle negative step values and like when the step is negative, I keep looping while the current value is greater than the stock value, and again I return one value at a time like using yield and since the step is negative, like adding and decreases the value like until the loop ends. 
 25:41: Overall, like, this implementation behaves like a Python building, like since it uses a generator, this generally the space complexity is like OF1 and because it stores only like one value at a time and the time complexity of the OF and like where anything like number of values generated. 
 26:03: Can you give two outputs here, first one is, 10-1. 
 26:13: OK. 
 26:15: 10-2. 
 26:21: And second one will be, first you exhibit this one, and then next one in the book just give the 0. 
 26:29: Just because you don't know, only one other, OK. 
 26:41: So there are 10, 0, and minus 1 this gives the output from 10 to 1, like decreasing and the second. 
 26:49: 3, start equals to the 10, stop equals to 0 and is minus 1. 
 26:53: So the generator yields value like, while like start is greater than to the top. 
 26:58: So after yielding each value start is like, decremented by 1 until it reaches 1. 
 27:04: So the next value would be 0, but the loop stops, because the start is, greater than stop. 
 27:10: It's like no longer. 
 27:13: Mhm. 
 27:15: OK. 
 27:22: Can you write my test for this? 
 27:23: Yeah, sure. 
 27:25: Right to write a. 
 33:43: Yeah, generally these test cases like, cover the main scenarios like normal positive range, single argument is a negative step on the edge, edge case like, where the range is like empty and, invalid input like where the step is you and together they validate both the expected functionality and error handling of the generator. 
 34:04: And you this So Nothing shows. 
 34:39: Like, basically it's an online company so. 
 34:44: I'll be imported. 
 34:47: It's OK. 
 34:49: I. 
 34:50: Generally asserts here is success is nothing, no problem. 
 34:57: If you do not equal to, then it will throw an error. 
 35:00: yeah. 
 35:04: And OK, so do you have any experience in, non-relational database as well as relational database, like in Mongo TV I have like generally I've used, Mongo TV post as well. 
 35:19: these two are like most, mostly these two. 
 35:24: OK. 
 35:25: So can you tell me what is clustered index and non-clustered index? 
 35:33: Like clustered is like a determines the physical order, like in which the data is. 
 35:40: Stored in the table and. 
 35:44: Since like the data can be like only be stored in the one or like Physical order like we can say like a table. 
 35:54: Can be like I have only one cluster index and. 
 35:57: It typically created on the primary key because like records can be retrieved very efficiently based on that column, and a non-cluster index is like a separate structure that stores the index column along with a pointer to the actual data row, and it does not change like how the data is like physically stored. 
 36:22: And like a table can have like the multiple non-clustered indexes. 
 36:29: Mhm. 
 36:30: OK. 
 36:31: How to create index in Mogadivi? 
 36:33: Oh, oh, when, Talking about like Mongo DB like. 
 36:39: We can see if like if users have like users collections and I frequently search by email like I can create like we can say ascending indexes like dB. 
 36:50: users create index. 
 36:52: Then like here one means like ascending order and minus 1 means like the descending order and like for a compound index like if the queries are often filtered by both like last name and the city name I can create like the DB users create index last name and Mongati also supports like the unique indexes like after creating indexes I would like to verify whether the queries like actually using them in the explaining. 
 37:20: OK. 
 37:22: Do you know how query gets executed in the background? 
 37:25: Oh, I see. 
 37:26: I mean query execution order. 
 37:28: Mhm. 
 37:28: Yeah, like when a qui query is executed, the database like goes through several steps like before returning the results, and first, like the query is passed, where the database checks the syntax and the validates and the, reference tables and the column exists and, next, the query optimizes, analyses like the different execution plans and chooses like the most efficient one like based on, factors like available index, table statistics, and, estimated cost and, then like the execution engine runs the selected plan and if the suitable indexes are like available and like indexes scanned otherwise like it performs a full table scanning it also. 
 38:16: handles like joints, filtering, sorting, and aggregation as like required by the query. 
 38:23: OK. 
 38:30: Is it possible to send the query parameters in the post method? 
 38:36: I think yes, like a post request can have like a query parameters as well as like the request body. 
 38:43: although like post is mainly used to send the data in the request body and the query parameters are like often used for like for optional information like filters, versioning or flags. 
 38:58: OK. 
 39:02: OK, so what is the difference between horizontal and vertical scaling? 
 39:07: basically, these tools, like, we can say are two ways of handle like increased application load. 
 39:13: Like vertical means like increasing the resources of the existing server, like, such as like adding more CPU memory or storage. 
 39:22: It's simple to implement, but there's like hardware limit like to. 
 39:27: How much a single machine can be upgraded and the other hand, horizontal scaling means adding more application instances of servers and like distributing traffic across them using a load balancer. 
 39:41: So this improves availability, fault tolerance we can say and allows the application to handle like much like higher traffic. 
 39:53: OK. 
 39:58: Just a minute somebody's being. 
 40:12: OK. 
 40:12: So what are the top security vulnerabilities that we need to consider while designing any of the FTP application? 
 40:21: generally when I'm designing a positive application, I focus on like some like. 
 40:27: security areas like authentication and authorization like secure, APIs using or to delivery tokens and like ensure users can access only the resources like they are like authorized to use and we have the input validation use like the identic models to validate the request data and like reject the invalid or the malicious input and the escal injections like. 
 40:53: avoid dynamic as well like use parameterized queries or SQL alchemy or to like prevent the SQL injection attacks and STTPs and encryptions like, ensure all the communication. 
 41:08: It's like over STTPS so the data is encrypted in transit and then we have the secret manage management like never hardcore pass passwords or the API keys and rate limiting course configurations. 
 41:22: These are the things. 
 41:26: OK. 
 41:31: OK, so, OK. 
 41:38: So that's it from me, sir. 
 41:39: do you have any questions? 
 41:41: yeah, like, apart from this round, how many rounds are in, coming for this future for this room? 
 41:47: I'm not sure. 
 41:47: I need to check with HR only. 
 41:49: Maybe they will. 
 41:52: A for that, I'm not sure on that. 
 41:56: OK. 
 41:58: Sure, thank you, thank you for your time. 
 42:05: I 
