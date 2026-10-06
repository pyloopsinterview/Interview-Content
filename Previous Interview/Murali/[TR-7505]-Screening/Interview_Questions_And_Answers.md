0:00: How are you? 
 0:02: I'm fine, Marie. 
 0:03: How are you? 
 0:04: Am I audible? 
 0:07: Yes, yes, you. 
 0:09: You start to. 
 0:14: I'm starting the recording, OK. 
 0:25: OK. 
 0:25: Yes, doctor. 
 0:27: So, yeah, OK. 
 0:31: So hi, morning, I'm Sharon. 
 0:34: I'm working as a senior, technical lead in the SCL. 
 0:38: I'm having almost 9 years of experience and here, in the SMBC, right now I'm working, As the technical lead. 
 0:49: So, yeah, so quickly start with your introduction. 
 0:52: What kind of expertise do you have, right now, on this project? 
 0:56: What is your role and, you know, roles and responsibility for that project? 
 1:01: OK, OK, thanks, Charles. 
 1:03: So yeah, myself, Moley Mohan, and I'm almost 12 years of experience software developer, professional, and primarily my focus is on, Python backend development, Django, SCPI, develop, like microservices based on architecture, and like, cloud technologies and database management. 
 1:23: Management side. 
 1:23: So throughout my career, I have worked on like multiple domains including healthcare, insurance, finance, financial services, and real estate technologies like that, and we're like I have been involved in like designing and developing the or, or deploying all of those, applications, like on the enterprise scale, level and like mostly, and. 
 1:50: And most recently I have been, like, I'm working on with the company Lacos Mercy Health as a senior Python developer, like, I'm a lead here, in this role, like, I have been like responsible for building like a, a mod modernizing the backend applications using Python, Django, Django Res Restreamwork or like. 
 2:12: iWatch Cloud, Docker, Kuberities, SQL, Sful APIs like that, and my day to day responsibilities included, including like, developing the scalable back end services, creating, like secure APIs, implementing business logics, optimizing database performance. 
 2:31: I have also like worked up. 
 2:34: Extensively, extensively like, with like microservices architecture with like, the different business functionalities were like, developed as independently deployed and like deployable services to, you know, improve the scalability, reliability like that and also have exposure of Azure data breaks, delta leak, delta tables, passport concepts. 
 2:58: So this is the wholesome work I have done up to now and This is my experience in my current company. 
 3:06: OK, that's fine. 
 3:07: And, how many years of, to years of experience in, tango? 
 3:14: It's almost, almost going to be 10 years. 
 3:19: OK, dangle with the dangerous. 
 3:22: Almost like 8 to 9 years, yeah, so that is all and yeah as you said you mostly work on the Django and work with the microservices architecture so yeah, how we can, set up the multiple database, in the Django application and then after that how we can manage the migration and the migrate commands. 
 3:46: OK, absolutely. 
 3:48: So yeah, this is very standard use case we, we work on that side. 
 3:51: So like, we use like generalist framework with our multiser based architecture and like, we can configure like multiple databases inside the databases section of the like starting file and by default like, Django uses our database called default. 
 4:06: So but we can, you, we can define additional databases such as reporting data. 
 4:10: Bases, audit databases or like, any, any other databases belongs to, you know, different services, like each database will have like, its own connecting, connection setting like engine host, port or username password as we know that database name and all, and these are the major works like for example in my we can like, we can have a default. 
 4:34: Post re database for, you know, like transactional data and like another database for, you know, reporting or analytics and once the database are configured, Django needs to, you know, to know like, which models, should, should interact with which, database like that. 
 4:52: And for that we use a database router, a database, router, you know, contain. 
 4:58: Like, methods such as, DB4 read, like DB before write, allow, allow relation and like allow migrate. 
 5:07: So these are the method, methods help like Django decide to, you know, read data from like where to, write data and like. 
 5:15: Which models belongs to, you know, which database. 
 5:17: So these are the major. 
 5:23: Work I have done and that's how I will implement this whatever you I will do the optimization. 
 5:33: OK, so of course, query optimization is also a very important part of, I would say like, like I usually like, usually identify and plus one, Like I would say and +1 query problems, which like, like which are very common in Django like applications to solve data and, like I use, select related for foreign key and 1 to 1 relationships and also like, Pre prefats related or for for like many too many or reverse foreign key relationships like or also like these methods helps, you know, fetch the related data efficiency, efficiently like and reduce the number of database hits in that case and for that or or some other case like. 
 6:21: like, there are some important techniques I would say like we're driving only like required fields instead of like, you know, loading the entire objects. 
 6:28: So I, I use like values, like a value list, only, and before wherever like appropriate, as per the use case, just reduce the amount of data, yeah. 
 6:43: OK. 
 6:43: What is the main difference between select related and related? 
 6:48: Sorry, can you come again? 
 6:51: Select what is the main difference between select related and prepage related? 
 6:56: OK, OK, so yeah, I would say like, select related is used for like, you know, foreign key and like, 1 to 1 to 1 field relationships like in, in it performs like SQL, SQL, join and fetch, fetch the related data in a single database query and. 
 7:18: here, like, and if I talk about the prefecture related, then it works like differently like I normally use that, for, for many to many and reverse, foreign key relationships although it can like it can be used for, you know, like other relationships like instead of doing, SQL join like Django, you know, executes separate queries and column like and combines the, you know, results in Python and If like, for example, if I talk like if one author has like many books and I can use like author object not like prefix related, so Django is Django might execute one query for for authors and another query for, you know, for, for, for their books and, and then map those records together together in the memory. 
 8:07: So that this is the what basically differences in between the both. 
 8:16: Mhm. 
 8:17: OK, fine. 
 8:19: OK, hope we can connect the jango with the delivery. 
 8:23: OK, so yeah, of course, yeah, that, that is very standard process I would say, because, the most common approach I would say I use like, database provides SQL endpoints that can, you know, that can be accessed from a Django application by using like Python libraries such as like, data data breaks SQL connector, we configure data breaks host, SUDB path, and access token data and establish our like, secure connection and then execute ExQL queries directly. 
 8:54: from the Jangw service and another common approach is like using the rest APIs like, in enterprise environment data engineering teams often like use data breaks, processing like, jobs or data sets through the APIs. 
 9:08: So I think that is the major, I mean. 
 9:11: So I, I will call the, the database job, in the Django, OK, we can call like, database job in, in Django like, using the for repetitive, or like, scheduled jobs in Django like I, I typically, use celery or with like reds or, or, or you can. 
 9:31: I said take your job. 
 9:33: Sorry. 
 9:36: Database. 
 9:36: OK, OK. 
 9:38: So yeah, for database job like, OK, like, There are like situations where we, we need to, you know, trigger or monitor like like workflows like or like feature rather than like running that job directly inside Django so like. 
 9:56: For example, like in healthcare project like Django can trigger a database job through the databas S API, and, like database, you know, job can then process claims or member data in the lake house, perform like transformations using Price Park and write up. 
 10:20: What? 
 10:24: To call the job. 
 10:25: OK, to call the job parameters are needed. 
 10:28: OK, OK. 
 10:28: The main, main parameters would be like, database work workspace, URL, the job ID, and like the authentication token or like what credentials, yeah, that, that would be the nature. 
 10:43: And one more, that is very important. 
 10:49: And one more parameter is that is very important. 
 10:53: OK, 11 more, Like. 
 10:59: Parameters in like run configuration or task parameters, like basically like I, I'm, I'm warehouse ID warehouse ID is important out there, yeah, OK, OK, got your point. 
 11:11: OK, I'm just missing that, workspace URL and with that warehouse ID is also important. 
 11:17: With time to come with the database, yeah, of course. 
 11:25: OK, suppose, you have millions of records, right, almost 2-3 million of records, and, what is your best address to finish the millions of records from the database, OK, and then you have to send it back to the front end site. 
 11:40: So in between you have the JaPI. 
 11:43: So what is your best approach to fetch the millions of record and send it to front end? 
 11:53: OK, OK, my mom, I would say like, for this, like my first approach would be like, filter the data at like databa level and retrieve the like retrieve only the required columns in records and I would, like use consider that I will, sorry, I will add one more condition. 
 12:11: Consider that you have a 2-3 million records along with the 150 to 200 KDs. 
 12:18: It's 150 to 200 columns. 
 12:21: OK, OK, OK. 
 12:23: So I would say like if like if I have like 23 million records and at the same time, I would, the application is receiving like around 150K to 200 reads. 
 12:34: So then my focus would be on like like the scalability. 
 12:40: I would say, caching or like, query optimization and like minimizing the, database hits at that scale, and simply relying on the direct, database queries for every request would be like not sufficient I would say. 
 12:56: So I would first, make sure that the front end is like I will clarify, one more thing also, sorry, sorry to interrupt. 
 13:05: I will clarify one more thing. 
 13:07: You have to fetch complete results set, complete 2-3 million records. 
 13:12: Consider that 1 million sufficient. 
 13:14: Consider that you have to send complete 1 million record to the browser directly from Pen means from data bres to Django, Django to react. 
 13:25: What will be your best approach? 
 13:28: OK, step by step, OK, OK, OK, step by step, let me think, step by step, like, basically for this, I'm going to take, Like approach So it's like, if, if the requirement is that that I have to send like an entire 1 million, so, instead one like I would, execute the query in data bricks, and search the, data in like, chunks or batches for like example like 10,000 or 20,000 reports at a time. 
 14:01: And, like, yeah, as Django receives like each of, each batch from like, from, from, from like data breaks, I would immediately start sending the data to the client instead of like waiting for all like 1 million requests, to be fetched. 
 14:18: in Django, like I would use, streaming HTTP response for like similar, streaming mechanism and like this allows like, the server to, you know, continuously, stream data to the browser chunk but like chunk by chunk and. 
 14:33: Then I would enable the Zzip, like, com compression so that like the payload size is reduced during the network transfers for like larger for like very large data sets, you know, compression so that it can like, significantly improve the transmission time and after that like on the react side I would, I'm thinking like, I would process the like incoming data. 
 15:00: Like incrementally and rather than like, you know, waiting for the all full data sets to arrive and this, this helps, you know, avoid memory, like browser memory to you if like, issues like, and provides the better user experience in that case. 
 15:16: OK, Mary. 
 15:17: OK. 
 15:19: OK. 
 15:21: Yeah, I'm done with the question. 
 15:23: do you have any questions for me? 
 15:25: OK, yeah, like, I have a, may I know like, all about the Requirement or the for the work role this is and what kind of work is going to be. 
 15:37: This is the, we are looking for the Django developer, OK, who have a good experience with the Django and, mostly work on the back end side. 
 15:47: So right now we are developing an application in the micro content as well as the microservices at the back end site with the jango as per. 
 15:53: So we need in that area, and good developers. 
 15:57: So that's, that is a requirement and, you know, that's a project is, means that right now the project is on the banking project because we are, work for the bank. 
 16:06: So that we have the millions of records and you know that things you know so we have the data bit the the level we are getting the data from lake house and you know processing the data showing that the theI content side both both the structures are, you know, in the, you know, the one sector like the microt content and the microserlicor set I can say so different services we, we are creating so that kind of project and, you know, requirement right now we are looking for. 
 16:34: So yeah, totally clears my, I mean question like it sounds familiar sounds good, very, I mean sounds very, very much implementable and I have. 
 16:48: Yeah, as I say that, it sounds very familiar, so I have worked on such, things and earlier. 
 16:54: So yeah, looking forward to, move ahead. 
 16:56: Yeah, sure, yeah, yeah, OK. 
 17:03: May I know like, what, how many rounds is going to be there for this position or for this. 
 17:08: that, I think one client round is there, I think, but, HR will let you know. 
 17:15: This is totally not the first basic, technical grounds, I think manager or, any client round is there, then HR will let you know. 
 17:24: OK, OK, that's fine. 
 17:25: That's fine. 
 17:26: OK, thank you, thank you. 
 17:28: Thanks for your time. 
 17:30: Have a nice day then. 
 17:30: Bye-bye. 
 17:31: Bye-bye, shut up. 
