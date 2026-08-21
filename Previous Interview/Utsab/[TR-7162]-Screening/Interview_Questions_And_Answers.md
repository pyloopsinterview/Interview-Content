0:00: How are you? 
 0:00: Are you able to turn your camera on? 
 0:02: Yeah, perfect. 
 0:05: Am I visible now? 
 0:07: That's, oh yeah, wait, it just turned back off. 
 0:12: It's not, yeah. 
 0:15: Good. 
 0:16: Hi, thank you so much for joining. 
 0:18: I appreciate it. 
 0:19: Thanks, thanks. 
 0:21: How's the day going? 
 0:22: After the waist, it's good, it's going good. 
 0:24: How are you doing? 
 0:26: I'm doing good. 
 0:27: Good, so the way this is gonna work, I have just a few questions based off your resume, and then after that we'll go over potential next steps and any questions that you might have, but first, do you mind if I turn on co-pilot in the background to take notes? 
 0:41: Yeah, sure, no worries. 
 0:43: It. 
 0:46: do you want to start with giving like a 1 to 2 minute overview of you and your experience? 
 0:51: Yeah, sure. 
 0:52: So yeah, let's start my introduction. 
 0:54: So, hey, I'm up and I have 13 years of experience in software engineering, primarily focused on Python backend development, AWS, and cloud native applications and enterprise like integration. 
 1:07: Currently I'm working with the Health Past where I was like involving in our development and modernizing healthcare. 
 1:14: Application that and vacant services and a big part of my work being involved existing tightly coupled process towards the services and like even driven AWS architecture and on the AWS side I have worked hands-on lambda with the API gateway state functions S3 and Like cloudWatch, like for example, we had a web application where the front end was posted on the S3 and back end like was built using Python API gateway, was used in the like, you can say entry point and our Python lambda function had like hard things like request validation, business logic, data transformation, and integration with the workflow. 
 1:57: We use step function as well so to be break the process into a smaller and manageable step proper. 
 2:04: And I have also worked extensively on the Oracle integration, including database connectivity queries and data mapping, transaction handling, and also the timeout like management and exception handling. 
 2:17: And from the production perspectives, like I have used the cloud watch logs, metrics and alert to troubleshoot, troubleshoot the lender functions, API request, and the estate function execution, and I'm also comfortable with the CICD automation testing code review and secure configuration and Like development across different environments. 
 2:41: So yeah, overall my strength is like really on the Python back and AWS cloud engineering side, but I also like experience with the event-driven architecture, API and development. 
 2:53: So the production troubleshooting and cloud modernize. 
 2:55: So I have approached, worked across the full development life cycles. 
 3:00: Yeah, that's all from my side. 
 3:02: Absolutely, I really appreciate that overview. 
 3:05: like I said, just a few questions here regarding kind of your resume and your experience. 
 3:09: You might have touched on it a little bit during your introduction, but I'll start with this first one. 
 3:13: I noticed that you were talking about AWS step functions. 
 3:17: so can you describe a production workflow that you implemented using AWS step functions, and then why did you choose that instead of lambda? 
 3:26: Sure, so yes, and like my current project with the Help us we use. 
 3:30: AWS step function for like a production workflow we are healthcare related transaction. 
 3:35: We are coming through a web application and need to go through the several process step before the like before they like it could be completed successfully and front end was the hosted Amazon S3 and API gateway was used the entry point for a backend and when the request to like come in the trigger and a Python lambda function and. 
 3:57: From the, from there we use the step function to like orchestrate the different stages of the workflow. 
 4:04: like, for example, of the workflow, we were first request the validation and business validation, then like, like retrieve the, update the request information from the Oracle database, perform the like necessary data information and business rules processing, and then like trigger the downstream processing or notifications we can say instead of putting all the logic that one. 
 4:29: Largely under the function we separate into the individual, like, individual step step functions, so that made our workflow much easier to like maintain and troubleshoot. 
 4:39: And one thing that was like particularly useful in the production was to build an error handling retries and visibility. 
 4:47: If, like if, if for example the Oracle like integrations failed because of that because of the temporary. 
 4:54: Connection or timeline issue so we could like we could like configure the appropriate retry behavior instead of instead of like failing the entire transaction immediately so we could also identify the exactly function exact history and then like collaborate with the cloud watch logs for the lender functions. 
 5:15: So this will be overall we use the AWS cloud version and the functions. 
 5:20: Yeah, absolutely, I appreciate that overview. 
 5:24: I'll move on to my next question. 
 5:26: What kind of production experience do you have with Amazon RDS and then can you kind of describe that a little bit more in depth? 
 5:33: Yeah, yeah, sure, sure. 
 5:35: So I had a production experience with the Amazon RDS primarily around using manager relation databases as a part of AWS best backend application. 
 5:45: And my core database like experiences also improved Oracle. 
 5:48: So when working with the RDS, my focus has been, the application integration side as well as, operational consideration like connectivity, query performance, transaction handling, and the connection management and the troubleshooting. 
 6:03: In a, in an AWS application, the Python beacon would connect to the relation database through the. 
 6:09: Through the appropriate database driven and would be like make sure things like credential connection configuration, timeouts and transaction handling. 
 6:19: So we are being managed securely rather than the hardcoded in the application for production workloads. 
 6:24: I also like, I also like paying the attention to the things like connecting the pooling and, avoiding the unnecessary database connections and especially with the lambda because lambda can like scale the horizontal and create a large number of, concurrent connection if it is handling properly. 
 6:42: So from the operational side, I am like comfortable looking at the cloud watch matrix and application log. 
 6:49: So investigation like slow requires connection and this kind of things that I have done. 
 6:54: Absolutely. 
 6:56: can you walk me through an integration that you've built between an AWS application and an Oracle database or an Oracle service? 
 7:04: Yeah, sure. 
 7:09: So that I have worked through in my current like help us project, we had a backend application built with the Python and AWS, and one of the important integrations was with an existing Oracle database that challenged me that the application was being modernized and towards a more. 
 7:23: Powerless architecture, but Oracle was like still on important system of records. 
 7:28: So we, so we needed a reliable way for the AWS services to communicate with it and the flow was basically that API gateway received the like received the request from the web application and then. 
 7:42: , like, and then it will invoke the Python lambda function inside the, inside the lambda. 
 7:50: We first handle request validation and business validation, and once the request was valid, the Python server stabilize the requirement connection, Oracle like. 
 8:01: Like, in our Oracle request and even the connection to Oracle using the appropriate database driven our perform, the request to queries insert that like, insert our updates based on the business process. 
 8:14: So we also handle the like the data mapping logics. 
 8:18: So for the more complex business process, we didn't like keep everything inside a lambda. 
 8:24: We use AWS step function to orchestrate the workflow. 
 8:28: So yeah, the, this type of work I have done. 
 8:32: Yeah, so. 
 8:33: Last question here, can you describe any experience you might have with a vent bridge? 
 8:39: One bridge even. 
 8:40: So yeah, in the even bridge like absolutely things you are referring to Amazon even branch, right? 
 8:48: So I have used even Bridge in my like even the current project as a helper project as a part of our event-driven AWS architecture. 
 8:55: The main purpose like was to decouple services so one application our workflow would publish and publish and even without having a directly call every downstream system. 
 9:06: So, like, like, for example, after the healthcare transaction was successfully proceeded through the main API gate via lambda estate function workflow, so we would like to publish an event and even bridge it indicate like indicate that the transaction has been complete or that's a particular business event that. 
 9:26: occurred even bridge would then emulate that even like even against our configuration, even rule and patterns and route it to the appropriate downstream target and depend on the use cases there that could trigger another lambda functions or initiate same additionally like asynchronous process. 
 9:45: And from like production support perspective, I also work with the cloud watch log login and monitoring to troubleshoot even process issues if and even wasn't like producing the producing the expected downstream of behavior. 
 10:02: I would like, I would first verify that and even. 
 10:05: Even being generated correctly. 
 10:07: So overall, like overall I have used the event bridge primarily for the event driven and like a synchronous integration, especially where we like wanted to keep service loosely coupled and avoid synchronous dependencies between the system. 
 10:22: Absolutely, totally makes sense. 
 10:24: I see that you're located in O'Fallon. 
 10:27: Is that correct? 
 10:28: Yeah, OK. 
 10:29: I used to live in O'Fallon. 
 10:30: That's funny. 
 10:32: This role is a completely remote opportunity, but they do require working PST hours. 
 10:37: Would that be an issue for you? 
 10:38: Yeah, it will do, yeah. 
 10:42: so as far as potential next steps, that includes, usually it would include speaking to a technical screener for this specific role. 
 10:50: It just goes straight to a client submission. 
 10:53: to be completely honest with you, I think you are a pretty strong candidate, so I probably will be submitting you to the client. 
 10:59: I do want to give you a warning. 
 11:01: Sometimes it might take a little while to hear back from the client just depending on the hiring manager and kind of what they're going through and that kind of stuff, but. 
 11:11: Grab your availability for, let's say the rest of this week and next week if possible just to submit that along with your profile. 
 11:20: Yeah, sure, I will, I will share you my availability and, and next week I will most of the time I was available so we can conduct. 
 11:29: Perfect. 
 11:30: Yeah, just go ahead and send me an email after this, and then once I get that availability, I'll go ahead and get that sent over. 
 11:37: as far as the process in general, do you have any questions about that? 
 11:42: no, not right now. 
 11:43: Just like I have, already you cleared the preface, like the next step I would ask, but you already cleared it. 
 11:48: So right now I don't have any questions. 
 11:51: Yeah, for sure. 
 11:52: Well, if you don't have any more questions, I'll go ahead and let you go a little bit early. 
 11:56: It was really great speaking with you and we'll definitely be in contact. 
 11:59: Yeah, me too, me too. 
 12:00: Nice to meet you. 
 12:02: Thanks. 
 12:02: Thank you. 
 12:03: Bye. 
 12:03: Thanks for your time. 
 12:04: Bye. 
