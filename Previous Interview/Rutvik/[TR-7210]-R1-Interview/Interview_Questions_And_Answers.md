0:00: OK. 
 0:04: Give me one minute. 
 0:06: I'll check where your panel is. 
 0:08: Mhm. 
 0:08: Yeah, sure. 
 0:09: No problems. 
 0:57: Yeah, how are you doing? 
 1:01: Sorry for being late a little bit. 
 1:03: No problem. 
 1:03: So yeah, how are you? 
 1:05: Give me a second. 
 1:06: Give me a second. 
 1:06: I'm good. 
 1:19: Sorry, I was stuck in a meeting Friday afternoon. 
 1:23: Sorry for that. 
 1:24: No, no problem. 
 1:25: OK, yeah, I, OK, let's, let me give a quick introduction. 
 1:31: So I have been working in IBM for from 2014 onwards. 
 1:36: currently my role is, solution architect, and, and this. 
 1:41: This account I have been working from 2020 onwards. 
 1:44: It's an EN in in a gen utility account. 
 1:48: And I, the current requirement is related. 
 1:55: As far as I know, it is ODB implementation, operational data bus, project that's going on. 
 2:04: And I think the, the, the, the position is mostly revolves around, integration areas, I believe so as far as I know, but we'll quickly discuss those things and gradually. 
 2:18: That's more or less to set the context. 
 2:22: do you want to go ahead with your introduction and what exciting stuff you are busy with lately? 
 2:26: Yeah, yeah, so like, hi, my, I'm, I'm Ruthvik, and like I have, I'm a senior Python engineer with around I'd say 2 experienced primary. 
 2:37: We like focusing on Python backend development, or APIs, microservices, and like, yeah, cloud native applications, and, like currently the most recent experience that I was working with Visient as a like lead Python and AIMLOs in platform engineer. 
 2:53: We were like my main responsibilities included like developing Python-based backend services and like APIs, working with APIs, working with PostSpare SQL, and I'll say like integrating data across like multiple enterprise systems and like, yeah, I also work with Kafka and Rabbit MQ for mostly like asynchronous, yeah, I would say asynchronous processing along with like Docker, GitHub and like HR services. 
 3:20: And like apart from development, like I am involved in technical design, performance optimization and products and troubleshoot, troubleshooting code reviews and like mentoring, you know, other engineers. 
 3:31: So yeah, like, yeah, so like one thing I really focus on is, I would say like building back end services that are like reliable and I would say scalable rather than, you know, just I would say like getting the functionality to work. 
 3:43: So yeah, OK, OK, so, Let me try to understand a little bit more about, the data volume and areas. 
 3:50: So your, current, current, Account whatever you're working on it is, on which domain is it, like automobile industry, which industry it is? 
 4:02: OK, so like this current project, so the domain of current project is like healthcare. 
 4:09: Healthcare. 
 4:09: OK. 
 4:10: And, What kind of data you are processing at this point? 
 4:15: Is it a streaming data or is it like you are pulling the data from the database, or what kind of data mostly you are processing at this point? 
 4:23: like it's a combination of both, I would say, like, you know, like portion of processing is event driven and like asynchronous rather than, you know, everything being real-time. 
 4:32: So, OK, combination of both. 
 4:35: OK, OK, and. 
 4:39: Exactly which area your application is play around? 
 4:42: Like, is it downstream application, upstream application integration area or is it a, I don't think it's ATL, right? 
 4:47: Your transformation is not your part. 
 4:48: No. 
 4:49: Yeah, OK. 
 4:50: OK. 
 4:51: so, which part do you, which part you are developing, like, yeah, go ahead. 
 4:56: Yeah, so let me. 
 4:57: Yeah, I am like mainly working on, I'd say back end services that, you know, that sit in the middle of overall integration flow. 
 5:04: So, like, you know, I wouldn't class, See why it has, you know, purely up stream or like purely downstream like we have like data coming from different enterprise systems and like our Python micros Python services basically they consume that data and like apply validation and business rules, yeah, like transform it into, you know, the format required by the downstream systems and you know then like either persisted in like post SQL or like publish it through APIs or messaging so yeah. 
 5:33: OK, OK, so, and your, your base platform is, which cloud mostly, like we, I, I, I have worked mostly, on, I would say a job, being one of the, that has been one of the like main platforms that I have worked with. 
 5:49: OK, and when you say Azure, which component of Azure do you use most for deploying your application? 
 5:57: the specific components in the job, like I have worked with most closely with, like, I would say application hosting, quantization, and like deployment site, and like I have also worked with AKS. 
 6:10: yeah, like, for example, yeah, understood, and I can see your experience there over there, but I'm just trying to say, let's say you develop that application and you need to deploy that application in somewhere in Asia to run it, right? 
 6:21: Normally, which for your Python application, the one that exactly you're working on now, where you do deploy them. 
 6:30: Yeah, yeah, yeah, I. 
 6:34: Are your functions or maybe as your web service as well, which one do you prefer so like for the Python applications I'm working on now like we typically quantomize the application using Docker and like deploy it in AKS. 
 6:46: And like yeah so the flow is like fairly straightforward I would say like we developed the Python service run the unit test and yeah after that indication test only also and like build the docker image and like you know push that image into Azure container like container registry and from there on like we like our GitHubba CI or CICT pipeline I'd say that deploys the image into like appropriate AKS environment. 
 7:12: So yeah, OK, that's not your responsibility. 
 7:14: Up to, up to putting into the registry is your responsibility, is it? 
 7:17: Yeah, correct. 
 7:19: OK, OK, so, Let me give you a scenario, and you tell me if I'm going in the right direction or not. 
 7:29: So let's say we have a junior developer. 
 7:34: Some junior developers are working on, and we are working on a scenario, a project where we have. 
 7:40: 2 or 3 agents we are developing, OK. 
 7:44: So those guys who are working junior developers, they don't know much about Azure or cloud-based environment, distributed environment. 
 7:54: We told, told them to develop, some agents and calling some backend APIs, Azure APIs, GPTs, and all those stuff and do some stuff. 
 8:05: So what they have done, we have 3 agents to be developed, so they, what they have done is, they have developed that agents in streamle. 
 8:14: OK, yeah, got it. 
 8:17: You know hosting this, right? 
 8:18: Yeah, OK, OK. 
 8:20: Now I need to take that application, make it enterprise grade, OK, and deploy it into the server, you, basically, OK, fair enough, yeah, so. 
 8:36: The agents work in a way that The first agents had some processing, and it's like a flow. 
 8:48: So first agent process something, it gets some output. 
 8:51: That output needs to be used in the second agent, and the that will be processed. 
 8:57: In addition to that, there will be some additional process. 
 9:00: And then the 3 agent, something like that. 
 9:03: So it's working fine in stimulant. 
 9:05: OK. 
 9:06: Because in one flow, like always, it goes in one flow. 
 9:08: -hum. 
 9:09: Now we have to move that to, as I mentioned, like containerized approach or anything you want. 
 9:17: -hum. 
 9:18: You tell me first. 
 9:20: I'm John Enrico. 
 9:21: I mean, I'll, I would like to request you, what would be the approach? 
 9:26: How we can, what do you think? 
 9:28: How from, from stream lift, where should I put it? 
 9:34: OK, so yeah, that was like quite a good question. 
 9:38: So I was like, give me some time to think. 
 9:41: Yeah, we are, we are, we are discussing together. 
 9:43: It's not an interview. 
 9:44: We are two friends. 
 9:45: We are just discussing that what is the best time, yeah, yeah. 
 9:50: so, like, I would say the, firstly, first and foremost, like I, what I would do is like I'll first separate, you know, the agent logic from the stringly TUI. 
 10:01: Because I feel like I wouldn't want stream it itself to like become the enterprise back end, correct. 
 10:06: And like if the prototype is like already working, like in that case I would preserve that business logic, you know, but refactor that into like independent testable Python services or I'd say like modules. 
 10:19: And for the particular flow that we can have, like, I think this offer it has like, if we will have an agent 1, we will have an agent 2, and we will have an agent 3, correct. 
 10:30: So with like a well defined contract between each step, the output from like agent 1 like becomes the input to agent 2 and like so on. 
 10:39: And yeah, like depending on how long running or like resource intensive these agents are, like, I would avoid, you know, keeping the entire flow inside like one asynchronous synchronous, sorry. 
 10:52: So yeah, like for the enterprise deployment, like I would compromise the application using Docker. 
 10:58: Like that is the most basic approach. 
 10:59: That's, yeah, OK. 
 11:02: I like before going to Docker, as you mentioned, sorry I interrupt you, as you mentioned that you are not going to use streamlet. 
 11:07: That's not a good idea, which you're 100% correct. 
 11:10: Instead of streamlet, what you will use? 
 11:12: OK, so like an alternative to streamlet, I will basically, I will use like. 
 11:18: See, I won't use streaming because it can still be like I would say I, I would say like, yeah, I, I wouldn't necessarily remove streamle completely because you know like it can still be useful as a UI or let's say like internal demo like what are you not internal demo. 
 11:34: I'm going for a production gate application now. 
 11:37: OK. 
 11:39: Like for a production grade application, the alternative of like using streamlet. 
 11:45: And we are, we are going to develop those are acts those agents will act as an API. 
 11:53: OK, so like, you would, in that case, like I would like use or type script or like react for the front end instead of streaming like on the back end, yeah, on the back end obviously I use Python or FastP for the API, you know, and the agent services, yeah, OK, OK. 
 12:11: OK, so we'll go to the contrast gradually. 
 12:14: So once we go into fast FBI. 
 12:17: And implement all the logics into fast API. 
 12:22: And then, as you mentioned, we deployed into a Container environment, whatever it is, it may be may be a simple, as your function or maybe an a case or whatever you want. 
 12:36: But a scalable function, scalable environment where new container will be created whenever there is load, loss of load and all that stuff, right. 
 12:44: And what these junior developers has done, they have lifted and shifted into the new environment. 
 12:51: They learned that Python environment, new API, what, how it is going to be used, and they deployed it. 
 12:59: What problem, what first problem they might face, do you think, if we try to run it? 
 13:06: Yeah, so like if I try to run it, like in this scenario, the first thing that I would look at is like, yeah, I would check like whether the application is stateless or stateful. 
 13:17: This is the first thing that I would look, like if like if everything is running in one application flow, so the developers, like they may be relying on like on in like in memory state or I'd say like local variables to pass the output from like agent 1 to agent 2 and like, you know, content like agent 3 forward. 
 13:35: And they're using in memory. 
 13:36: Let's say they are using in memory, yeah, if they are using in, sorry, sorry, could you come again in memory states? 
 13:43: Yeah, they're using in memory state. 
 13:44: Yeah, so like why are you using in memory state like by in memory state like I mean, you know, if agent one stores its output in a Python variable object or like a stream session state, then you know, agent to expects to access that same variable again and like that work when you know everything is running in the same process or a container. 
 14:03: But like once we deploy like multiple containers and I'd say scale it horizontally, then like then in that case like let's say agent one could run in container A and at the same time you're like you know, agent 2 runs in container B and at the same time container B won't have access to like container A's memory. 
 14:22: So yeah, like so that state would be lost or I would say unavailable in that scenario. 
 14:26: So how, how we can redesign that in that case. 
 14:29: Yeah, so like in that case for redesigning it, like we can redesign it this like as you correctly mentioned exactly to the point you, you was told the exact error that they will face now we have to solve it. 
 14:43: We have to solve it somehow, so we have to do some changes somewhere, right? 
 14:47: What can you suggest? 
 14:49: So like we can redesign that part of like. 
 14:53: The, the main things that I would suggest is to like remove the dependency on like in memory state, like redesign that agent workflow like, you know, so that that state is externalized. 
 15:04: let me give you an example. 
 15:05: Like instead of like agent one storing its output in a Python or like streaming variable and agent two reading that variable, so I would, in that case, like, yeah, like I would introduce an orchestrator at, at that point. 
 15:19: Like agent one returns a structured response and like the orchestrator either passes that response directly to the agent 2 to it's, you know, obviously like API or like persists it in post a SQL with a workflow ID. 
 15:32: And yeah, like then afterwards then the agent to processes it and like sends its output back to the orchestrator that we have like introduced, right? 
 15:41: So basically what you're saying that yeah in such in in one I'm not going into details so that we could save this data into it somehow in the database and from the database we'll take it so we can do the same thing with blog storage also, right, something like that. 
 15:57: Which one is better approach? 
 15:58: So like blob storage or this one, like the approach that I have to do. 
 16:04: So yeah, I would say like blob storage is an option, no doubt, but like, you know, the choice mostly depends on like what we are storing. 
 16:12: If the agent output is structure is like I would say a structured decent workflow status or like you can say agent status or like time stamps, then like in that case I would prefer Post a SQL, you know, because like we can query and update that straight transactionally. 
 16:28: And on the other hand, if the agent produces a large artifact like a document or you can say a PDFs or like image or large large files, so like in that case, in that case particularly, like then I would use like a your blob storage so that like I could store the artifact in blob storage. 
 16:44: So yeah, OK, OK, so let's go to, let's shift the gear a little bit, so let's, let's think about, Your, let's get some idea about your experience related to streaming data processing. 
 16:59: OK, so now let me go to that dual requirement and give you some idea and we can discuss how you are comfortable with that. 
 17:06: OK. 
 17:07: So what We are planning to do in this project is So this is a large utility company. 
 17:16: So they, they have electric, gas, different utility taken care of. 
 17:20: They're taken care of, and they have, this requirement is from the electric side. 
 17:26: So on the electric side we have different kind of data sets like we have beta data. 
 17:35: We have electrical meters. 
 17:36: We have, distribution data. 
 17:38: We have, transmission data, lots of data points and different, different, devices. 
 17:44: Have you had any type of i vision and all those software by any chance? 
 17:50: So vision vision PI vision Aviva pai yeah yeah I got it I got it. 
 17:58: welcome, welcome. 
 17:59: You have some ideas, right? 
 18:02: OK, OK. 
 18:02: Have you worked with that? 
 18:04: like, no, like I would say like overall I have an idea, but I have not like had some experience. 
 18:10: Yeah, yeah, that's OK. 
 18:10: Yeah, yeah. 
 18:11: You don't need to exactly have, as long as you have some idea, that's OK. 
 18:14: So basically all those applications, also all those downstream applications and upstream applications all are together. 
 18:21: So now what we have, let's say we have all the applications in our left side, Sorry, I don't see myself in the camera. 
 18:31: What's going on? 
 18:32: You can see me, right? 
 18:33: Yeah, I can see you. 
 18:34: Like now, yeah, it went for a while and it again. 
 18:38: Oh yeah, yeah, that's OK. 
 18:39: Yeah. 
 18:40: So basically what I was saying is, let's say we have all this application from sensor data and everything coming from the left side, OK. 
 18:49: And in the right side we have a big data leak which is based on lake. 
 18:55: So far all these data are distributed or are scattered kind of. 
 19:00: So basically we have, IT datas. 
 19:04: We have OT datas, OK, all are coming into and. 
 19:09: Each application owner is integrating that in their own ways. 
 19:13: What we're trying to build now is a bridge between these two, a common bridge. 
 19:19: This common bridge will work, will, so basically, snowflake, what we're taking care of the snowflake part, they don't need to bother anything. 
 19:28: They'll connect it from the bus, OK, OK, like, ODB bus, correct. 
 19:34: What do you mean, yeah. 
 19:36: and IT and OT both will be publishing all the data in the bus itself, right? 
 19:42: So, that's the whole thing. 
 19:45: So have, have you got any kind of experience like that in your life? 
 19:49: Have you walked on service bus or any, any data bus project? 
 19:54: like, I, I, like I have experience, like I have, I would say like a little bit knowledge about that. 
 20:02: I have worked with mass and like even different architectures, although like I haven't worked specifically with like ODB implementation or like a utility environment. 
 20:11: OK, OK, OK. 
 20:14: That's OK. 
 20:14: ODB you haven't walked on, but any kind of azure in azure or any kind of, like So you have used, I think you have used, what you have mentioned. 
 20:23: I'm sorry, I haven't gone through your CV totally. 
 20:25: I've not, haven't got a chance for that. 
 20:27: So for the event-driven architecture or the streaming data processing, which, which tool you have used so far, which the technologies that, yeah, yeah. 
 20:39: So like for event driven and streaming style processing, like me, my main hands-on experiences has been like like Kafka and RabbitMQ. 
 20:48: yeah, like the is one of, one of the ideas that relate more closely to the streaming site. 
 20:52: See, I have worked with that, OK, yeah, OK, so can you give me some idea of, can you give me, explain me about the project a little bit, OK, and what is your role and how you use? 
 21:03: Yeah, sure. 
 21:04: So, like talking about the project, so yeah, let, let me give you an example from my current project that like we didn't, because, you know, like. 
 21:14: I would say the project is in a healthcare domain and like we, we, we have multiple enterprise systems, you know, that need to exchange and like process data. 
 21:22: So like my particular role is like a primary on a Python backend and integration site. 
 21:27: I developed this APIs and like back end services that receive data from like different systems, validate and transform it. 
 21:34: And for the event-driven part, specifically like we use Kafka and Rabbit MQ depending on, you know, like the use cases. 
 21:40: For example, like, you know, when a workflow, I'd say doesn't need to be completed synchronously. 
 21:46: Of one service pub like one service publishes a message on I would say like another service that consumes it independently like that helps us, you know, handling higher volumes and I'd say or like keeps the service loosely coupled and on the deployment side, like I containize Python services in Docker like as I previously mentioned, and like push the images to as our container registry mostly and yeah, like. 
 22:11: So like my role isn't just development. 
 22:14: I'm involved in like more technical design and like API integration design for that. 
 22:19: So in which case you, you prefer cough coffee? 
 22:22: Have you used IBM MQTT? 
 22:24: Sorry, like, could you come again, please? 
 22:26: IBM bus. 
 22:27: Have you? 
 22:28: No, like I have not worked with IBM. 
 22:32: OK, no problem. 
 22:34: so, for, this case, you have hands-on experience to work with, rabbit MQ or whatever you have mentioned, right? 
 22:44: OK. 
 22:46: OK, let me go through your works a little bit quickly. 
 22:51: If I see anything that I, do you have any questions for me? 
 22:56: yeah, like, I just want to know, like you have told me about like which, like this type of project that like we, we, you, you are working with. 
 23:05: So could you please tell me about like the rules and responsibilities I would be having like I would be hired. 
 23:10: Oh, OK, so basically this, I think this. 
 23:14: This particular project where we will be working on if you are selected, there are many different segments. 
 23:21: They have, ultimately this data is being processed and send it to our team who are working on forecasting, and short-term forecasting. 
 23:32: That's one of them. 
 23:33: I think there are more. 
 23:34: I am not directly involved on that team at this moment. 
 23:38: And, there are, so this ODB has a huge responsibility. 
 23:44: That's the project you are talking about. 
 23:45: I was involved in the initial design, now I'm not. 
 23:49: But that will be, that will be the, that will be the, Reach for all the data for the data for our electrical data into the data up. 
 24:01: So, it will, your responsibility will mainly for that. 
 24:06: Currently what you are doing mostly similar, the integration part of it, not the ETL or anything. 
 24:12: There is the other team to do that. 
 24:14: So integration and development, all those parts that I think mostly it's. 
 24:18: What you are doing now, but what I would suggest is, go through some case studies of ENU. 
 24:26: So you like it. 
 24:29: ENU means energy and in, and, implementation of how ODB can be implemented, what are the different case studies, how they have done, especially using Oracle ODB. 
 24:42: OK, yeah, noted, noted, yeah, OK, and, so with your experience you can quickly relate, right? 
 24:49: For example, you haven't done something, I can, I can, I can understand that, but That's pretty, we all haven't done, but you can, you can explain, OK, I haven't done this, but we can do it this way. 
 25:01: With your experience, you can easily, I believe, map that. 
 25:04: But you need to know what we are planning to do. 
 25:06: So you go through those studies a little bit before, because in the next, next one would be from the client side. 
 25:12: And they, They, the interview will be a little bit more tough in a way I would say so it's to be expected to be tough. 
 25:24: Yeah, that will be tough, and they don't want to be friendly or anything like that. 
 25:27: OK. 
 25:28: So, just, just want to make sure that you have a proper, study. 
 25:33: You will get some time in between these two, right? 
 25:35: So I believe, I'll give my feedback, but if they are, you are called for the next round, please be ready for those ENU. 
 25:42: You mention, you can mention that you have gone through this ENU case studies. 
 25:46: You have an idea. 
 25:48: They, they should feel that even if you don't. 
 25:51: Haven't worked on that industry. 
 25:53: You have an idea for this same kind of data, how to process those, yeah, yeah, OK, especially the, streaming data. 
 26:01: You have the experience a little bit. 
 26:03: I, I understand, but, for OTIT combination, how you can handle the bus. 
 26:10: OK, how you will design it, what are the challenges might be we'll be facing, how to solve those challenges, those kind of things from the Python perspective. 
 26:19: OK. 
 26:19: I think I am good for now. 
 26:22: OK. 
 26:23: So, you have done your reading in Los Angeles, your, your study in Los Angeles, I saw, right? 
 26:29: somewhere? 
 26:29: No, like. 
 26:30: You or somebody. 
 26:31: No, no, no. 
 26:32: OK, OK. 
 26:33: Somebody else. 
 26:33: I, I took 3 interviews today. 
 26:35: I probably messed up with somebody else, but anyway, thank you very much, and it's nice to meet with you. 
 26:40: I'll give my feedback and somebody might call you back. 
 26:42: Yeah, I like, it's, nice meeting you also. 
 26:45: I like, yeah, thank you so much for explaining the rules and responsibilities and like mostly about the project. 
 26:50: Yeah, yeah. 
 26:51: So I'm, I'm from my website. 
 26:53: It will be client site interview, so, but yeah, if you're selected, that will be the, that will be your role. 
 26:58: Yeah, that makes sense, yeah. 
 27:00: So, like, have a good day. 
 27:01: Thank you very much. 
 27:02: You too. 
 27:03: See you. 
 27:03: Have a good weekend. 
 27:04: Yeah, have a good weekend. 
