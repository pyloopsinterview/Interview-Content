0:00: -hum. 
 0:05: Can you please remove the background? 
 0:07: Oh yeah, sure. 
 0:12: It's good. 
 0:14: Yeah, OK, Mr. 
 0:24: Yeah, can you please walk me through your background and, current project, your roles and responsibilities? 
 0:31: Mhm. 
 0:32: Sure, like, my side, like I have 13 years of experience in software engineering, with a strong focus on Python for tech development, cloud platforms, data engineering, and the AI driven applications, and, like I have more than 12 years of experience with the Python, like 7 years of experience working with like both Aure and AWS and like my core expertise like includes Python API and like generally most recently like I worked with the Mongodivi like engagement where I contribute a trade broader reporting platform like used by the like trading compliance and the operational team. 
 1:13: To analyze the millions of like trade reports and basically the platform users react on the front end and Python GP on the back end and MongoDB is as the like the primary database and like here my responsibility is span the entire application stack including the back end service development, API designs Mongo DB optimizations and like one of the like the major initiative I led was. 
 1:40: Redesigning like the reporting workflows to handle the large scale trade data efficiently. 
 1:46: I developed the first API services that export reporting APIs and like build the dynamic mongo DB aggregation pipelines to support the complex filtering search, sorting, and like the pagingmission requirements and like. 
 2:00: To improve the, like the user experience, I work closely with, content engineers building the react-based reporting dashboards and also, redefine the API contracts, optimize payload structure, and, reduce the response latencies like for the, large websites. 
 2:19: So that's pretty much about me. 
 2:22: OK, how, how do you design fast ATM microservices and, handling inter-service communication? 
 2:29: Mhm. 
 2:29: Like I would design like ATM system like as a set of small independently deployable services rather than like putting everything into like the, services. 
 2:38: Like, for example, like the in Mongo DP project, like I would separate the reporting trade data and the AI orchestrator, orchestration's responsibilities. 
 2:48: into the independent services and each service like exposes like well defined the rest APIIs using the fast fast and the identic models like for request and the response validations and for like inter-service communication, I generally use synchronous rest communications and the like calling service needs and like immediate response and for like operations. 
 3:13: That are like long immediate response and like require them and also I prefer an asynchronous pattern using messaging or in like the even driven approach so that helps me to like the scal and avoid the tightly coupling services. 
 3:30: OK, can you please explain your experience on React and TypeScri? 
 3:34: What type of applications we build, you, yeah, you can handle 88, 8 years of 8 plus years of experience in React. 
 3:44: Like I work extensively with React on the front end, particularly on the enterprise applications where like the, do I need to consume the like the Python or the past GP services and the large data sets. 
 3:56: And and recently like we use React for reporting on the dashboard layer like work closely with the back end team and like they find the API contracts and building the components for things like. 
 4:07: filtering and like searching the sorting paging issues and displaying the like the large data sets and also like I work with the functional components so it's like user state use effect and the use memo usable components, form handling routing and the API indications and also I work closely like on on attach it like the strong typing for like the component props API response requests. 
 4:35: And, like the, interfaces or os and the usable utility functions. 
 4:44: Can you describe in a a journey solution application you built, see, like on the journey side, like, basically like it was talking to our journey, like we have like creating the models or, or, or like, in my current project like the business problem like which I solved like was that the user such as. 
 5:06: trading and the compliance teams like we're dealing with a very large volume of like trade reports. 
 5:11: So instead of like manually applying, multiple filters and going through reports like we wanted to like allow users to like ask questions like in that natural language so such as like, asking for like, unusual trading activity or like a summary of activity like for a particular period. 
 5:32: So like on the back end side. 
 5:35: I use, fast API to build the, orchestration layer, and the flow was essentially like the user submits the natural language questions like from a DUI and the Python service like interprets, the request, identifies the, relevant training information, and also, retrieve the like appropriate data like from the Mongo D and then construct a control prompt like from the, like for the LL and, we did not simply send the users' questions directly to the LM like and the trust the response like, also like we, added the validations and the business rules like around the process so the retrieve data was like provided as a like a grounding context and we, we validated the generated response like, before presenting it back to the users and we also like implemented access control and audit logging like because like the underlying trade or information is sensitive. 
 6:32: OK, what are some common challenges associated with, using LLMs? 
 6:38: like the, the basic challenge was like the hallucination. 
 6:41: Like, an LLM can generate a very convincing answer that it's not actually supported by like the underlying data. 
 6:48: So basically in monitoring it, analytics like use case like we address that by grounding the model like with retract trade data, applying the business to validation and avoiding the situation where the model was like expected the invent information and after that the data security and the privacy like. 
 7:08: with, enterprise data, so I need to control what information is sent to the model and, like we use authentication and authorizations like apply the data access controls and make sure like the sensitive information is not like expose or exposed unnecessarily and I remember like another challenge is like context management like large prompts can. 
 7:31: Increase latency and cost. 
 7:33: So I did not simply send an entire like data set to the LM. 
 7:38: generally I retrieve only the relevant information and construct like the a focused context. 
 7:45: OK, you said that other munication, right? 
 7:47: What authentication and authorization mechanisms have you implemented, like, here, like, basically, from, like the OR 2 2.0 and the open ID kind of like typically using the JWT based access to or the security APIs, and like for authentication, like the client or, like the, the client indicates through an, identity provider. 
 8:13: receives an access to and like. 
 8:16: Passes that token as like the bearer token to the pass TPI service and pass TPR validates the token signature issuer audience and like expirations before before like allowing the request to be proceed and for like authorization I use rule-based access control like where the check user rule or the permissions, from the token or like an authorization service like. 
 8:42: For like more granual requirements and I prefer like permission or school-based authorization like for example like whether a user has reports reverses and reports rights. 
 8:58: which of your services have you used in production? 
 9:01: Oh, like, have you worked with, mhm, like, I like, I worked with several like Azure services in production like me application hosting integration, security, and the monitoring like for compute and APS like I've used Azure app service and as your function like to post post the fast EPD services and. 
 9:20: The serverless processing and I also like work with Azure API management for like exposing and security APIs also the throttling routing and managing API policies and for like messaging and as synchronous communication I use Azure service both and like have experience with like the event driven architectures and, for storage I work with the Azure blob storage for like the documents and the large objects. 
 9:49: And apart from that, I also use Azure Cosmos TV and also like integrate Azure hosted applications to the database such as like Mostly as well and the Mongo TV. 
 10:00: OK. 
 10:00: And finally, explain your experience on Linux. 
 10:04: Linux also, mhm, like I have total 7 years of experience on the Linux, like hands on, like, particularly for the Python development for API cloud development, and the like the project of troubleshooting like, like I work with Linux-based environments for like deployment and managing the Python applications, configuring the environment variables, like managing, processes, reviewing the application and the system logs. 
 10:32: And also the troubleshooting performance for like the connectivity issues and like from a development perspective like I'm comfortable with common Linux commands like profile and the directory management permissions processes networking and the log analysis and I like generally I regularly use the tools such as like find PS curl, nett tail calling the trouble. 
 10:58: production Linux serve is slow. 
 11:00: How do you troubleshoot it? 
 11:02: like, basically it's slow, but like I would travel to like systematically like rather than immediately restarting the server like first, I remember like I identified like water sources like actually, contents like CPU memory, desk input output or the network. 
 11:20: So I had to start with commands like up time top or like top to check the load, average and the, CPU utilizations then. 
 11:29: like, I had used 3, like, the command is like 3 I1M to, to look at the memory I back and if DF-H and DF I'd like to check the disk capacity and the ir node usage and, like for the disc performance I look to look at the input output weight and the tools such as like, iOS type 2. 
 11:51: determine like whether the server is like waiting on this and for like network related issue I check the connections and the like interfaces statistics using the tools like SS and SA SAR. 
 12:07: Oh. 
 12:11: how do you check the memory usage on Linux? 
 12:16: like for the memory, like, I remember, generally, I use the first. 
 12:23: Like I use top or like I stop to identify like which process are like consuming the most memory and if I need more details for a specific process then I can use the PS with the memory related fields like for example, I might run like free hyphenate top, and one more command is like PDS of hyphenation for, percentage and year or type. 
 12:49: So basically if the application is running in Docker or Azure, container app, so I also check the container memory, utilizations and configure the memory limits like through the platform monitoring tools. 
 13:04: OK, got it. 
 13:05: Thanks for your time. 
 13:08: I'll meet you on the next step, OK. 
 13:11: And one more thing, can you please, show your photo ID? 
 13:15: I'll take a screenshot of you. 
 13:17: Just give me a second. 
 13:17: It's another one, yeah, right. 
 13:35: Mhm I You're using any screen, my background, you know all that actually blurring actually it's basically the blur blur, yeah. 
 14:04: Yeah, blurry is coming now, now it's good. 
 14:09: No. 
 14:15: And like. 
 14:24: OK then, I'll read you on the other steps. 
 14:26: OK, thank you. 
 14:27: Have a nice day. 
 14:27: Have a good day. 
 14:28: Bye-bye. 
