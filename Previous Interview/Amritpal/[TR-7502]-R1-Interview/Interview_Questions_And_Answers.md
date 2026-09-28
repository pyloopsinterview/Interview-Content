0:00: Hello. 
 0:02: Very good afternoon, everyone. 
 0:05: Hey, good afternoon, my lady. 
 0:07: Jackson, you can drop off. 
 0:09: OK, sir. 
 0:10: Thank you. 
 0:13: Oh, I'm good. 
 0:14: How are you, ma'am? 
 0:17: you're based on. 
 0:20: I'm in Laurel, Maryland. 
 0:24: Laurel, Maryland. 
 0:29: Which state? 
 0:30: Oh, Maryland. 
 0:32: Oh OK. 
 0:35: Or is it better? 
 0:38: I just. 
 0:44: Just give me one minute. 
 0:45: Let me pull up your list and yeah, take your time. 
 1:04: All right, so are you still working at the Wisconsin Department of Health? 
 1:08: Oh, no, no, no. 
 1:09: Last week like it ended. 
 1:14: OK, give me a little background about yourself and in 2 minutes and background and what kind of experience you bring on other other people. 
 1:22: So, like, I have over 13 years of experience in software engineering, like, primarily focus on python backend development, rest APIs, microservices, platform, and like the data, intensive applications and like. 
 1:37: and, like, like in Wisconsin department, I was the, principal Python developer. 
 1:43: Like, my responsibilities includes like, designing and developing the Python, back end services, using Fast API Django, and also like building the, rest. 
 1:55: working with FHile child healthcare data and also like developing the injections pipeline using Kafka and also like involve the with the AWS data breaks SQL CICD monitoring, logging and the production troubleshooting and, like, on our healthcare data platform, like, we received the clinical and the public health data like from the multiple source systems and like, I worked on the APS that evaluated and like normalized the incoming Jason SHS resources like, before publishing the events to Kafka and Kafka consumers then like. 
 2:34: , process the, those events, asynchronously and made the, the validated data available for the downstream analytics and the data breaks and, also, like, after, I also like worked on the front end like using React and Angular. 
 2:53: So yeah, like, my role is like combination of hands on like the path and development, the healthcare data, integrations, event-driven architectures, cloud deployments, and, the production reliability. 
 3:06: So, yeah, that's all. 
 3:09: OK. 
 3:11: So, no, good to know. 
 3:13: Thanks for that, and I'll just give you like a brief synopsis of this project. 
 3:19: Let me share my screen here. 
 3:20: There's one slide which I want you to take a screenshot of. 
 3:23: Yeah. 
 3:24: Let me know when you're able to see my screen. 
 3:27: Are you able to see my screen? 
 3:28: Yeah, it's visible. 
 3:31: OK, can you take a screenshot of this? 
 3:33: Just so that you have it for reference. 
 3:36: Just give me a second. 
 3:39: OK. 
 3:42: The Cool. 
 3:45: So this says I've got all the details. 
 3:47: Who's the customer? 
 3:48: What's the requirement? 
 3:50: what's the interview process, and what are some of the dos and don'ts in terms of coding test timelines and stuff like that, right? 
 3:57: So typically it follows in this process after we, screen today and then send your resume to the customer, there'll be a customer screening process if they like your thing. 
 4:06: So they'll send you a calendar invite to schedule that, and then after you clear that, there's gonna be a coding assessment link that you'll be receiving. 
 4:15: And you have to complete that in 72 hours and then if you clear that, then this would be probably an round of discussions with the customer. 
 4:22: OK, yeah, sounds good. 
 4:25: yeah, so this is about the customer, the role it's all like it will be a customer driven project, so they're into health care, value this case. 
 4:33: So as you know, so they are in the process of modernizing a lot of their, data stack, and this is one of a big project where, They are trying to modernize their clinical dataization process and to data breaks, using personal as the back end and they're looking for help for people like you who can, you know, come in and help them build it, on their end. 
 4:53: So it's gonna be a bit technically intensive. 
 4:57: The, the, I mean, they're, they're good people to work with. 
 4:59: It's just that they're. 
 5:01: A little too picky about the candidates they want to bring on board. 
 5:05: So, we prepared for some very deep technical discussions with them. 
 5:10: So that's the reason I want to kind of evaluate to see where you stand and, and then, we'll, we'll go from there, OK, yeah, got you. 
 5:23: Alright, so, OK, now given that you know, and then you know I set up some guidelines for what I'm expecting as part of this discussion, so, Now tell me, take an example within your current, any other questions before we move on? 
 5:42: Like any questions you have in terms of project? 
 5:45: I'm good, Morai, OK. 
 5:47: OK, good. 
 5:48: Alright, so take an example of your, I mean, all the work that you have done. 
 5:53: Take one or two solid examples where you're kind of designed, built, then up back end, integration using Python, what challenges you face, how you went about designing, what was the problem statement? 
 6:04: What was your contribution. 
 6:06: So I want to kind of share a very good story around 2 or 3 good use cases and try to explain to me as technically as possible from your end to kind of see. 
 6:14: no, I will see that, OK. 
 6:17: Absolutely. 
 6:17: Like, I remember like, one strong example like from, my current project is like the healthcare data injections platform. 
 6:24: Like yeah, like I worked on with the, discussion department of like the health services. 
 6:29: So basically, here, like the requirement was like to build a reliable back and indications like that could receive the clinical and the public health data like from the multi-source or multiple source systems and, validate and like, normalize that data so and like make it available like for the downstream analytics and the data breaks and here I was like primarily responsible for like the Python backend and the injection site like I design and like the develop the rest APIs. 
 6:59: using fast API and, at the API layer like we, validated the incoming JSON and the FHIR FHIR like the Skype legal resources, check the required fields, handle some, malform, payloads and apply like applied the, expected authentications and authorization pattern and See, like, for longer running, processing, we do not want the API request to wait. 
 7:28: So after validations like we Published an event to Kafka and the downstream consumers process the data as synchronously, so I worked on like the both producer and the consumer side logic, including, messages, civilizations, topic configurations, partition considerations, retries, and error handling, and. 
 7:54: Talking to her, like one of the biggest challenges was the transient failures like versus the duplicate processing. 
 8:00: So if a, if a downstream service like temporary failed, we needed to like, retry without the like, could like create duplicate records like. 
 8:11: Like I, I implemented control to try handling and the. 
 8:16: the, exceptions categorizations of like logging and failure or routing for the, non-reco recoverable messages and once like, process the data was like made available in the databas for analytics, like then, I also work with the SQL for like the, the data validations and joints indexes and troubleshooting and like the, production issues and in last like, like, from a production perspective, I was involved in like the, racing failures. 
 8:50: End to end like from like the APIs and the authentication layer like through the Kafka and the database processing and like to the like downstream platform so that combination of backend development, the event integration and production troubleshooting is like probably the most relevant thing like, from this one. 
 9:11: OK. 
 9:12: And from a design point of view, how did you go about doing all the design considerations like, OK, when you got the requirement, what were some of the key, things that you looked at before coming up with the recommendation? 
 9:25: Hm, generally, for, for like design perspective, like what I get as a requirement like this is like. 
 9:33: I don't start with the technology first. 
 9:35: Like I first try to understand the data flow, the business requirements, the expected volume, reliability requirements, and like what the downstream consumers need. 
 9:46: So, like for a healthcare engagement platform, the first thing I looked at, it was like the source, like system and the data contracts, like what type of clinical data like we are receiving, also. 
 10:00: We can say the JSO structure, mandatory fees, authentication requirements, and like how that the data like needed to transform for the downstream, use. 
 10:12: And the second consideration was, synchronous versus the asynchronous processing. 
 10:17: Like since some clinical data, processing like could be, long running, but I did not want. 
 10:25: The API to hold the client request open. 
 10:28: So we designed the API to like, validate the, like, the request and then publish an even to Kafka allowing the downstream consumers to like process it as seamlessly. 
 10:41: then I look at the reliability and like the failure scenarios like I, I especially consider considered like what happened if the Kafka is temporarily unavailable. 
 10:53: if a consumer fails halfway through the processing, Or like if the downstream database or the database processing has an issue, so that led us like the control retries, exceptions, categorizations, logging, and the failure routing. 
 11:14: OK. 
 11:14: And then what about scalability and performance? 
 11:18: Mhm, generally for scalability like including the ka part partitioning and keeping the AI layer stateless so like, we could scale it horizontally and like, yeah, also like I look, look at the both the API layer and the downstream injections pipeline because The bottlenecks can occur at the different stages like at the API layer, I kept the services stateless, so they like they could be horizontally scaled. 
 11:48: We use the, like, I told you earlier, like the fast API for the rest layer, and I focused on doing the lightweight valid validations like at the the API boundary rather than like keeping the request like open. 
 12:03: Like for the long run processing and for like the heavier processing, the key design, like the decision was using the Kafka asynchronously. 
 12:12: The, the API validates the incoming clinical payloads and, publishes an event, while, while consumers process the, data independently. 
 12:23: So that allows us to like scale the consumers based on. 
 12:28: Processing workload instead of like making the itself responsible for like everything and see. 
 12:35: Kafka partitioning was also an important consideration because it allows multiple consumers to process the messages in parallel, so we had to think about the partitioning strategy or like make sure like we were not creating unnecessary ordering or like the processing bottlenecks. 
 12:57: OK, OK, what about, things like lineage observability and all, have you worked on those kind of things? 
 13:04: Have you ever incorporated that in your design, like, like, see. 
 13:10: Observ was definitely an important part of like the healthcare injections platform like especially because we had multiple stages in the pipeline and needed to troubleshoot via like clinical data record field like on the observatory side I work with a structured application logging also we can say the exception handling and like the operational alerts like. 
 13:39: we wanted to, like, enough, information to raise a request or like, we can say events from the API layer to the cast and the downstream processing. 
 13:48: So like, then, some, something failed, I could determine like whether it was an API validation issue, issues, authentication problem, car processing issues, and, the, the database problems, like, for example, in this project, like if a clinical payload was accepted, by the API, but the letter like failed during the consumer, processing, so we needed, to. 
 14:17: correlate that the processing act activity with the original request or event so, we used appropriate identifiers and the, the structure log so like we could follow the, processing, path, rather than like looking at the isolated log messages and see. 
 14:37: for lineage. 
 14:39: I think about like it as. 
 14:43: Understanding where the data originated, like what transformations happened and. 
 14:49: Where it ended up. 
 14:51: So in our injection flow, we, we had like source clinical data like coming into the API validations, like the norm normalizations are occurring and the invention injections layer of Kafka carrying the event and then the downstream processing, making the data like available in the data breaks and see. 
 15:15: We maintain the information needed to troubleshoot and understand at the moment. 
 15:22: OK, yeah. 
 15:23: OK, what else I'm thinking, so you talked to me about. 
 15:28: So do you, so when you go in front of the customer, will you have like good 3 or 4 stories like this to talk to him in case if it goes deep down? 
 15:38: So everything that I touched upon right now, try to go deep into it and see, you know, what else you can brush up, what else you have done. 
 15:45: And try to explain to them more on performance observability because they're really heavy to audits and stuff like that. 
 15:50: it's a, it's a a company that you know that they're very heavy into audits. 
 15:55: So, and one of the primary reasons they're doing this modernization is because they want to be tax compliant. 
 16:04: So you want to think about, scenarios where you have, we, we have contributed to that and, how you handle different types of, so what kind of different data type formats have you handled for HS 7 models, generally, like, like we handle primarily the Jason-based clinical data including, fire standard sources coming from the different source systems and the source data was not always like consistent, so. 
 16:34: One of my responsibilities on the injection site was to evaluate the payload, check the, the required fields, normalize the structures, and, The security and the audit perspective because this is like the healthcare data we had to be careful about the authentication issues logging and also like for HS 7 like I was careful about like how I describe my experience. 
 16:59: HS 7 was like the the relevant to the healthcare like interpreity environments like but my strongest experience it was like the SSI style of the Jason resources. 
 17:12: OK, well, I think I'm good with your thing. 
 17:15: I mean, any questions for me? 
 17:18: I just want to know like, like, apart from this, like for the future. 
 17:27: Yeah, so as I told you, there'll be 3 rounds. 
 17:29: So customers, so we'll upload your resume, get it uploaded. 
 17:33: So if they shortlist, they will call you, send you a note, for scheduling a customer. 
 17:38: And if you clear that you will go into the dil. 
 17:41: You will get a link to do it. 
 17:43: So it'll be basically Python scripting and SQL scripting. 
 17:46: You'll get in a half an hour kind of a test. 
 17:48: So you have to complete that within 72 hours. 
 17:51: So just make sure that you are using best practices, putting comments. 
 17:55: Just don't write a piece of code and leave it for the. 
 17:58: person to read it. 
 17:59: So put some comments in terms of how you process the basic stuff, right? 
 18:03: So make sure that your code code is readable and, you know, so whatever it is, right, and, once you clear that there's gonna be probably one final round with the customers and the 2 or 3 people from the team they'll probably talk to you. 
 18:17: So it's gonna take, I mean, so they're moving fast and slow, also fast in the sense when they move they move pretty fast. 
 18:25: so right now I think there's only 1 more position left. 
 18:28: So there are, we have filled 4 out of the 5. 
 18:30: So we are, I'm, I'm actually submitting a couple of more candidates for the 5th position, so hopefully, they should close it soon. 
 18:42: OK, yeah So yeah just prepare well in these areas like I mean the things go deep, talk to you about what you have done, across your design performance scalability, you know, challenges that you have faced. 
 18:58: Go deep technically. 
 18:59: I mean don't try to be at a peripheral level. 
 19:01: Go deep into the Python frameworks. 
 19:04: And tell what kind of challenges you faced where and how you resolved it, right and if it is calf car just go down into the technicalities of the deep in terms of how you're handled that cough car. 
 19:16: So I think those are the kind of things that they'll be looking for and you know, if, if you are, if you have any specific clinical, data inion experience that you can bring up, you can bring that up too. 
 19:28: Do OK, yeah. 
 19:32: Anything else? 
 19:34: not from my side. 
 19:36: OK, cool. 
 19:37: Good luck, and I will, we'll keep you posted, the next step. 
 19:40: So keep a look. 
 19:41: You should get some, yeah, if you get an email from validate.com and just keep a look on your spam folders and stuff like that just to make sure that you're not missing out on anything, OK? 
 19:51: And your vendor, vendor will also reach out to you. 
 19:53: We'll let you know once we hear from the customer. 
 19:55: Got it. 
 19:57: Yeah, bye-bye. 
 19:59: I'm good. 
 20:00: Yeah, all right, thank you. 
 20:01: Have a good day. 
 20:01: Bye, same here. 
 20:11: there's the 
