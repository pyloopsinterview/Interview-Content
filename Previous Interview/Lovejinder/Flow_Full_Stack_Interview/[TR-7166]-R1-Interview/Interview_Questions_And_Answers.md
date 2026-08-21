0:00: , loading the, OK, loading the, can you see the back. 
 0:07: I'm The daily show a stand-up call at 6:30, so I'll continue with my. 
 0:14: You can continue after the next one, yeah. 
 0:19: OK, thanks. 
 0:22: OK, let's quickly start, learning that, can you please, introduce yourself? 
 0:27: What kind of expertise do you have? 
 0:29: How many years of experience do you have, and, last project, which technology you choose, and, explain your, explain your last project. 
 0:39: Yeah, sure. 
 0:40: So, like, my name is Ajila Singh, and like I have a little 11 years experience in backend development. 
 0:47: I'm mainly focusing on Python, Django, fast API, cloth, and like microservices. 
 0:52: And like most recently, I have been working as a lead Python like AIM a developer, selective Insurance. 
 0:59: And like my main responsibilities is like designing and like, you know, developing scalable backend services and like APIs for enterprise insurance applications. 
 1:08: Yeah, like I work with Django and Python for like application layer, post SQL and like Mogodi for data, Reddis for caching. 
 1:16: So yeah, and like I'm also involved in API security, performance optimization, and like database tuning. 
 1:22: I have also conducted like good reviews and like mentoring developers. 
 1:25: That has also been my topic. 
 1:27: Yeah, like on the cloud side, like I have like a strong experience with Azure along with like Docker Kubernetes Jenkins and Git and yeah for deployment like, CICD and over the years like I have also worked with Azure Data bricks, ISpark, and yeah, Delta Lake and data tables for like large scale data processing. 
 1:49: Yeah, so, like, overall, like my role has, you know, grown from like hands-on development into technical leadership where like I am involved in architecture, troubleshooting, design decisions and like delivering solutions to the other teams. 
 2:02: Yeah, that was a little over ordinary. 
 2:06: OK. 
 2:08: That's good. 
 2:09: do you have experience in, data mix also? 
 2:11: Yeah. 
 2:13: OK, so do you know how to create the job, how to create the pipe, means, how to call the idea pipelines to the, data jobs? 
 2:25: Yeah, sure. 
 2:25: So like, like telling about how, how will I create, like, yeah, it's the pipelines and data breaks. 
 2:33: Like I have had hands-on experience with your dataics, especially I would say like 5 Spark and Delta Lake and Delta tables. 
 2:40: For example, you know, like in, in one of my projects, like we had data coming from a different operational systems. 
 2:46: And yeah we use data breaks and piles part to ingest that data and apply transformations and business rules and then store the process data in data tables. 
 2:57: And like for the job set up, we would create a database job and like associated with a notebook on Python or like P spark code. 
 3:05: And yeah, like we could define the cluster configuration parameters, dependencies, and like execution schedule. 
 3:12: For example, like if the pipeline needed a particular business date or like environment, we could pass those values as, you know, as a job parameters and for the pipeline orchestration, like we could trigger database job from like a job data factory depending on the architecture. 
 3:29: Yeah, and like the ADF pipeline would I like, you know, handle the illustration like the database activity would start the required notebook or like job with the parameters and like inside, yeah. 
 3:42: Yeah, that's good actually. 
 3:44: Yeah, that's good actually. 
 3:46: so how many years of, experience do you have in general? 
 3:51: Yeah, like more than 7 years. 
 3:54: OK, OK, OK, so can you please quickly, explain me how the Django works and what, how the request and the response flow works in the Django architecture? 
 4:06: Yeah, sure. 
 4:07: So if I talk about like the request flow of in Django, inside Django, like, you know, when a client like a certain application or like another service sends an HTTP request, like it first comes into a Django web server. 
 4:21: And like middleware layer and like middleware can handle things like authentication, security, and like logging, logging goes or like request related processing and like after that Django uses a URL configuration or like a URL dispatch I would say to match the, you know, incoming URL and the method to be to the appropriate view. 
 4:41: And after that, like then the request goes to the view and like, you know, in our application, especially the Django rest framework. 
 4:49: like the views usually an API view or like a view set. 
 4:54: like the view handles the request, validates the input, like calls that would be businesses or service layer. 
 5:00: And if the API needs data, the application, you know, contacts with the database through Django. 
 5:07: For example, you know, if we might query positive SQL for false information and like if we have frequently requested data, we can also check like where it is before, you know, go into the database. 
 5:18: So yeah, once the late logic is completed, the view creates the response and like with the Django is framework, you know, we typically serialize the data intuition and like we return the STT response. 
 5:27: So yeah, this is the architecture for the. 
 5:32: So how we can create the multiple database connection in the Django and how we handle the migration and the migrate command so. 
 5:42: OK, like, so talking about, in general how we create, how we can configure multiple databases, like we can configure multiple databases in like, database setting in settings. 
 5:52: Pwi Fi, for example, like in one of my projects, like we had application database in Post Basel, but you know, some reporting data was like maintained in separate database, and yeah, like we configured both databases with different lysis, for example, default for transaction database and like reporting for reporting databases. 
 6:12: And yeah, then depending on the requirement we can you know explicitly tell Django like which database to use with like you know using method for example, you know, normal application transactions would use a default database. 
 6:27: Which reporting to queries would use the reporting databases also and if I talk about for the larger application I would normally use a database router for that yeah. 
 6:40: OK. 
 6:41: So OK, but my question is how you handle the migration and migrate commands, yeah, as, as I said, you will use the data bit routers, but how it's work. 
 6:54: OK, so like, talking about, how they handle that. 
 6:57: So yeah, like with multiple databases, migrations need to be handled carefully because, you know, Django migrations are like not automatically applied to every database in the way, you know, we may expect. 
 7:08: And like in my project, like we use a database router to control which models are, you know, allowed to migrate to which database. 
 7:15: And yeah, like the important method is like allow migrate, for example, suppose like we have two databases, you know, and like default for transactional data and like, I would say reporting for reporting data and if I have a customer model and know that belongs to the transaction database, so like my router can return through for that model and like default database and falls for, you know, that reporting database, then we can, you know, I run the mic migration command. 
 7:43: And yeah, like I specify the database using database option. 
 7:47: For example, you know, like, if I can write it in a, you know, a single line we can write a Python manager PY migrate database it's going to default, so yeah. 
 7:59: Delta's, oh sorry, hyphen hyphen database is equals to database that is. 
 8:07: OK. 
 8:09: OK. 
 8:09: So how you, Handle the query optimization in Django. 
 8:15: Yeah, like, courier automation is one of the, I would say, like, important things. 
 8:20: So like we would consider of, in my real projects, courier automation was important, because, because like some of our APIs are dealing with large data sets and like we had performance requirements, for example, like in, Django rest API like we have an endpoint that was returning a customer and like transaction information. 
 8:40: And yeah, like initially the API was making multiple database queries because, you know, we were processing, we are accessing related objects inside the loop. 
 8:48: And yeah, like we identify that by looking at Django debug toolbox and like our application, logs I would say mostly and yeah, like after that like we optimize it using Django ORM features, like one of the features that I don't even aware of is like a select related like for for foreign you know like 1 to 1 relationships. 
 9:08: And yeah, the other one would be like preface related for many to many and like reverse relationships, yeah, like this helps us avoid end plus one query problems and like we also avoid sorry to interrupt you, no agenda, What is the N+1 problem? 
 9:28: OK, so like N +1 problem is, mostly, it happens when we make our own database query, or, you know, to get a list of records, if then accidentally make an additional query for each recorded by processing that list. 
 9:43: But Django follows the lazy loading, right? 
 9:45: Whenever Django needs a database, data only at that time, only Django. 
 9:53: Means fake the data from the database. 
 9:57: So What is the exact N + 1 problem? 
 10:01: How the Francis is included in that? 
 10:05: So, can you please elaborate? 
 10:07: Yeah, like, you correctly said, like, yeah, the Django query sets are lazy, like, so simply creating a query set doesn't like immediately hit the database. 
 10:16: Django hasn't, I feel like Django hasn't necessarily executed the SPL yet, but the query is executed when the query set is evaluated. 
 10:24: For example, like, when I, I tweet a word, convert it to a list, I go, like call a len method, like it checks its truth value in certain cases or like otherwise, you know, request the results. 
 10:37: But like the, I would say the important thing is like the lazy loading doesn't automatically prevent the unpleasant problem. 
 10:43: for example, like if I fit like 100 policies and like then inside a loop across a related customer. 
 10:50: The initial query set is lazy, but like I would say like accessing policy.custom like can trigger additional database queries, and like if, if that relationship hasn't already been loaded, that's where the M+1 problem typically can happen, yeah. 
 11:07: Yes. 
 11:08: OK. 
 11:10: And have you work on the gender is frame up? 
 11:14: Yeah, I have looked them up. 
 11:17: OK, so, what is the flow to create a dangerous framework application? 
 11:25: How do you handle the APIs? 
 11:27: OK, so talking about the flow, yeah, the way I, I usually approach it, first we define the model and data structure, depending on, you know, what the API needs, and like when we create a serializer. 
 11:42: And like if I need to create a API, I usually start by defining the model, as I said, and depending on what data the API needs to work with. 
 11:50: And yeah, like then I create a serializer which is responsible for converting general model objects into like Jason and you know, like also validating incoming request data and like after that I would create like a API view I'd say, yeah, like depending on the requirement I might use an API view or like a generic views or like a view set and yeah, so like the view handles the request cause that will be business or the server logic. 
 12:17: And it interacts with the database and like prepares at last the PPOs the response. 
 12:22: So yeah, yeah. 
 12:25: What do you think it will work? 
 12:29: Sorry for what? 
 12:30: Because of what do you think? 
 12:32: Whatever you're saying that he will create the models levelizer than the, few steps. 
 12:38: What do you think it will work without, Django settings? 
 12:44: like without Django sitting, I don't think it would work. 
 12:49: Yeah, that, so because of that you need the jangle springer setting for before the creation of modern setting as an holistic site. 
 12:57: But yeah. 
 13:01: OK. 
 13:02: So, OK, let me lodge in there. 
 13:08: Sorry here the difficulty of pronounce, so I'll, I'll pronounce it. 
 13:11: OK, I have, the standard code, so it's important. 
 13:18: So, Apara will continue with you and further than my feedback. 
 13:22: I will share my feedback with the Aara and the chat also. 
 13:26: So do you have any questions for me right now? 
 13:30: Like, no, right now I, I, if I would be having some questions, I will be asking you later. 
 13:35: OK, yeah, you can ask those questions to offer also, definitely after all, or the HR will answer your question definitely. 
 13:43: So yeah, Aer I will continue this call and sorry for this and let's check, yeah, you. 
 13:53: Yeah, and it's, I take it for dinner. 
 13:57: I love this dinner and Yes, I think. 
 14:03: Oh Elogen, OK. 
 14:09: So you got 2 years of expenses 11 years, yeah, OK, so. 
 14:16: How we can handle, we have the, millions of the records in data table, so we have to show that, data to PO I means or we can show we, we can handle that millions of people. 
 14:31: OK, so, like, about, like how we can handle like, millions of data and like millions of records we have millions of recording data table basically Beijing from delta table, and to show to me is that we do APIs correct, correct. 
 14:48: So like the first thing that I would consider of is like I would not directly, you know, load all the records into the API response because like I think that would create, you know, major performance and like memory issue I would say. 
 15:00: And yeah, like in one of my data base on projects like we had a very large, data effects coming from like multiple enterprise sources and so we are, we, you know, followed a similar approach. 
 15:11: The first thing that I would do is like I would expose the data through an API with paging nation. 
 15:16: That is one of the important concepts. 
 15:18: And yeah, like the client would request something like, I would say like page size 100 or like a page size 500 instead of requesting like millions of records at once. 
 15:28: And like I would also make sure that like query is like filtered at the data layer before returning the results. 
 15:35: And for example, if the user is looking for a transaction for a particular customer and data range, like, I would typically push those like filters down to the data query rather than, you know, like returning the entire table and like filtering in Python. 
 15:50: And for a very large data sets like I would prefer a key set and like I would say a cursor based pagination instead of, you know, like traditional offset pagination. 
 15:59: And for example, you know, instead of like saying offset one leg like we can use a stable column such as an ID or a time stamp or and like request recalls. 
 16:10: So yeah, I apologize for it. 
 16:16: Cursor reports. 
 16:16: OK, so that how that cursor records means, yeah, so like cursor because just now you would work like this image, you know, if, if we have like cursor this pageation basically means like we can, you know, use a stable position or a key, from the last report we returned instead of, you know, like saying skip the first, like one like records, for example, yeah. 
 16:40: OK, got it. 
 16:41: Also, your work on any data streaming your APIs. 
 16:48: Yeah, I have worked on it. 
 16:52: so how we can, Actually it means what methods we are basically use for that streaming. 
 16:59: OK, except for data streaming APIs like, the methods that we can use is basically if you know if you're asking specifically about the methods or mechanisms we have used for streaming mechanism, yeah, so like, For a Django or a DRF API, if we are streaming a large STTP response, we can like use, I could, I could remember of like stream light STTP response and like Python generator, yeah, you know, because, because the like the generator leads or produces the data implemented, yeah. 
 17:33: OK, so how that generators works, yeah, but like, as I said, like the generator deletes or producers data like a basically a way of like producing data one item at a time, I'd say, and like instead of, you know, creating the entire data set in a memory at once, and the key thing about this is like we can, we can use yield keyword instead of like return, and yeah, like when I call this function for Python doesn't execute the whole loop immediately like it returns a generated object. 
 18:01: So yeah, this is how it works. 
 18:05: OK. 
 18:07: So, which method we use in generator, basically? 
 18:12: OK, so we can use, we have multiple methods. 
 18:15: We can use iterated method also, but like, we, as I said, like we use streamlined STT response with the generator. 
 18:25: And like yeah the specific method would be like yield yield method that and I I think we can also use iterator method if we have a query set we can use like query set. 
 18:37: iterator method. 
 18:40: OK, What are the basic, yeah, like the basic security, in general for API, yeah, like first is the authentication I would say like we need to verify who's, who's calling the API basically, depending on the architecture that could be like system authentication or I can say like token based authentication like we can use data bogan and like or 2 or like OIDC based on like identity. 
 19:10: Provider and then after that we have authorization, which is, you know, like really important. 
 19:16: And yeah, like it tells it, you know, it tells us who the user is while permissions determine like what the user is actually allowed to access. 
 19:25: OK And like we, we can also use SCTP and TLS, so like credentials and API data are, you know, transmitted in plain text. 
 19:36: yeah ok so basically authorization authentication ok so So you worked on the session-based and token-based authentication right. 
 19:52: So in this session, generally we, it's, create on the server side. 
 19:58: So if we have the, multiple servers and, server basically user has connected to one server and it's disconnected in between. 
 20:07: So how we can handle that situation basically. 
 20:10: Is there any way to maintain that obsessions? 
 20:16: yeah, like if we talk about like multiple servers. 
 20:21: yeah, like with, I, I would say like, yeah, I would say like with traditional session-based authentication, the session information, you know, can be stored in server side like so if we have multiple Django servers and a load balance as you said like. 
 20:36: So like we have to make sure that user system you know is available regardless of which server is the next and like in a real production setup I would like avoid keeping the session, you know, like only in memory of an individual Django server. 
 20:50: Instead, like, we can use a shared fusion packet such as like a ready or a database. 
 20:55: , like, I would like to give you an example. 
 20:59: suppose like we have a server 1, server 2, and server 3 behind a load balance, and like the user loop loops into like server 1 and like the Django que is a session. 
 21:09: like the session data is stored in Reddis. 
 21:12: If server goes down, the next request is allowed to do a server 2, and like server 2 can use the session ID from the client's cookie. 
 21:20: I like to try the same session from Reddis. 
 21:22: So yeah, yeah, yeah. 
 21:25: OK. 
 21:27: So basically the token, so you worked on how to or how that how to is work, yeah, OK, so like you were talking about how the R2 works, the mechanism, yeah, like I have, yeah, like I have worked with token-based like authentication, particularly JWT based authentication for the APIs and like the I have also worked in that, yeah, over 2, and like one small distinction between them is like over is mainly an authorization framework while like authentication is commonly handled through open ID connect on like top of I would say like over 2.0. 
 22:05: like, in a typical enterprise application, like the user first goes to an identity provider like as your AD or I'd say like another O or like OIDC provider. 
 22:15: And the application re that the user to like that provider or for authentication basically. 
 22:21: And like, once the user successfully authenticates and like this the required consent, the identity provider issues an authorization code back to, you know, back to the application. 
 22:31: And yeah, like the back end can, you know, then exchange the code for tokens and here the important token is like usually the access token, that we have the I have multipleton of the token that is the access token. 
 22:44: this is the application sent to the back end the API in the like authorization header. 
 22:49: Yeah, like the API evaluates the take typically, you know, it's a such a user audience inspiration, etc. 
 22:56: and I, I think that can also be a refresh token depending on the flow and the client type, yeah. 
 23:03: Yeah, so. 
 23:10: Over the ways to basically Authorize the user means so that how many methods basically we have. 
 23:19: like to authorize the user, like there are obviously there are so, several ways we can authorize the users, and yeah, like the right one depends on the application and, and I say like security requirements and the most common approach that I have worked with in Djangu's framework is like rule-based access or you can say like, I, yeah, for example, like we can have roles like admins, claim adjusters, or like regular user, and like each role gets, you know, different permissions. 
 23:48: Then we can use permission-based like or I would say like scope-based authorization like with OS or OIDC the the access token can contain scopes or claims and like the API checks whether the caller has the required scope before, you know, align, allowing the operation. 
 24:05: And yeah, like we can, we can also do object level authorization in there also, and this is important to enterprise applications because you know we having access to an API doesn't necessarily mean that like a user can access every record. 
 24:20: For example, you know, a claims user might be allowed to view only claims belonging to the assigned or, like organization origin, so yeah. 
 24:31: OK, the jungle. 
 24:38: So how that actual civilization has worked in the jungle means? 
 24:43: What's the use of that one? 
 24:45: Yeah, like serialization is one of the important concepts that we use and, like the if you talk about like the internal working of civilization in Django, so like for in Django application the user provides the username and password, example, you know, Django's authentication system verifies those credentials against or like configured user. 
 25:07: And the user database using its authentication back end and like if the credentials are valid, Django establishes the user's authenticated state, usually through a session. 
 25:17: And like after that work on each request then we can identify the logger and you know logged in user basically to a request. 
 25:23: user yeah and we can then use like Django commissions or groups or like custom permissions logic to control access. 
 25:32: Yeah, and if I talk about like, see like suppose like I have a policy-based model which feels like policy number, customer name, like the status, and I'll say like effective state, then I can create a DRF model serializer for that model. 
 25:49: And when a client sends a request, the serializer converts the Django model, Django model instance into a, Jason friendly data, and then the DRF sends that back to the client. 
 26:02: So, yeah. 
 26:04: Those are the different types. 
 26:07: Is there any alternative way how to escape that civilization process? 
 26:15: Like the alternative way of civilization, like. 
 26:20: I say like there, you know, if, if alternatives to use a DRF CLizer, there are a few options and basically we have one is the basic we can use this civilization creating the classes and defining the models and the results, yeah, so like it basically depends on like what we are trying to achieve, for a simple API response we can build a Python dictionary manually and it will run it using DRS response. 
 26:47: For example, if I need 2 on, 2 or 3 fields, I don't necessarily need a full model CRI, you know, like, yeah, we can also use Django's Jason response for like, simple Django's in point, although, you know, for a full recipe I generally prefer DRF because, you know, like we get validation authentication, yeah, authentication. 
 27:09: I see. 
 27:12: OK, Civilization, so that's going on. 
 27:23: To to Oh So, basically how we can use the caching in the jungle. 
 27:37: OK, so like again caching is one of the important concepts that we use to like so frequently use data and in Django, like I have used caching to produce like repeated database calls and like improve API response time. 
 27:50: For example, in one of my APIs we had like the reference data that didn't change like frequently, but you know that was requested very often. 
 27:58: And like things like the status status schools and like look up values or like configuration data and like instead of going for SQL every time an API request came in we stored that data data in Radies for like in order to maintain caching and in Django we can, you know, use Django's venting cache framework with like I would say Reddi as a back end. 
 28:20: And yeah, like we can cache an entire view or like API response or specific data or like low level cache operations depending on obviously the requirements. 
 28:31: OK, so you worked on only reduced one or any other caching mechanism? 
 28:38: Like I have family worked with Reddi, but, it has been my family caching solution, but I have, I'm also familiar with Jango's cashwork. 
 28:48: Like, yeah, Django's cat, I remember like 37 like meat. 
 28:54: And. 
 28:59: OK, so how would that, Django Wars works basically. 
 29:03: Alex, Django's ORM, RM that stands for like objectation mapping, Django's RM is like basically the layer that lets us us like interact with the database using Python objects. 
 29:16: And like query sets instead of you know writing like SQL for every operation, for example, if like I have a policy model like I can write like I can write policy data about objects and like we can apply like a filter method where we can write a status whether it is active or like whatever and yeah like Django CRM translates that into an like appropriate escape query and like sends it to the configure database such as like post ques you can see. 
 29:42: And like one important thing is that like query sets are lazy. 
 29:45: So when I like create the query set like Django, you know, doesn't immediately execute their skill so yeah. 
 29:54: So, can we ride the raw queries, directly and go or? 
 30:00: So yeah, like in Jan like Django supports a like you know when the ORM is not the best fit return right like that. 
 30:12: OK. 
0:05: So your risk framework other than Django, which framework you worked, like I have worked on flask and yeah, flask and fast APL. 
 0:19: OK, how that the microservices architecture works, yeah, like microservices is, like one of the important, like the architecture in which like we devise and our application in multiple modules and like in my recent projects we use microservices to like break a large application into like a smaller and like independently deployable services like we are each service like was responsible for a specific business capability. 
 0:46: For example, like in a healthcare modernization project, instead of like having one large application handling everything, we could like have separate services like I would say a patient service or like a provider service or like claim service. 
 0:59: And like each service owns its own business logic and like ideally I say its own data and if the patient service needs information from the provider service they communicate through an API, you know, like rather than directly accessing the provider's service database and for in there like for synchronous communication we use rest APIs, for example, you know, fast API services communicating like over STTP. 
 1:24: And for asynchronous corporations we can use like event or particularly I would say a message broker such as in Taf car. 
 1:31: So yeah, these are the things that we can do. 
 1:35: Yeah, OK, basically we accessing the others we have the new one user service and the other one. 
 1:44: System service and other service so how we can basically access that one service in the hour. 
 1:52: like, if one service is trying to call another service in a microservices architecture, it needs to access another service and like we normally don't directly access the services database. 
 2:04: instead, like we communicate through its API or like, say, like messaging interface, for example, let's say like we have a user service and like policy service. 
 2:14: And if the user service needs policy information, it can like call an endpoint exposed by the policy service or something like I'll say I get a get endpoint. 
 2:25: And yeah, like for internal service to service communication, like we would typically, you know, use this to HTTP depending on the architecture and like, yeah, we could also use like G DRPC or like asynchronous messaging such as like Kasa. 
 2:42: OK, all right, yeah, OK, what are the response scores basically and who we have in the rest areas, like we have multiple response codes and like we have like, SCTP codes like we have 500, 400, 4, 200, OK. 
 2:59: If I talk about like them like we have 200 OK for like the it tells us that the request was successful or not 2001 created a new resource like resource was successfully created typically after a post like we have 4 400 that is a bad request. 
 3:15: And we have 401 unauthorized. 
 3:19: like we have also 1234, like we have multiple requests. 
 3:25: basically in that 400 request, that, yeah, like 400 requests is basically, bad request, and the request is still invalid, such as like, missing or like invalid input. 
 3:38: So like if we provide an invalid or we didn't provide any input, so like it returns us, good run a bad request. 
 3:48: OK. 
 3:50: Oh, Good. 
 3:53: So I we can go to some Python questions. 
 3:56: So basically, what are the magic methods we have in the Python? 
 4:01: the magic methods in Python like. 
 4:05: that I can remember of is like one thing, one method I can remember of is like, init method and like FTR method, len method, and yeah, these are the three methods that I can remember of. 
 4:20: OK. 
 4:23: Yeah, OK, Loiner, so you still said you also worked on the school, right? 
 4:28: Yeah, I have worked on the. 
 4:32: OK, so how that, indexing works basically, like indexing, yeah, so indexing we use for faster lookups and like, say about, index, it is a separate data structure that you know that the database maintains to make data travel faster and instead of scanning the entire table like, to find matching because the database database can you know be like use index to locate the relevant rows much more efficiently. 
 4:59: So yeah, this is my thing. 
 5:03: any drawback to use that tendency? 
 5:07: like, like if I talk about drawbacks of using indexing, definitely, like, you know, it has some drawbacks, and the biggest one is like it, you know, that indexes consume additional storage and you know that can slow down your like right operations. 
 5:23: Yeah, adoptation also insertation writing, yeah, insert or daily transaction, that can be, yeah, daily transaction that will always check the of that index is the uni one or, OK, So, what are the types of joints we have? 
 5:44: Like we have multiple types of joints. 
 5:45: We have like outer joint, inner joint, left joint, right joint, left outer joint, and like it's a type of right joint only. 
 5:53: we have cross joint. 
 5:55: we have like self-joint. 
 5:56: So yeah, these are the multiple types of joints that we have. 
 5:59: That's good. 
 6:02: OK. 
 6:06: So, in Pie Park you worked on, merging that, end up and something operations, yeah, I have opened. 
 6:18: And that works basically means what are the Mechanism behind that one. 
 6:23: OK, so, like, yeah, like I have a, for large scale data processing including like appendant noise, or like, salt patterns, particularly when you're not working with data tables. 
 6:36: You know, we work, we use this particularly working with data tables only, and for example, if in one of my data platform projects like we were, you know, receiving incremental data from school systems. 
 6:47: And like new records needed to be appended while, you know, existing records need to be updated based on like business key I would say. 
 6:54: And for a for a simple app scenario like we can use a data frame right with append mode. 
 7:01: Using like DF. 
 7:02: right. 
 7:03: format, this is the like syntax that we follow, but like when we need both inserts and updates, are you typically use our delta lake merge operation, for example, you know, like if, if we have a customer ID and that is a business key, then we can match the incoming records against that, against the existing delta table. 
 7:23: Yeah. 
 7:25: OK, so you have worked on any front end, site? 
 7:31: Yeah, I have worked, I worked on like front and frame books, with front and frames like react and angle, sorry, reactor and like le. 
 7:39: Back then I, OK. 
 7:42: Good one then, yeah, or. 
 7:47: What are the hooks in the reactor basically? 
 7:50: OK, so like hooks in reactors are, basically like, you know, there are functions that are introduced in react that allow like functional components to use state and like other reactor features without needing class components. 
 8:04: And like like I have mainly used hooks such as like one of the hooks that I have used is like use state and like use effect and like use memo and yeah I also use a use callback and use context. 
 8:17: These are the hooks that I have used. 
 8:20: Oh, OK. 
 8:24: so we can maintain the user data basically. 
 8:28: So for maintaining the user state, like it depends like on what kind of user state we need to maintain. 
 8:35: And like we have to maintain the logged in user information and like authentication status and I'd say permissions across multiple components and for local component state like I would use a use state and but like for user information that needs to be accessed across many components I would typically use a shared state approach such as like a context API or like I can use readers there or like another state management library yeah. 
 9:03: Yeah. 
 9:05: OK, fine. 
 9:05: So you work, on the Azure side, which means basically which cloud we you worked on. 
 9:11: Yeah, I have worked on the other side and like the cloud that I have used is like like Azure and Abas both. 
 9:18: I worked both on like Azure and AWS. 
 9:22: OK, so, Zul side, which, services you mainly work with. 
 9:27: OK, so now on your side, the services that I have worked with is like, I worked with, in the AKS Azure Services, and like, yeah, correct, and like Azure data breaks, I have also worked with Azure storage and like Azure monitoring and application logging, services, yeah, like I also did the, mainly worked with Daracom. 
 9:52: A of. 
 9:54: so he worked on, Gita action something creating image, yeah. 
 10:04: OK. 
 10:04: Oh, OK, fine. 
 10:07: So if you have any questions, so you can ask me, so we can close. 
 10:11: Yeah, like, like, I first, I wanted, like I wanted, wanted to ask like what will, what would be the like major roles and responsibilities if I will be hired for this role. 
 10:23: Majorly rules on responsibility, you will work on the cross, functional teams basically. 
 10:30: And the role is like little only that and the communication communi you have to communicate with directly stakeholders and have linked on-site operations basically at all things. 
 10:45: Yeah, that, that, that works well. 
 10:47: I have been into this kind of scenarios as well in my previous projects. 
 10:53: Like more, yeah, more you can get, yeah, so and like, the last question that I have like what would be like what are the number of rounds that I would be having for the. 
 11:06: Yeah, might be this is 1 1st 1 and the 2nd, directly with client round that will be OK, OK, yeah, that perfectly works. 
 11:15: Yeah, and if there is any more required, so it's basically communicate with you the wrong way. 
 11:24: OK, yeah, like, thank you for, thank you so much for the time and have a good day. 
 11:31: Yeah, bye-bye. 
