0:00: HiRecruiter at Micro one. 
 0:01: Thank you. 
 0:03: for joining the interview. 
 0:04: How's your day going so far? 
 0:05: I explained. 
 0:14: Glad to hear that, Amrit. 
 0:18: Please introduce yourself. 
 0:19: Share a brief overview of your background, your key skills, and what you're currently focusing on. 
 0:24: Yeah, so basically I'm, I'm Paul Singh. 
 0:26: I have over 12 years of experience as a backend full tech engineer. 
 0:30: my expertise in like designing and developing the, S APIs, scalable backend systems, and the cloud native applications using Java, Springboard, Node GS, Python. 
 0:42: do, Kubernes and the school databases and my current role at AI version like, I work as a lead pattern developer and architect as well. 
 0:50: we're like, I build as a high performance microservices like for we can say pharmaceutical supply chain and inventory management systems and my responsibilities like include systems like. 
 1:01: developing the best APIs, integrating with the ERP and the third-party logistic providers, optimizing like application performance, and throughout my career, like I have focused on like building the scalable backend services, like, we can say improving the systems reliability, following the secure coding practices and, working in agile environments and like. 
 1:23: with the distributed teams and like now like we are looking for, I'm looking for like the back end engineing expertise while like supporting the AI model evaluations and the code review initiatives. 
 1:49: Thanks. 
 1:50: That's a solid mix of cloud tentative microservices and integration to heavy back-end work. 
 1:54: In Java slash Springboot, how do you typically implement timeouts, retreats, and circuit breaking for outbound HTTP calls, and where do you enforce those policies? 
 2:03: OK, like, basically, like in Springboot microservices, I generally use a Resilience 4J like library to implement the timeout circuit breakers like for we can say. 
 2:14: The external service call like timeout like I configure connections and the timeout on STTP client, such as web client or rest template like to ensure the request like don't wait identify and the timeout like don't wait like basically depends on the downstream services like SLAs. 
 2:34: And retries like for transient failures like the network glitches or the temporary 55 errors so I configure retries with the exponential back off and also like I avoid the retry client side errors such as like forex responses because like those usually retire the application changes we can say rather than be another attempt. 
 2:58: And talking to her like the circuit breaker, like I use circuit breaker to prevent the, we can say repeated calls to like unhealthy services and when the like failure threshold is exceeded the circuit. 
 3:11: Opens and requests the field fast or like return or like fallback responses and after like a configured wait period, it just transitions to like half open to test whether the downstream services has recovered. 
 3:25: And in last, fallback like for like non-critical operations, implement fallback method which are generally that, cache data default responses or like we can say user friendly and the error messages instead of like, failing the we can say entire request. 
 3:58: Good. 
 3:58: Breaker slash fallback is the right mental model, and your point about not retrying 4 XXs is important. 
 4:04: When you apply retreats with exponential backoff, how do you ensure The operation is safe to. 
 4:13: Try I dependency and prevent duplicate side effects across services. 
 4:19: generally for like duplicate things and like effect across corporation like get food and the delayed trial like, we can say generally see, because executing them like we can say like a multiple times result in the same state. 
 4:35: So like for post request that creator resources on like process orders like. 
 4:39: Generally, I avoid the blind trials instead of like we use ident potency keys or like unit request IDs so that like if the same request is received multiple times we downstream the services recognize this and it returns the previous result like instead of like creating the duplicate reports like for our signalers communication through like messages queues each event carries a unique message ID. 
 5:03: And consumers maintain procedure message IDs or like, or we can say use databases contents like to ensure that duplicate messages are like ignored, making the processing portent. 
 5:14: And, like when multiple microservices are involved, like our preferred human-driven patterns and we can see also a startup organizations instead of distributed transactions. 
 5:25: So each services like performs at local transactions and if a failure occurs like compensating the actions are like executed, rather than redrying operations, that could also create duplicate side effects. 
 5:38: So, retry only transient failures and retry only are important operations or like make them are important using identific keys and also use saga patterns like for distributed transactions like to maintain the consistencies or also we have the across this. 
 6:02: Makes sense. 
 6:08: Identityency keys request IDs plus deduplication on consumers is a practical approach. 
 6:14: And using saga slash compass, how would you handle database connection pool saturation and slow queries? 
 6:20: What metrics alerts do you watch and what changes do you make first? 
 6:25: for like the database connection, generally if I notice that take your time. 
 6:29: What metrics alerts would you watch first when you suspect connection pool saturation and slow queries in a he? 
 6:39: With Java service, hm, like if I notice data disconnection pool, saturation, like my first step is to identify the root cause, rather than to simply increase the pool size. 
 6:50: And also like I started my monitoring connections pool mattresses like, Hikari CP and the application monitoring tools like we can say, micrometer, Prometheus, or Grassa, and I checked the active, connections like ideally connections, connections with time, and the pool exhaustion. 
 7:07: And next, I review the application code to ensure the connections are like. 
 7:13: not being, held longer than necessary, and I make sure the transactions are short lived, database resources are like we can say, properly closed, and they are like no connection leaks, and then I analyze slow queries and optimize them like by adding appropriate indexes. 
 7:33: reducing the unnecessary joints and, avoiding N +1, query problem. 
 7:38: So faster queries raise, connections back to the pool more like quickly and, for the traffic scenarios like I use the database load by using caching with that, synchronous processing for like the non-critical task and paging issues, instead of like loading large data sets. 
 7:56: And after that, I also like configure sensible Hicari CP settings, such as like the maximum pool size, connections time out, ideally time out or the max lifetime based on the, database capacity and the application workload and simply like increasing the pool, size like it's not always the, right solution because the database itself has the connection limit. 
 8:18: And when the suspect connections pool like saturations, it's like it's like I follow we can say the structured approach like instead of making just assumptions so like I analyze the database using tools like slow query log, explain plans or the APM tools like to identify the slow run queries and optimize them, with the proper indexing for like the query factor. 
 8:54: That's a solid structured approach. 
 8:57: Especially focusing on leaks, long haul of transactions, and slow queries before tuning pool sizes. 
 9:03: When you see pool saturation, how do you determine whether the bottleneck is in the application? 
 9:09: Asian League slashing traffic spikes. 
 9:12: generally we can say for the application leaks or things like I determine it by correlating both application matrices and the database matrices. 
 9:22: Like, first, I check the connection pool mattresses like, if there are like some active connections ringing at the maximum pending request, like increasing, and then the connections acquisition time is like rising, it's confirmed pooling saturation, and then I determine the cost like. 
 9:39: If it is an application issues like I look for connection leaks, long running transactions, threads, blocked threads or code paths like where connections are not being, released properly, and also, like review recent deployments like to see if, any code changes reduce the problem. 
 9:58: And like also if it's the traffic is spike like I compare the timing with the request volume and if UPS or the transaction rate, we can say the suddenly increases. 
 10:09: So while the application and the database are like otherwise healthy and if it's likely a temporary load issues like that cause, I use auto scaling, rate limiting, or like, also sometimes I use load balancing to handle the increased traffic. 
 10:25: And if it's a database bottleneck, I check the CPU memory or disk input out good log conditions, slow query logs, and the execution plans. 
 10:34: So if queries are taking longer than expected, connection stays occupied and eventually exhausting the pool. 
 10:41: And after that, all, like, I also use monitoring tools like Prometheus, Graphpana, APM tools such as like Dinatrace or the new Relic tool like correlate the applications latencies and the database performance. 
 11:02: Good. 
 11:04: Correlating Simple metrics with request rate and DB health signals is exactly head operations, for example. 
 11:13: Payment or order create. 
 11:16: So retreats don't create duplicates. 
 11:31: Like for critical operations, like take your time, yeah, like for what specific mechanism response behavior to guarantee identitent cost for create to? 
 11:41: Mhm, yeah, like for critical operations like payment processing or we can say for critical operations, what fields or key would you use as the identitency key? 
 11:51: Where would you persist it, and what would your API return on a repeated request with the same key? 
 11:56: Yes, like for critical operations like payment processing or order creations, we never, rely on the res alone because that could create duplicate transactions. 
 12:07: So we make those operations ident important by using the unique identpotency key or request IDs that travels with the request across the services and if the same request is received, again, like due to the data or the time of. 
 12:22: The downstream like services checks like whether it has the already processed that request and if it has, it simply returns the like existing results instead of like executing the operations again and in distributed workflows like we also use saga pattern each services like performance local transactions independently and if one step fails, we execute compensating transactions through. 
 12:48: Roll back the previous successful steps like rather than relying on this single distributor system and to guarantee potencies like for create order, I generate or like accept a unique ident potency key for like every order creation request and before the creating the order, the services checks like whether that key already exists in the database or in potency store. 
 13:12: And if the key is like, new, we process the request, create the order, store the potency key along with the order ID and return the response and if the same request comes again because like a retry, time out or we can say a network issue, so we, don't create another order. 
 13:34: Instead of like we, look up the existing item potency and return the previously, created order and response. 
 13:51: That makes sense. 
 13:52: Ari. 
 13:53: Returning the previously stored result for the same identitency key is exactly what prevents duplicates across retreats and timeouts. 
 14:00: How would you unitotist an identitent create order endpoint to prove it never creates two orders under concurrent identical requests? 
 14:07: OK. 
 14:09: tell me for that. 
 14:12: we are like just, for like identical request or things. 
 14:15: I would write both the you can say the unit test and the concurrency integration test. 
 14:20: generally for the unit test, I would mark the, repository and at emergency store. 
 14:26: I would call the create order or order method twice like. 
 14:30: with the same potency keys and verify that the order is like created only once or, or the repository safe method is like in invoked only once, and the second call, returns the existing order instead of like creating a new one and like for concurrency test, I would use an executive service like with multiple threads. 
 14:51: For example, like we can say 10 to 20 threads all sending the same request, with the same item button. 
 14:58: At the same time, so after all threads complete, I would like to verify just like only one order exists in the database or also. 
 15:07: All requests receives the the same order ID in the response and the repository contains exactly one record like for an item potency keys. 
 15:16: So to make this reliable, the item potency key should have a like unique database contents and the service should like execute the check and save operations like within the transactions. 
 15:27: So these pres these conditions were to verifying save called once and adding underrate. 
 15:37: Yes Not just service lodge. 
 15:40: Yeah, absolutely. 
 15:42: Like, in your integration test, how would you make the database enforce identitency, for example, see. 
 15:50: Like, absolutely. 
 15:50: Like, besides verifying that the save is called only once, I would include a concurrent integration test like 2. 
 15:58: Do you walk me through the exact database to level mechanism you'd use unique index slash constraint transaction by ONT. 
 16:07: O C O N F L I C T, etc. 
 16:10: and the specific assertions you'd make in the Integration test under concurrent requests. 
 16:17: Yeah, like I would use an executive service like with multiple threats, synchronize them with the, we can say. 
 16:25: Even like them with a countdown ledge and have all the threads invoked the create order endpoint simultaneously using the same ID keys and after all requests like complete, I would verify only one order exists in the database and all responses return the same order ID and only one item potency record is created and no duplicate reports are like inserted even like under the content load. 
 16:51: And to enforce the uniqueness in the database, I would like to create a unique contents on the itemergency key and column all like on the appropriate business keys such as like customer ID order request ID, and during the integration test, all the content requests use the same potency keys and if two requests reach the database simultaneously. 
 17:16: The data is guaranteed that only one insert succeeds, and if another request attempts to like insert the same key, like it receives like duplicate key exceptions or like data integrity violation exceptions and in the service layer like I catch that exceptions retrieve the existing order using the itempotency key and return the previously created order like instead of like failing or creating a duplicate. 
 17:44: And at the database level like I would enforce the regency key using the unique index or the unique contents on the regency keys or like we can save appropriate business keys like in post way as well like we use all like insert on like conflict do nothing or like on on conflict do update to handle the duplicate request peacefully. 
 18:10: So like the order creates we can say logical, would like run inside the transaction. 
 18:14: So either the redraw operation succeeds once it's like, rolled back completely and And last, like for the content integration test, I would use an like, executive service and the countdown latch like to send, the multiple, identical requests simultaneously with the same item keys. 
 18:46: Constraint is a solid way to validate identity and race handling. 
 18:50: Mhm. 
 18:52: Amri, when that duplicate Toki violation happens under load, how do you ensure the client gets the exact same response consistently, including status code and body without leaking internal error details? 
 19:04: OK, got it. 
 19:05: Like, for like body without leaking internals, like when a duplicate token or item potency keys, violation occurs, I don't expose, like the database exceptions to the client. 
 19:17: Like instead, like I catch exceptions such as like duplicate key exceptions or like data integrity violation exceptions in the same service layer. 
 19:26: So like I then use the same identity keys like to. 
 19:31: Generally derive the already created order from the database and return that existing results like from the like client's perspective like the data receives exactly the same responses as the original successful request so. 
 19:49: The same STTP status for like, typically, 201 created. 
 19:54: So if the original request created the order successfully and the same response body like, including the same order ID, timestamp and the business data and the same item potentity in the response like headers like if applicable and internally I log the duplicate request, with the request ID and the correlations ID, like for monitoring and debugging, but the client server like. 
 20:18: never sees the database errors, track, or internal implementation details. 
 20:32: Good. 
 20:34: Mapping the constraint failure to a deterministic fetch existing and return path keeps responses stable and avoids exposing internals. 
 20:41: How do you prevent a race where the second request catches the duplicate Toki error, but the fetch existing order, query can't find it yet due to transaction isolation or replication lag. 
 20:50: OK, generally see, like, basically, to avoid that the these conditions, I don't rely on the catching the duplicate key, exceptions. 
 21:00: the preferred approach is to store the item potency key and the response, automatically, with the same transactions as the order creation. 
 21:09: So please ensures that once the trans transactions commits, both the order like item potency records are like available together. 
 21:16: And if the second request gets the duplicate key, exceptions before the first transaction has committed, and I, I, I treat it as a transient condition, and instead of like, we can say immediately returning an error, our performance, shorter than exponential back off like to fetch the existing order, since the first transactions typically commits with a few milliseconds or the try usually succeeds. 
 21:49: That makes sense. 
 21:51: Impotency keys plus transactional rights generally beat exception to driven control flow, and retreats can smooth out short commit races. 
 21:59: How do you enforce identitency when the client? 
 22:02: Trees with the same key. 
 22:05: But a different request payload, for example, different items or amount. 
 22:09: generally, when a client retries the same item ertency key, the first step is to check the urgency store, like, before executing the business logic, and like if a key already exists, like I immediately return the previously stored response, during the same aesthetic status code, response body or, the order ID, and without reading the new order or like invoking the downstream services again, if the key, does not exist. 
 22:37: generally I start a transactions, create the order process like both the order and the potency report automatically, and also like store the response against that key and then the commit the transaction. 
 22:51: So these guarantees that the potency records and the business data remains consistent and to handle the concurrent request and enforce a unique conference on the potency keys. 
 23:02: Like if like two requests within the same key arrive like simultaneously. 
 23:07: With only like one transaction succeed, so the second request, detects that the key already exists. 
 23:14: So it's catches the store's response and returns the exact same result like instead of like creating the another order. 
 23:28: Good. 
 23:29: Returning the previously stored response and treating the identity record as the source of truth is the right shape, and the unique constraint covers concurrent submissions. 
 23:38: When you code to review an implementation like this, what failure modes do you look for around transaction boundaries? 
 23:45: Especially the cre. 
 23:47: Identityency records versus create order via store response ordering. 
 23:53: basically, when I review an implementation like this, no problem, take a moment. 
 23:58: In your view, should the identity record be inserted before the order is created or after and why? 
 24:05: like, as I told you earlier, like, when I review an implementation like this, I focus on transactions boundaries like before because like most of my, an emergency bugs happen there. 
 24:16: So first, like I verify that these two locations and emergency records are like, written in the same details transaction. 
 24:23: So I don't want a situation like whether the order is committed, but the item potency record fails or like vice versa. 
 24:30: And second, like. 
 24:31: I checked the external API calls such as as the payment gateways or the notification services are like not executed inside the long running retail transactions and externally like external call like. 
 24:44: Should happen after the transactions come in so like we handle our synchronously using the patterns like our work patterns and after that part like I verify the transaction isolation level like. 
 24:56: That ensures there are like no risk conditions like we are two concurrent requests can both pass the existing check before like one commits and after that I make sure, make sure the rollback behavior like it's correct. 
 25:09: Like if any part of the transaction fails like neither the order like or nor the item policy required like should be persisted and also I, I ensure that the duplicate key exceptions are like. 
 25:21: Handle the gracefully like by fetching and returning the existing response instead of like exposing internal database errors. 
 25:40: That's a solid review checklist. 
 25:42: Atomicity. 
 25:44: Avoiding external calls inside the transaction and verifying isolation slash rollback are exactly where subtle identitency bugs hide. 
 25:52: How would you design the identitency storage so you can safely return a response even if the process crashes into a transaction or right after commit? 
 25:59: What states fields would you store and how would you handle into Progress key? 
 26:03: Yes. 
 26:05: Mhm. 
 26:05: And like to handle crisis, safely, basically I designed the emergency store or like the source of growth, and like process it automatically, basically with the business, transaction, like when a request, comes in, like I created, I emergency records like with the status like in progress. 
 26:28: And within the same transactions that creates the the order and once the order is like successfully committed, I update the emergency records to the, to complete it and store the response like metadata such as like we can say the order ID STTP status code and the response body like or a reference to it. 
 26:47: And like if the process crashes before the transactions commit, so the transactions roll back completely, so like neither the order or nor the potency record exists, so the client like can safely retry and if the process crashes immediately after the comment, like, both the order and the potency records are like already processed. 
 27:12: And when the client retries with the same itemruency keys, the services like simply like reads the completed report and return the exact same response like without creating another order. 
 27:36: A back-end service passes all unit and integration tests, but a small percentage of production requests return inconsistent results under load. 
 27:45: How would you determine whether the root cause is a race condition, nondeterminism, or a testing gap? 
 27:52: like, for like the testing app, if the issue appears only in the production under, under the road, generally I would take a, systematic approach like to isolate whether it's the these conditions or not determine, not deterministic or like a testing gap. 
 28:10: So generally, first like I would collect production evidence by the correlating request IDs, correlation IDs, or logs, traces, and then my I just like to. 
 28:20: Identify like when and where where the inconsistency occurs and I'd also like to compare successful and the field request to like look for the common patterns and next like I would try to reproduce the issues in a staging environment using the load testing tools like a jay meter or the gateline and with the production like the traffic on concurrencies, if the issue appears only under the, concurrent load, like it's strongly indicates these conditions and to like identify the risk conditions, I would look for the shared mutable state like missing the synchronizations, transaction boundary, issues or like, cache inconsistencies or like the content updates like the. 
 29:08: Same idea, like, but, I had also, reviewed the looking or the optimistic or the pessimistic locking and the database isolation levels and to identifying the non-deterministic ID check like for the code, that depends on the timing like thread scheduling, unordered collections, asking processing random values or like eventually consistencies between the services. 
 29:42: Thank you, A developer says, we're safe from sequel injection. 
 29:48: Then because we. 
 29:50: Escape all user or why not? 
 29:53: Mhm. 
 29:59: basically, we see when the Scal injections are like happen. 
 30:02: I will not, like the recommended approach is, do you want me to repeat the last question, or can I continue? 
 30:08: No, no, you are continue. 
 30:10: the recommended approach is like to use the, parameterized queries or the, prepared statements and, when user inputs is passed as the parameter rather than the, concatenated into the as well sing. 
 30:24: frameworks like the spring, spring data, JPA Hibernator, the JDBCs. 
 30:30: Prepare the statement automatically or separate the escal code from the user data, like which is like much safer. 
 30:36: And in addition to parameterized query, I also like generally follow this like use input validation to. 
 30:44: and ensure the data matches the expected format and avoid building dynamic as well by, by con coordinating user inputs and apply the principle of the least privilege so the data, like database users like only the permissions that it's needed and use ORM frameworks like Hibernate or JP like whenever it's possible. 
 31:16: Understood. 
 31:17: Let's. 
 31:19: Proceed with the next steps. 
 31:21: Please say say an interview to save till now. 
 31:37: See interview Congrats, you just finished the verbal questions. 
 31:52: Now the last step is a 30 minute exercise. 
 31:58: Got it. 
 32:06: Hm. 
 44:57: Hm. 
 47:52: I I 
