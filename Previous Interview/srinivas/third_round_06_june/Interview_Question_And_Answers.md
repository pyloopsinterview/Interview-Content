0:01: Tell me if you're speaking you're on mute. 
 0:06: Hey, hi, hi David hi girl. 
 0:09: I, I wait. 
 0:14: Are we expecting Jayden also reaching or you want to continue do not know. 
 0:19: I know I haven't got any. 
 0:23: I haven't got any acceptance from Jaden. 
 0:25: So if you guys are good to start. 
 0:27: I want to give a couple of minutes to get whatever they do. 
 0:32: I, I don't know if he's coming. 
 0:34: I have no idea. 
 0:37: To live we can continue if you want to return to his jail. 
 0:41: Oh And the same, yeah, yeah, totally subjective for it so I'll drop off you guys can continue with the evaluation questioning thank you yeah. 
 0:57: Really, you drink that. 
 1:04: OK, yeah. 
 1:06: So, we'll get started with, We'll do, what was that? 
 1:17: Yeah, so we'll do like an intro, some conversation, we'll do some technical Q&A, we'll do. 
 1:27: coding exercise and then time for questions at the end. 
 1:33: so yeah, I'll, I'll start. 
 1:35: My name is David Stroka. 
 1:36: I've been at National Grid now for a little over a year. 
 1:42: I've worked a few places before this, I worked at the Center of Advanced Computing at Cornell University before this. 
 1:53: Cornell University. 
 1:54: My son is at Cornell University right now. 
 1:56: He is, yeah, he is. 
 1:58: That's pretty cool. 
 2:02: Yeah, I lived out right down the road from it. 
 2:04: There you go. 
 2:05: I just came back. 
 2:06: I just came back from school, so go and pick up everything. 
 2:09: Come on. 
 2:10: That's funny. 
 2:12: yeah, so you're right next to me, yeah, yeah, yeah. 
 2:17: Oh my God, that's a good like 6 to 7 hours drive, yeah, like they could be all, yeah, they could be all when the summer break starts. 
 2:26: Yeah, and I work on the ODB project and the NSC project at National Grid as the technical lead. 
 2:35: OK. 
 2:36: I Yeah, hey, so my name is Li Xun. 
 2:41: I'm a staff product engineer in National Grid. 
 2:43: I joined National Grid for like, I think 2.5 years already. 
 2:47: Yeah, I work in another product different from Davis. 
 2:51: my product is called like, short-term low forecasting machine learning platform, yeah. 
 2:56: So do the like a low forecasting, electrical low forecasting, and the generation forecasting, yeah, for the electrical assets. 
 3:05: OK, so let me start with my introduction. 
 3:07: So, hi, my name is Srinuma. 
 3:08: I have around, you know, about 12 years experience in backend application and API data platform. 
 3:14: I'm on the Python site. 
 3:15: Currently I am working on a tenant health where I double backend service and data integration platform that basically support healthcare operations and analytic reporting system. 
 3:25: On the key projects side, I'm involved in building Python and fast database platform and process large volume of operation and patient analytic data that coming from the multiple healthcare system. 
 3:36: I developed that API back in back in microservices, and event driven workflow using CAP and RINQ. 
 3:44: We use Post SQL for transactional and reporting workload and Docker for Country and Azure for, you know, deployment. 
 3:53: Apart from my development, deployment side, development side, I involve architecture, performance optimization, code reviews, monitoring, engineering, collaborative with the business teams, and convert requirement into the scalable technical solution. 
 4:07: And yeah, that's all pretty much, pretty much what, yeah. 
 4:13: My question is like, how you develop the rest APs, why do you choose like a class API? 
 4:17: Why, why don't you just go with the A AS development core. 
 4:21: can you come again? 
 4:23: When you develop the API API layer. 
 4:26: Why did you choose the fast API? 
 4:30: You said like the data core. 
 4:32: Yeah, actually, B core is more, not more native, right? 
 4:35: And they will, I don't know about the ODP. 
 4:37: Probably like the API layer is also developed, will be developed by the DA core, right, not, not from Python. 
 4:43: So right now all of our ODB is Python. 
 4:47: Oh, I'm at home. 
 4:48: I see, yeah, and, yeah, the point of ODB right now is, you know, needing deliverables and getting, getting on the, getting the, what's a good word for it. 
 5:04: Yeah, not that you just proof of concept, but get like a solidified application in place and then growing it from there. 
 5:11: Yeah, I see that's the word for that. 
 5:13: I don't remember. 
 5:14: Yeah, yeah, thanks, but, yeah, actually I think I probably have to switch to like a cool, yeah, what I and the point, yeah, the point is because it's such a modular. 
 5:27: The point is to make it so modular that each part of it can be replaced with something else. 
 5:32: So like if I know that as of right now it is all Python, but the, the roadmap is to eventually have pieces in.net core have pieces of pieces and whatever. 
 5:44: Exactly, exactly. 
 5:47: OK, so let me answer my actually answer your question, why I choose fast AP because it's basically provides a lot of functionality out of box, which is basically help us to develop APD faster and less volatile code. 
 6:01: For example, fast API automatically handle the request validation, data silization, API documentation through the swagon or OpenAI. 
 6:09: And also the tight checking because these are, you know, these are things that I would, I would, you know, otherwise I, I have to build and maintain myself. 
 6:19: If I were in not creating everything from scratch, and another advan advantage is maintainability using well established framework. 
 6:27: It means the code is more structured and easier for other developers to understand and following a common indu industry standard. 
 6:36: And fast AP is also designed for high performance and support programming, which is can be beneficial for applications that need to be handled multiple, many concurrent requests. 
 6:47: So whether this is the reason I choose fast API. 
 6:50: Yeah, that that core actually is more powerful. 
 6:53: Whatever you have described, I mean that the core has everything, has everything, yeah, and it has more like native support from Microsoft. 
 7:01: So let me ask you this question, you know, because I, you just described, about the fast API right. 
 7:06: How did you do the authentication and authorization by using the fast API? 
 7:11: How did you authenticate, like, just one token? 
 7:15: OK, so yeah, for authentication and authorization, fast data, you know that provide basically I can say first of all, we use JW token authentication. 
 7:23: It is basically, you know, to give us more privilege to understand and the common approach to use JWT is I can say for authentication, right? 
 7:33: And the courses start when user. 
 7:35: Log in, you know, valid valid credential. 
 7:37: The server verifies the credential to generate JWT token, and basically that contained information such as user ID roll or permissions, and the token is, you know, then returned to the client for subsequent requests. 
 7:50: The client send the token into into an authorization header and typically for the. 
 7:55: We are, we may not take token and then, you know, when API received the request is first validate the token by checking signature and expiry time, expiration time, and any other required claims. 
 8:09: If token is valid, the user, you know, authenticate and, and, you know, request is allowed to, allowed to proceed. 
 8:15: And for authorization we can you know use information stored in a token such as rules permission, for example, admin endpoint may be required admin rules and violin regular user can only access standard endpoints and so authentication, yeah, let me ask you, so like, so as a another word, right, as the like, you can end for you if access token like you said everything has been like. 
 8:42: Packed inside, right, so basically that's like You have to authenticate authenticate under the request from there. 
 8:50: So how many claims do you validate? 
 8:53: How do you validate the signature? 
 8:55: OK, so you token, yeah, correct. 
 8:58: So first of all, you know, for validating, you know, against the signatures, so that exact number of claims depend on the application requirement, but typically I would include only the, only the claim that necessary for authentication and authorization. 
 9:13: For example, I would usually have the claims such as like user ID, username, or email, or role or standard JWT claims like issues or audience, issue times, and expiry times. 
 9:25: So typically applications, there might be. 
 9:30: Like 5 or 10 claims depending on the business requirement. 
 9:34: Additional permission are, you know, needed, I would, I can say I, I would also require permission-based claims, but I generally try to keep token lightly to avoid, you know, putting unnecessaries and sensitive information into it, so yeah. 
 9:48: Oh, how, how do you verify the signature? 
 9:50: OK, so this is very, this is very important, mhm, yeah. 
 9:53: So for, you know, verifying, you know, to, I can say, tokens of the API, you know, verify signature using the same secret key and public key that was, you know, used when token was issued. 
 10:06: Tools and we are trying using syn symptomatic encryption and both token generation and valid validation use the same secret key and if you know if you you we sorry if we are you know using a a sys a systematic encryption. 
 10:22: The token is signed with the private key and verify using the corresponding public key. 
 10:27: And during the validation, the framework check whether the signature is, I can say, matches or not, whether this token expired, whether the issues issuer or audience is are valid or not, or whether, you know, whether the token has, tampered, has been any tampered. 
 10:45: So, yeah. 
 10:47: Who? 
 10:48: You How are you delivering the JWT? 
 10:55: OK, what? 
 10:57: How are you delivering it? 
 10:59: Like, is it, yeah, like how do you deliver it normally? 
 11:03: OK, so, so, first of all, the project, you know, I worked, most common approach was delivery JWT through, through the authorization either using beer token or, patterns. 
 11:15: So after users successfully authenticate either through the login service or expert, like enterprise identity identity providers such as Azora AD, access to designer. 
 11:26: The client application for every subsequent request and client include that token and the request headed as like authorization via token and then the fast DP side, the authentication, malware or security dependency extract the token from the header and validate it if everything check out, checks out and a request to like proceed to the business logic. 
 11:53: And in some cases, especially, you know, from the browser-based application, I have been also in a token handle through the STP only cookies to reduce, you know, exposed to the client-side script, but, but in the healthcare platform, I work on the most of the, you know, of the service and application to service communication. 
 12:18: so what information were you putting in the claims that mean? 
 12:20: OK, so basically, you know, if I want, if I specifically, I can say the particular, I can say information. 
 12:27: The major information I use, like being focused on information like service and, I can say, typically I include like unique identifiers like subjects, claims, issuer, audience, expiry, expiry time, and, related role role related information. 
 12:45: And depending on the application, we might be included groups, membership, permissions, applications, specific rules, and could be user authorization checks as well. 
 12:56: So yeah. 
 12:58: So how do you ensure, how do you ensure that it's safely delivered, because if you're including that information in there without encrypting it, then it's anyone can read that. 
 13:09: Perfect. 
 13:10: So for the, for security purpose we use the JWT, you know, typically signed, not necessarily encrypted, so that, so claim are, you know, base 64 encoded, which means anyone who has token can technically decode it. 
 13:24: View contain because of that, we never put sensitive information such as password, healthcare records, right? 
 13:31: So the way we ensure such a secure delivery family through the STP TRS and all communication between clients, API identified providers or nos in service, we encrypt it into in transit and that prevents some, someone from like I say, in trying to interpret and I can say. 
 13:52: Encrypt the data, dating try to read that that while you know transmit over the network on the top of that that we use, you know, to sign signature product to integrate it with the tokens. 
 14:05: Even someone can decode the claim they cannot modify the content without invalidating invalidating the signature. 
 14:12: So yeah. 
 14:15: So is there any nons in there to prevent replay attacks? 
 14:20: I guess so, yeah, you know, I can say in environment I can say that reply no reply attack are definitely in a consideration because in GWT based system, norms can be no use depending on the authentication flow. 
 14:37: In our application we finally relies on the short-lived access token, STP token, expiration checks, and refresh a notation to reduce re replay disk, and we also validate standard. 
 14:49: Standard claims such as like EXP and INTs and you know some of the JWTIDs which can be used for uniquely identified tokens and for higher security scenarios, the nons or JTI, you know, value can be stored on the checks to ensure the same token is not reused, mis misculy and, there no exact implementation depend on the security requirement and identify provider being used. 
 15:16: So yeah. 
 15:19: OK, so in your fast APR applications, right, definitely you have the data models, mhm, right. 
 15:25: So can you tell me, yeah, I, I, I pretty assume you use the like a pathetic, right? 
 15:30: Mhm, yeah. 
 15:31: Can you tell me when to use data class, when to use paetic? 
 15:35: OK, so far, 1st, 1st tell me what is a data class. 
 15:41: OK, so basically, you know, I can see that, sorry, you asking about the data. 
 15:47: D decorator a decorator. 
 15:49: OK, so basically they're decorators, I can say they're more on the Python side, you know, when typically use decorator when I need simple glasses that primarily used for holding structure data instead of manually writing constructors or the I can say the comparison method and I can say decorators generate those not automatically which makes the code such a such cleaner and easier to maintain. 
 16:15: So that's why we use in decorators. 
 16:18: Yeah, why do we use the decorator data plus decorator? 
 16:21: Why do you use the pandemic data model? 
 16:23: So what are the pros and cons? 
 16:25: OK, so basically, you know, the pros and cons and why we use that. 
 16:29: Like, so, if you know, I can say that data class, you know, decorator was infused in the Python to reduce boiler code when creating classes or. 
 16:39: store data instead of, you know, manually writing the constructor, the comparison method map Python generate them automatically and I typically use class, data class for internal domain models and data trans transfer objects where I need simpler and a lightweight structure and don't require runtime validation. 
 17:00: And there, there is no pros and cons as well because the main, main advantage are, you know, less brate code and that, that's OK, that's OK. 
 17:09: My question was like why do you choose that a class. 
 17:14: What do you choose Python. 
 17:15: OK, OK, OK, so I, I'm more into the data side. 
 17:19: So yeah, you know, the different, the funds scenario I choose parenting and data, data is intending leaves our system such as like API request, API response, and I, so I choose data class for internal application object where the data is already trusted and validated and Then are, they are just simpler and lightweight and for practical example, I can say fast AP would be request payroll come into the AP through parenting model that can validate and then inside the service layer I may convert into the data class for business, processing. 
 17:54: So my rule is, my rule of thumb is like parenting at the system boundaries and data class inside the business logic layer. 
 18:02: Tell me what is a dependency injection. 
 18:04: OK, so basically, you know, dependency injection, I can say, is more, I can say, you know, than dependency injection design pattern where object receive the dependency from external sources instead of, you know, creating them itself. 
 18:21: The main benefit, is loose coupling. 
 18:24: The component focus on. 
 18:27: the dependency injection is API implementation. 
 18:29: sorry, sorry, can you come again? 
 18:32: The dependency injection API implementation. 
 18:34: OK, so basically dependency and injection, I can say, they are, different kind of scenario. 
 18:40: The API application typically implement, dependency injection by defining service separately and then injecting them into the component. 
 18:49: That need, need them and rather than just creating, you know, those services directly inside the endpoint controller. 
 18:54: And for example, if I have user API I might have user service that contain business logic and repository that handle database access. 
 19:04: The API end points depend on the user service and users of the user service depend on the repository. 
 19:09: And instead of, you know, creating those objects manually inside the endpoints, I registered them into the dependency injection container and bank requests come in, framework automatically resolved and at the dependency and provide the required assistance. 
 19:24: So, yeah. 
 19:25: What's the similarity, I mean between the dependency injection and the Python closure. 
 19:32: you asking more like a scenario. 
 19:35: What is the Python closure? 
 19:37: OK, Python closure. 
 19:37: Sorry. 
 19:38: So they are, you know, they are related to a sense of both, like allowed function to, to access something. 
 19:44: This is, provide outside of rather than just creating internally closure, you know, capturing the variable from its surrounding scope and keep access to that dam, you know, even after outer function has finished executing. 
 19:58: And dependency injection, you know, on the other hand, provide basically dependency from external sources such as frameworks, containers, instead of no object creating those dependency itself, so, yeah. 
 20:09: Both are in a separation of concern, Mhm. 
 20:23: let me see. 
 20:35: 2, Explain to me your pedantic implementation. 
 20:40: I do love pedantic. 
 20:43: so explain to me how you, how you implemented it and how you utilize it in the system. 
 20:48: OK, so basically in our fast API application, yantic was primaly used for request validation. 
 20:54: And response evaluation and data consistency for every, every API we define parenting models for incoming request or outcoming response, right? 
 21:04: And when request came in past pay automatically validate the payload against the. 
 21:09: Identity schema before the business logic was executed and we use you know feed the type validation of optional fields, nested models, and custom validators and yeah, such as, you know, minimum length, maximum length, and rejects patterns so that they just basically help us to catch invalid data. 
 21:28: At the API boundaries itself instead of, you know, handling validation throughout, throughout the application and it's also automatically generated open open AI and open API and a document which made API consume easier for the team. 
 21:43: So yeah, this is the IP and if the client send the invalid emails, or you know, non-medicate identing automatically return the validation error before request reach to the service there. 
 21:55: How many ways to do, how many ways to do the data validation from Pontic? 
 22:00: OK, so there, you know, I can say majorly, major way I can say there, you know, over several ways, first of all, you know, first, I can say first type-based validation where parenthe automatically validate based on the fields such as like type in and string data, daytime time and emails to your. 
 22:19: Second field constant like where we can enforce rule like minimum length, maximum length, rule range, or reg pattern. 
 22:27: And 3rd is customer evaluator, where we write our valuation logic for the specific field. 
 22:35: Venus rule of for more complex, and, fourth is, cross-field evaluation. 
 22:41: We are, you know, validation depends on the multi-fields and together and such as like checking that end to end, like end date or the start date after the start dates. 
 22:51: And finally, we can say we use, you know, nested models in our upon our, our approach and, when evaluating complex request or structure for the child objects, so yeah. 
 23:06: Have you ever encountered, I mean, the other memory, I mean your Python application using tons of memory. 
 23:12: What could be happening? 
 23:14: Oh yeah, so basically, you know, yeah, this kind of scenario I have also faced the expense, excessive memory, you know, consume can be happen, Python application and especially on the data processing side and long running services. 
 23:28: The first thing I I would do to identify whether it's actual memory leak or sim simply high memory usage due to workload. 
 23:36: Common causes I, I, I have seen, including, you know, loading large data set into memory and keeping unnecessary objects alive. 
 23:44: And unmounted catching as well, large in memorial collection. 
 23:47: These are the major causes. 
 23:49: And, you know, in Python, especially the circular reference or global object that may remain the referenced for a long time and, and can be, you know, contribute to memorial issues as well to investigate. 
 24:01: I typically use profiling tools like trace melog memory profiler and application metrics and you know container monitoring identify identifiers which which is object I consume memory or whether maybe use continues doing what time. 
 24:17: And, I, if I want to fix that issue, the solution will depend on the root cause, and common fixes include processing data, batch batch batches, and data in batches using generators, instead of loading. 
 24:32: So yeah, these are, you know, common fixes I can say. 
 24:36: Difference between a generator. 
 24:39: OK, so generator, I can say major difference, I can say the generators, both are basically, iterators or and generator are used for lazy, evolution and meaning they are produced values one at a time. 
 24:54: And instead of, you know, loading everything in, into memory. 
 24:57: The main difference is that, you know, the creator is an object that, that is implemented in the ITR of method and the next other methods where, where it is, I can say generator is simply a way to create it creators using yield feed and under the hood, every generator is it created and but not every, you know, traders is a generator. 
 25:22: So yeah, that's my understanding. 
 25:26: OK, why the generator you can only write it read it one time. 
 25:30: OK, so yeah, basically, you know, over, over the experience and now I feel that the main, reason is, you know, memory efficiency, Gerator use yield yield keywords which is, pause the ecution and return the one value at a time, right? 
 25:46: So when the time when, when the next, value, you know, is requested, Execution resume from the various left of and unlike list generator, it does not allocate memory or value upfront. 
 26:00: It generates value only when they are needed, which those are lazy evolution. 
 26:06: And for example, if I need to process millions of records, a list would create all millions recorded in the memory immediately. 
 26:13: And a generator would create only the, only, you know, current records being processed and then move to the next one when requested. 
 26:21: So, that's why generators consume significantly less memory and roll out more used large data sets. 
 26:29: Why the yield is so useful in the like in the testing in the unit testing OK, basically, you know, really I can say why we basically I, I, I, as for my understanding mainly I can say. 
 26:44: it just like I say, that's a separate data, not test data from the test mode and the start of, you know, hard coding inputs, expected, I can say a Python test file, we can keep an YML file which is easier to read and modify. 
 26:59: I also make test more, driven and business users and Q engineer perspective sites. 
 27:06: And another advantage I can say is human, Bible is, you know, human readable and support hierarchy structure. 
 27:12: Which makes it, do you understand my question? 
 27:15: Can you rephrase my question? 
 27:17: You asking me to explain the why. 
 27:20: No, not, not yellow. 
 27:21: Yellow, yellow, yellow return. 
 27:21: Why yield is so useful in the testing? 
 27:26: So you have the fixtures. 
 27:27: OK, sorry, sorry, I, I, I thought it's. 
 27:30: So basically, you know, I can see yield, you know, major advantage of yield because, as I said, memory efficiency, and when function user return it, it is a skewed. 
 27:40: Complex, I can say complete, completely, return, sorry, execute completely and return the entire result at at once. 
 27:48: And like I said, the main advantage is yield that allow us to generate value one at a time instead of loading everything into the memory at once. 
 27:57: And when function I'm talking about setting up the fixtures in the unit testing in the unit testing. 
 28:06: the major activity in Pie test yield is in a commonly used, right, in a picture, picture, right? 
 28:12: Yeah, exactly. 
 28:13: So basically the code before yield performs the setup, such as like creating database connection, test client, test data. 
 28:20: So I can say, and, and then, you know, provides the test to the yield after test finished, the code of I can say code after yield is automatically execute for the cleanup. 
 28:30: And such as like closing connections, deleting my temporary files, roll back the test data. 
 28:36: So that's the, that's, you know, why you be using it more commonly. 
 28:42: It You're doing a great job. 
 28:46: I'm sweating. 
 28:47: I. 
 28:51: yeah, so I can ask a little, let me see, and we still have time for technical questions, and we can get into some softer questions, So We've been, what, when you're writing unit tests, how do you normally approach your writing these unit unit tests? 
 29:14: Oh, so more formal, I can say major are, you know, scenario, my approach was I can say first I understand that business logic. 
 29:23: That this is major needed and that, you know, that to evaluate, identify expected behavior on possible edge cases and failure, you know, scenarios before writing the test case. 
 29:35: Typically, I I follow the arrange, arrange, act, and assert pattern. 
 29:41: First, I said, set up the test data and. 
 29:44: Mockups, then I view the function or API being tested. 
 29:48: Finally, I verify the expected outcome for backend service. 
 29:52: I focus on testing business logic independently from external dependency for database call or producer or third party APIs, usually mock to keep test fast and reliable. 
 30:06: I also try to cover, you know, positive scenarios, negative scenarios, validating failures, 8 cases. 
 30:12: The goal is not just in the court coverage, but ensuring applications behave correctly under the different conditions. 
 30:18: So yeah, these are the majors. 
 30:20: With one sentence, with one sentence, tell me what's the difference between unit test and the integration test. 
 30:26: OK, so basically one sentence I can say the unit test, you know, verifies single component in isolation using mocks, whereas integration test is verified that multiple components work together or correctly in the in the real dependency. 
 30:42: So yeah, like I said, these are one one another. 
 30:45: But let me tell you, I really test you wrong from the GitHub parameters. 
 30:49: It really test you wrong on the same, on the, on the real thing, right? 
 30:52: Yeah, on the real platform. 
 30:59: OK, why don't you do the, oh, let me ask you this, OK. 
 31:02: So you also have, experience in the observabilities, right? 
 31:08: Mhm. 
 31:09: So when you do the like, in the track, you always see this kind of thing. 
 31:15: I mean that string is used in the logging. 
 31:18: Why, why it's complaining. 
 31:22: OK, so, major, I can say I can say when you I look, look at the Linux application logs, you know, often see, like you format like different distinct format and loging statement. 
 31:34: The main reason is performance and efficiency. 
 31:37: like instead of, you know, constructing the log messages immediately, we pass the format string and variables separately. 
 31:44: If that log level is disabled, Python does not know spend time, spend time building the final string. 
 31:52: It's basically keep the, I can keep logging consistent and make the structure logging procedure easier. 
 31:59: So, yeah, I, I use, I can say I use the production system that high in high volume loggings that would reduce unnecessary string and formatting over overhead and considered logging best practices. 
 32:15: Yeah. 
 32:17: Evaluation really doesn't matter about the locking level you will just like evaluate that that string. 
 32:24: I agree, I agree with that. 
 32:26: But yeah, I think like exactly you know it's a form of lazy evolution where we write something like logger.info right and like and like it will give logging user login of with the user ID so logging frameworks to delay the formatting right and the message until it's actually needed if that log is like level is not enabled, the string formatting never happened, right, which saves CPU memory override. 
 32:57: So, yeah, correct, basically benefit lazy evolution is log only a message only formatting if the logging level required, which is basically improve the performance and in the production system. 
 33:12: All right, let's ask a few softer questions before we get into Into the coding exercise. 
 33:21: what is one thing that you want us to know from your resume? 
 33:24: Like what's one project that you really want us to know about? 
 33:29: One project, I guess, I guess in the starting I cover my current project, but I, in one project I would, I really like you to know about like healthcare data, education, and analytic platform. 
 33:43: I work on tenant health. 
 33:45: The reason is highlight this project is because it's brought in brought you know together almost everything. 
 33:52: I enjoy working on the on the Python backing development, AI designing and architecture event driven. 
 34:00: So I, I was responsible for developing fast API based microservice and the APIs and the, the, you know, I can say. 
 34:10: we used post as well for data storage and Kafka for evidently. 
 34:14: Why I found most reward rewarding was, you know, was solving scalability and reliability and challenges that data volume grew because we're dealing with the health-based data. 
 34:24: It's largely been a when it's too quickly to, you know, go up in the high traffic sites. 
 34:30: We optimize data processing workflow and improve the AP performance, and we successfully, you know, achieved that our requirement and we given the most performer perform application. 
 34:42: Have you been building the pure back time backbones. 
 34:47: So pretty much, yeah, what thing is working on that's the operational data bus, right? 
 34:52: Yeah, so yeah, have you worked, I mean, on your resume it seems like you have been working with Kafka and all those things. 
 35:00: Can you tell us a little bit about those experiences. 
 35:03: on, on the Kafka experience, you think, yeah, OK, so majorly, you know, I, I, I really know really work I enjoyed with the CAFA, because I absolutely, you know, in the healthcare platform, you know, we use CAA family because, you know, event drivent data processing and system mitigation. 
 35:18: We had coming from multiple data data coming from multiple healthcare systems instead of in a tightly coupling service through the synchronous API, we published the event to the Kafka topics in different downstream service, but then you consume those events independently for analytic and devoting our official workflow. 
 35:38: My involvement, I can say. 
 35:40: Including designing and designing producers, consumers, defining the event schema, handling the error scenarios as well, monitoring messages, processing, and ensuring rely, ensuring reliable data flow between the services. 
 35:55: And one of the biggest advantages we saw was improved scalability and decoupling. 
 36:00: Service could process data at their own. 
 36:04: Our own pace without impacting on our streams of system, which can be very important important as our data volume is increased. 
 36:13: Yeah. 
 36:18: OK, I think we have time for one more, what are you most proud of? 
 36:24: Like, it doesn't have to be a big thing. 
 36:25: It could have just been something you figured out or something that, just really cool after you go.
0:00: Reliable data flow between the services, and one of the biggest advantages we saw was improved scalability and decoupling. 
 0:08: Service could process data at their own pace without impacting on our streams of system. 
 0:15: This can be very important important as our data volume is increased. 
 0:21: Yeah. 
 0:25: OK, I think we have time for one more, what are you most proud of? 
 0:31: Like, it doesn't have to be a big thing. 
 0:32: It could have just been something you figured out or something that, just really cool after you got working. 
 0:40: yeah, like, they have one actually, one I can say experience I have been where I, I feel like I'm really done really good work. 
 0:49: And one thing I, I would, I'm proud of that because our data basically, Our data volume grew, as I said earlier in my answer because we're dealing with the health based data. 
 0:59: So data volume very grew up very easily, and some of our processing workflows started experiencing delay which affected the downend and reporting. 
 1:07: And our main priority is we've maintained the performance of our application. 
 1:12: So we have to first identify this issue because it's experiencing delay for the US user perspective. 
 1:18: Which I affected, you know, I can say I'll work on redesigning the part of workflow using synchros, a synchronous event driven, processing with the Kafka. 
 1:26: I optimize, you know, some post-gra SQS, postgra SQL query and help to break the workload into the smaller independent service. 
 1:34: the part of, the part of I am most work out is not just, you know, technical solution, is, is, it's you know that where I'm able to improve the reliability and toy. 
 1:46: Efficiency without, you know, and disrupting the existing services operation. 
 1:50: Seeing the big scale successfully and adoption increase very rewarding. 
 1:54: So yeah, I can say most part of work I guess yeah, you talked about that one. 
 1:59: So reliability, let me ask you, how do you do the like, ability Grios data quality for. 
 2:06: Data. 
 2:09: OK, OK, so basically, you know, data quality, I can say that will be very important for because, you know, we are indicating data for multiple healthcare systems. 
 2:18: We implemented validation in at multiple layers at the eBay layer we use parenting models and validating incoming requests to impose schema rules. 
 2:28: And during the data processing we checked required fields, data types, mismatches, duplicate records, and evaluate values. 
 2:36: We also, you know, use database construct where, appropriate and, you know, and, edit monitoring to, like, like logging identify data quality issues earlier for event your workflow ensure consumer, you know, consumer validate message payload before processing them. 
 2:52: And in addition, we worked closely with the business team to define data quality rules and the conservation steps to ensure, process, process data match source system expectation or not. 
 3:05: So, yeah, that's how we are maintaining data. 
 3:18: so Oh, can you see this? 
 3:24: OK. 
 3:26: So let's get into the The technical assessment so that we have enough time for questions at the end. 
 3:36: so here's a very basic, Example of a Python application. 
 3:45: And we'll start by just saying can you just look at it for a minute and just explain to me what's going on. 
 3:55: The looks really smooth. 
 3:58: Does it look smooth. 
 4:04: What I'll do that. 
 4:19: Oh But OK. 
 4:27: He now 3. 
 4:33: A small yeah. 
 4:35: Oh. 
 4:40: I'm trying to fit it on one on one, I can see that I can see classes similar to a handle logging mixes, you try mixing, and right, and. 
 4:58: I will do this. 
 5:01: So you can see the bottom of it too. 
 5:03: It's good. 
 5:06: there we go. 
 5:07: Problem solved, Let me understand past understanding of nature and change because. 
 5:23: So, like, I, I read the code correctly, but, So what, what would I need to explain like here? 
 5:32: Yeah, just tell me what's going on in here. 
 5:34: What's, what's this? 
 5:35: What's this doing? 
 5:36: What's gonna happen when you run it? 
 5:39: Like what, what is this? 
 5:40: What is this doing? 
 5:41: OK, so as per my understanding, the right now in this code at the high level, the code is implementing. 
 5:49: Handle pipeline using like mixing and the base handler and class providers at the inheritance and each mixes and you can say basically is demonstrating the combination of object-oriented design pattern and the handler's class is the base section. 
 6:06: It defines the abstraction handler from the method and that, you know, every, every ingredient in a handler must implemented. 
 6:15: And it also implement call method which means stance can be or like function. 
 6:22: I also noticed use of in it subclass where, you know, subclass created with a key argument and it you know automatically registered itself, you know, the three directories and that is actually. 
 6:40: essentially for plug-ins and other patterns and the login is, you know, added in a blogging period before processing the messages and it basically print the last name and the message and then call the super handler. 
 6:56: And, and retry mixing, you know, I did retry functionality. 
 7:02: It attempt to, execute then downstream handle and multiple times and retry if exception occurred or not and, ecola you know contain. 
 7:14: Actual business logic, actually, there is in, in the equivlog where a main business logic exists and in inherited from the handler. 
 7:22: A string is simply reading the message upper method that converting the string to the lower case. 
 7:29: And when I run, you know, the loud and loud, the loud, the result would be, as I say, it's a hello world since, you know, handler implemented call method, calling loud loud hello world internally invoke the loud dothandler world hello hello world and. 
 7:52: that's basically execution, tool will be logging mixing handler that execute first printed in the log message and it called super handler. 
 8:04: The control moves to the retry mixing handler. 
 8:09: And we try mixing enter to the retry event loop and call super handler and Like control move to like each each eco handler and eco handler return the hello button. 
 8:23: and, yeah, final result contained the hero. 
 8:27: Yeah, I guess, that's my understanding too well. 
 8:33: You know. 
 8:34: Probably 90% of that. 
 8:39: Actually I just got to the starting is really hard to read, but I, you know, it's now it's. 
 8:45: I think the one thing you missed is the registry is a single dictionary and the handler and not the per subclass like the field was, yeah, yeah, yeah, yeah, like they got like 90% of everything, so that was pretty good, I, I noticed that that is, but there's not in a fully yet. 
 9:03: I explained it, but, because in history being populated to the init class subclass function method when new handwrite class is defined with the keys such as like. 
 9:14: Class eco or eco class right or the class automatic register register itself you know handleries so yeah that's this will allow us to application that dynamically look up or yeah yeah that's understanding. 
 9:32: Awesome. 
 9:33: So what would happen if I were to swap the bases, Of So If I were to swap that order from logging mix right here it's looking at, so if I were to move this one to the front. 
 9:51: OK. 
 9:54: And then put this in here. 
 9:59: What would happen swept the logic when we tried so. 
 10:05: I guess behavior would change, but. 
 10:13: What it is like If I move eco in the front, right, so that would significantly change right is it because you know, main, main swapping you have done this is MRO did change, but the observable output did not in the original version that claim you know chain was launched that, you know, that call that chain was logging and retry and echo after the swapping, it become retry logging and eco since. 
 10:43: since there was no exception being thrown, the both mix mixings all supermethod and the logging still happened once is still return the uppercase string. 
 10:55: So the final output remained the same, but the flow would be changed. 
 11:04: Yeah. 
 11:10: Well, OK. 
 11:14: So Put it back. 
 11:26: All right, so if we try and mix in the dock handle, so we have this right here. 
 11:34: If, It has a bug Can you figure out what that bug is? 
 11:49: Who is, one potential issue I see. 
 11:56: Did you try mixing ketch? 
 11:59: let me, let me check one second. 
 12:09: Yeah, the retry logic only works if the exception is raised. 
 12:14: And if the downhill handle return the invalid result, like non, non-empty response or bad data, we try mixing considers a, is a successful and never retries, but there is no even more, I can say. 
 12:31: If, if it, if it's catching all the exceptions, right, and like including programming errors that should not be retried. 
 12:39: And one thing I stand out like I did try mixing patches every exceptions and typically I would retry only transit failures such as like network or service availability and retry coding errors like type type error or attribute error were not, you know, help to can be tried, hide the real problem. 
 13:01: And I also notice any logging happening outstanding and they try loop because logging mixing is you know before they try mixing and in the MRO and if they try. 
 13:18: which occur only first attempt get logged, and, it might be incorrectly to assume there only one attempt. 
 13:29: I think you had it right in the first sentence where it does, it will throw a runtime error if it because of If the retries is 0 or it's bad data coming in, then it's gonna, it's gonna error, so yeah, so you would need to put a guard and, in order to so that it wouldn't, error right here. 
 13:56: All right, so the next one, why does the handler, so this ABC handler, Why does the handler work without a medic a me-class conflict? 
 14:10: And what would it cause an issue the handler, I can say abstract as a, I can say abstract class that basically you identify contract for like all handlers and by inheriting inheriting like from ABC and marketing handler method it as I can see. 
 14:37: Upset about it and I can actually insure but I think. 
 14:46: I This basically the reason I can say the handle in inherited class from ABC, which means Python use ABC meta as a metaclass for that class. 
 15:00: Then every subclass of handlers such as Leo or loud, ultimately inherited from the same metaclass. 
 15:07: And yeah, so there's no conflict because Python can we find common metaclass that satisfy all parent classes. 
 15:16: And when it becomes a problem, when it's two parent classes and choose in capability metal classes. 
 15:24: like I said, that's, Yeah, that's exactly right. 
 15:31: yeah, that would be the issue if you inherited a different meta class like something from fast API or Eum meta, then it would cause issues, All right, could you rewrite the logging mixing as a protocol? 
 15:51: OK, so could we, could we rewrite this as a protocol instead? 
 15:57: Yeah. 
 15:57: So, like, instead of, you know, requiring inheritance from the specific base class, protocol defines the required method, any class, right? 
 16:05: So I can see if, if I were to rewrite the using protocols, my goal would be define. 
 16:13: The behavior of contract rather than just providing implementation to the inheritance and then any class that implemented was kept like capitable and handle handle method automatically satisfy the certify the protocol without excluding the inheritance from it. 
 16:33: And the key difference would be protocol is focused on structured, typing rather than just inheritance. 
 16:40: And with the current mix mixing approach like logging mixing, injected beaver into the inheritance chain through the arrow and the super method. 
 16:52: And the protocol was not, you know, would not provide the implementation. 
 16:56: It would simply define the exact, expected, sorry, expected in high end. 
 17:01: And the advantage of is that you know reduce height complexity and avoid some MRO and metagrass concern we are discussing on earlier, right? 
 17:12: So it, it is, it will also give us more flexibility because object expose the Capital handle method method can be part without needing the inhalers from the common base class. 
 17:27: so, yeah, that's fine, yes, so, so, yes, but in this specific example, could you write that as a protocol or would you or not? 
 17:42: I guess my answer would be. 
 17:45: Yes, I can see. 
 17:48: You can take, yeah, so, for example, I would at least say not directly like because logging is not just a defining a netance provider behavior. 
 18:02: A protocol is really intended to define a contract. 
 18:06: For example, it can say that the object must have handler method, but it, it does not parti participating in the MRO. 
 18:15: It cannot provide the, cooperative super method behavior that is, mixing rely on it. 
 18:22: And in this school, basically the entire, entire purpose of this class is logging mixing classes, you know, injected functionality into the inheritance chain and being active as a behavior mixer, mixing and if kind of if, if I converted into the protocol, I would lose the logging implementation completely. 
 18:44: And because protocol does not provide behavior in the same way mixing too, right? 
 18:48: So. 
 18:49: My answer would be that I would create protocol describing something that support handler method, but I want to replace, you know, logging mixing itself with, with the protocol because it's mixing, mixing, you know, providing functionality that not just not defining the items. 
 19:08: yeah. 
 19:09: That's why my approach. 
 19:13: OK, yeah, I mean, yeah, I think that it, it, you were there and yeah, so the big thing is that the MRO because it resolves through super you couldn't, you would like you said you'd have to change the application in order to implement it as a. 
 19:29: Protocol instead of just being able, you couldn't just put in a protocol and have it work you'd have to actually change the application because of the MRI stack but yeah no you said everything you were supposed to say so that was good so if someone defines a quiet, this quiet echo, so we have this in here so we have this defined, With without the key, so there's no, no key in there, is it in the registry, On this. 
 20:10: I guess, Anything. 
 20:16: No, actually, why would not be added as a registry. 
 20:21: The registration only happened inside in it subclass then subclass created with the normal null key. 
 20:28: And so eco, a key like a key eco like allowed has like right. 
 20:33: So, so both those are get registered. 
 20:35: But quiet is defined like class quality right and pass, so there's no key pass in there. 
 20:42: So inside in the subclass, the key is none and the condition fails. 
 20:51: Let Yeah. 
 21:05: I hope I'm right. 
 21:08: So why is it that the key is not, not important versus a truthy check? 
 21:15: Actually, you know, he's basically. 
 21:19: No, that actually good, good, first of all, the lines if he is not done. 
 21:24: The more explicitly than using a to to to check like if key because it allows valid false values still be registered. 
 21:34: For example, if somebody, intentionally used keys, as a blank string or keys equal to 0, then through the check would be treated those that are false and skip registration entirely. 
 21:49: But with, with the if he is not, is none like this kind of condition, it's only saying like none means. 
 21:59: Don't, don't register any other value, and if it's faulty, it's treated as a, legitimate key and from the, yeah, and from a defensive perspective, defensive program perspective is, is none is more of pricing because the distinguish between non-key was provided or key was provided was, happening like, evaluate, protocols. 
 22:38: Yeah. 
 22:38: So, because it, it was, it was not none in the ricky check, we dropped It silently dropped the key, so it would not be in there, yeah. 
 22:51: So not none makes the contract explicit, Yeah, you crushed that. 
 22:58: the last person I interviewed with this, we didn't even get through all five questions, so. 
 23:04: That was supposed to be hard. 
 23:08: yeah, actually, I'm starting, I thought it would be some crazy thought program, but when I, you know, when, when it's easy to when, when, when, whenever you want to read the, and try to understand the logic, it's more easy to understand the behind the scenes working, not judging by the code, but when you understand the code, it, it's more easy to understand behind the logic. 
 23:31: Exactly, So, I guess another question I can ask is why did we get a second hello world? 
 23:44: That would be a good one, I guess so. 
 23:48: Because you know, I can say because after the loud example I think the code is also creating like cutting a quite an instance. 
 23:56: I can see like in the update code like you are like so so basically you know in we actually running two separate handle objects first. 
 24:07: Loud equal like loud method is in the result loud hello, which is produced the hello world right and the later the quiet method is also, you know, returning the I could say quiet hello world. 
 24:18: So since quiet inherited directly from the eco, it is still executed like message, right? 
 24:24: So yeah, this is made the difference is that quite does not inherit on the logging stick and time mixing and so it won't see the logging output. 
 24:35: And yeah, that's why we second he was he is output it. 
 24:40: Yeah, now I'm gonna add more questions to my, to my list of things. 
 24:46: Yeah. 
 24:49: OK. 
 25:01: Yeah, OK, so obviously I have to sit down and I enjoyed the coding practices. 
 25:07: I have this kind of question because it's more focused on understanding how Python works, understand, code rather than just writing a code from memory, right? 
 25:15: So it was, it was interesting. 
 25:19: No, it's in this, in the age of AI, it's like it's, you have to understand the theory, you have to understand the language because you can get AI to write you code all day, but if, if you're, if you don't understand the foundations and you don't understand what's going on, it's garbage in garbage out and you're gonna have a crappy foundation. 
 25:39: So the point is you need to understand the theory and what's going on. 
 25:43: in the code more so than being able to write me a script that can sort, you know, yeah, yeah, cool. 
 25:53: How, you know what, I always ask the AI ask me, ask me, don't really soon. 
 25:57: So yeah, it's gonna ask you a whole bunch of questions. 
 26:00: You should be able to like a guide the AI and I don't like the AI like a guide you right, exactly. 
 26:07: and the same thing, you know, I always tell my media developers because not always depending on the AI and chatbot response, you should, you should know about the, basic understanding, at least the base foundation, and, yeah, it's actually more necessary for this kind of, you know, driving this kind of generation. 
 26:25: Because they all depending on the giving the output which is coming from the AI I just to piece it on piece it on on the the fundamentals are more important in the in the AI. 
 26:43: Yeah, and I have one question like like what are the rules and like expectation you have on particular for this rule? 
 26:53: And yeah. 
 26:55: Is there any expectation or role or responsibilities or particular part of this role? 
 27:04: sorry, say that one more time. 
 27:05: I'm, I'm like, I am asking like what are the rules and responsibilities, for and what are the expectation, you guys have for for this rule. 
 27:15: So for, for the ODD project, I'll give you a little bit. 
 27:18: It's, it is a data bus like we were saying earlier, and I think the biggest thing is we have a proof of concept. 
 27:25: We've, we've gotten it to work. 
 27:27: We've done all that stuff. 
 27:28: It's getting it from. 
 27:30: I don't want to say like It is, from like, I wanna say from the application is now to like the, the rigid, you know, production grade application we need, because right now it's, it's a, it's a struggle between, you know, engineering and product to be like, this is a viable tool that we can use. 
 27:55: And we need to be able to demonstrate that. 
 27:57: So the purpose of us bringing on, you know, more people and more, Python experts is to get this, you know, leading deliverables, getting out the door, getting it so that it is, you know, a hardened, production-ready, secure application that can be, utilized in the secure environment so that we can, you know, show that this is not only viable, but this is the solution that we should be using. 
 28:23: So a lot, and so to say that a lot of the responsibilities is, you know, like creating, you know, working together, like we'll be doing a lot of stuff together like working through like, all right, here's the architecture, this is the approach we wanna take, you know, plan it out, getting the, specs, you know, writing out the code, reviewing the code, that's our biggest bottleneck right now is like PR reviews, stuff like that, and so for us it's, Yeah, a lot of like just, Like nitty gritty stuff, like just making sure this application evolves and grows correctly using the correct, you know, design patterns, making sure it's production grade like you said AAA for testing because that's super crucial. 
 29:09: That was the big thing that I put onto the project if we went from like almost no unit test to I think I've got it up to like. 
 29:16: Close to 1000 unit tests for all of our stuff because of, of the need for it and making sure that it's, it's production grade and that it is doing, like you said, doing what it says it does. 
 29:29: so, yeah, for us, it's a lot of like Getting it from, you know, where it is like ground floor into something that's an enterprise level application. 
 29:40: OK, and that, that's a lot of make sense actually. 
 29:43: And yeah, quite interesting because you already in that phase where we have to do first of all coding practices we, that your requirement and expectation are matching or not and code quality is more actually required for this kind of projects and yeah. 
 30:00: I, I enjoy working there. 
 30:03: Yeah, what was your previous role? 
 30:05: I'm sorry. 
 30:06: What was your previous role senior senior engineer? 
 30:10: OK, OK. 
 30:11: No, I'm, I'm actually more of the lead full tech development in the Python. 
 30:15: Mainly I'm in the Python, but I'm was full tech. 
 30:18: Oh yeah, that's why on the resume I see everything, yeah, I can, I become dizzy, yeah. 
 30:29: It's OK. 
 30:29: Yeah, your Python skill is pretty good. 
 30:31: Yeah. 
 30:33: OK. 
 30:36: Yeah, and any questions? 
 30:38: And yeah, one last question is what, what will go into the next step after this? 
 30:44: Is there any next round? 
 30:47: so next steps are, We, we go back to date and we say this is, this is the result of everything, this is, You know, this is how we feel about the situation they go through and compare that to The other candidates and then from there they, they make the ultimate decision, Jaden and What's his name? 
 31:20: I forgot off the top of my head. 
 31:23: no bro, really, I think so. 
 31:25: not bro. 
 31:26: I think only Jaden. 
 31:28: It probably is Jaden then, yeah, Jaden's the higher manager. 
 31:31: Yeah, you're going to hear back from Jaden. 
 31:33: Yeah, we're going to give all feedback to Jaden. 
 31:34: Yeah, OK, yeah, and then he'll, he'll get, get back to you on that. 
 31:39: Sure, I understand, and thanks for giving me insight actually. 
 31:43: Yeah, and that's all for mine. 
 31:47: All right, awesome. 
 31:48: Yeah, you can get like roughly 30 minutes back. 
 31:54: Which is a good thing, you know, generally speaking is the best thing, very much so in a very good way, so yeah. 
 32:02: I Yeah. 
 32:06: Absolutely thank you nice to meet you. 
 32:09: Thank you and happy to meet you. 
 32:11: I see. 
 
