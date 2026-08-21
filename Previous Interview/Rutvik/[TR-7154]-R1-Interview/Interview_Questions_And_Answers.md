0:00: Book Oh yeah, you have a lot of work today. 
 0:05: no, it's already done, but you know, process this crossing, what is the pending for this board that's all. 
 0:15: Oh, I am so sorry. 
 0:17: My Wi Fi has seems like it's causing some issue. 
 0:20: Would you like forward to dropping the coffee back in really quick? 
 0:23: Sure, sure, no, no problem. 
 0:25: Thank you, yeah. 
 0:35: I idea. 
 0:38: According to the Hello. 
 0:44: Hey. 
 0:44: Hey, Naveen, how are you? 
 0:47: I'm good. 
 0:47: How are you? 
 0:48: Yeah, doing good, man. 
 0:50: Just, it's a Friday so typing out some of the work. 
 0:54: That's good. 
 0:56: Can you give me a minute, my colleague Jenny will be joining. 
 1:00: Yeah, I think she just joined, but, she is, she's facing some network issues. 
 1:03: She rejoining. 
 1:06: I mean, I will turn on my camera in a few seconds. 
 1:09: Yeah, no problem. 
 1:13: All right, all right. 
 1:17: Just gonna take some notes, And I'm going to open your. 
 1:24: You were doing it. 
 1:31: So that's it, where are you from? 
 1:33: I'm from Plano, Texas. 
 1:37: Oh Texas OK. 
 1:41: And where do you work right now? 
 1:42: I'm working in, like Vincent, basically, it's my current time. 
 1:48: Sorry, what is the prince name? 
 1:49: Vincent, Vincent. 
 1:51: Vincent, it's, yeah, yeah, it's also my visit. 
 1:56: I mean, it's they have, you know, frequently people are pronouncing some of you know, some, some of them are pronouncing Vincent and some of the time Vincent, so. 
 2:05: OK, OK, that's good. 
 2:08: OK, so I have your profile. 
 2:11: So what we can do is, Ruth, we can start with like a quick introduction about yourself, OK. 
 2:19: it would be great if you can focus on your, recent experience, OK, and, we would love to understand more about your experience working with the AWS services as an engineer again, right? 
 2:34: Correct, but focus is more on the back end engineering, OK, so we would love to understand and try to tie it back as like you can keep everything. 
 2:42: Big shot as much as possible, but at least for one of the engagement, be it the res one or the prime one, try to, like, you know, associate it with a use case or the, the engagement problem you're trying to solve. 
 2:57: OK, sound good. 
 2:59: OK, so, let me know what you say. 
 3:02: First of all, hi, I am my is rhetoric SI, and I am the Python. 
 3:05: Yeah, I'm a update from engineer. 
 3:07: Around like 2 experience software in the software industry. 
 3:11: Mainly, you know, I, I work on cloud native application, data engineering, AMI. 
 3:15: My core and expertise in the Python, SQL, REST APIs, AWLN, Data Bricks, Dockcoun, datacom, CICD, they know, and the PS log as well. 
 3:25: I also work on extensively with the framework like PAS API, Class, Django, along with, you know, front-end technology like such as like DA, TypeScript, JavaScript. 
 3:34: So, about my current project in Vincent, basically, currently I'm working as a lead AML platform engineer where I can, I am involved with the healthcare data analytic platform and we're processing a large volume of healthcare data for the analy analytical and downstream downstream, you know, building data workflow where data comes in and like transform into the Python database, BioSpark, and then that made available for, you know, downstream consumers. 
 4:03: And we, on the AWS side, I have hands-on experience with the S3 lambda, EC2 RDS Dynamo DB. 
 4:10: For security purpose, we use IM policy and I also work on step function. 
 4:15: you know, I also work on terraform and infra as a code, docker for centralized Kri, sorry, for site and for API development, I build general as API using Python fast API. 
 4:28: Or about like if I'm saying about my work which I have done, so it's, you know, kind of data which we are dealing with is, it's a kind of healthcare data and basically, you know, we, I can see that one of the key project responsibilities is, is like building a data workflow where data is received from through Amazon A3 and Validate and transform using Python, data breaks, Paspark, right? 
 4:54: And, then, then we made available for downstream application and I also work on the like building APIs. 
 5:01: I also work on data handling, logging, metrics, case logs, and we also, you know, coordinate with the team to, you know, production supports. 
 5:09: Yeah, that's all pretty much about me. 
 5:12: OK, tell me about, like, tell me 11 of the recent project experience, right, where you're trying to solve, like you are telling that you're picking data from S3, of course data might be coming from somewhere else, right, correct, then you're storing processing using, like, you know, say like lambda, or any other framework while you're storing. 
 5:35: I would love to understand why you're storing on database, OK. 
 5:38: , another thing which I would love to add you about that is where are you using step function if it is not relevant to that engagement, then how you're orchestrating it, then, help me understand your approach towards, like, you know, CICD and deployment, right, to deploy the applications like, and in what cases you have used terraformation whatever, like, you know, you have used. 
 6:06: OK, sounds good. 
 6:07: OK, so I need to cover him a lot of, a lot of things. 
 6:10: So, let's start with my current, like project. 
 6:12: I give you like how, like, what, what we are trying to solve, right? 
 6:16: So first, the reason we store data in S3 first is mainly because we need to durable and scalable and cost-effective like, like landing zone. 
 6:25: We don't want, you know, downstream to sync to dependent directly on the source system being available or at the all time. 
 6:32: And once, you know, once, once data is landed in the estuary, we can validate it and track it and respond, respond it if it's necessary and maintain, maintain the auditable trail. 
 6:43: From there, we have been pushing workflow, like for, for smaller event, driven tasks, we can use AWS Lambda while, you know, for large transformation, we use data breaks. 
 6:53: With the passport. 
 6:54: For example, if, if we are like validating the incoming file structure, check and like check the required fields and data quality and perform the the like transformation and standardization, then the process data into the appropriate storage or data platform for downstream public analytics system. 
 7:15: One important part is we don't apply, you know, or don't simply, you know, overwrite the raw data. 
 7:20: We maintain a separation between raw or lending data and then postage data that basically give us more ability to go back, like back to the original imports transformation has been a problem if it's business rules changes. 
 7:36: For architecture side, I can give you like overview that you, you can think like, it's a, it's a, it's, it's a source system. 
 7:43: Then there is ST lending review, then there is validation which we are performing like transformation using Python data breaks, then the current data, what we are dealing and downstream analytic and application. 
 7:54: The main value of the, this approach is decoupling and the scalability side. 
 7:59: We also like, like it's an approach for reprocessing a capability. 
 8:03: It's also, you know, allowed different downstream consumers to use current concurrent data. 
 8:08: And yes, the current, current engagement we use our oxidization like based on the type complexity. 
 8:14: AAWs step function are useful when we have, you know, multi-step workflow and where we need exp explicitly state management to try and branch, branching or error handling. 
 8:27: And for example, like I'll give you an example, like, like tri triggering the lambda and validate validating the result, and then moving into the next person, the steps, I have no, I also, I can say, I also work with airflow and database workflow for data pipeline, where we have no more data engineering-oriented dependency and scheduling processing. 
 8:48: For CICD side, yeah, for CICD we use data action. 
 8:51: We, when you, when developer reads the project request, the pipe and like perform, things like, code formatting, and, and that the checks and checks with the blank and linking with the flask and piling and there's no multiple test cases which we have found in the by, you know, with CIPD here. 
 9:11: Once changes are passed and required check checks are approved, the pipeline can be built, you know, deployment artifacts, do or image, and deployed into the appropriate averse environment. 
 9:22: So yeah, that's, you know, that's pretty much, I can say, give you the overview with all, with the effects. 
 9:30: OK, Jenny, go ahead. 
 9:33: No question. 
 9:35: Yeah, thank you so much. 
 9:41: I think you're feeling, yeah, you know, helping me understand the context and everything, Jenny, battling. 
 9:49: Yeah, better go off video. 
 9:52: Yeah, can you hear me better now with camera though? 
 9:54: Yes, yes, yes, sweet, sorry about that. 
 9:57: Yeah, seems like my painter is unstable right now. 
 10:00: yeah, no, so, thanks so much for covering your experience. 
 10:03: I think that has been really helpful, just to kind of go over your, like, Software engineering background, right, so I did review your resume and I did see something interesting about how you have utilized both terraform and confirmation for resource provision. 
 10:20: can you please elaborate what cases you who you used one for terraform and another board the information, and what's the pros and cons. 
 10:31: Telecom site, like, definitely I have, you know, worked on telecom site and, you know, and the platform vision site as well. 
 10:37: My experience I have used like, like both, right? 
 10:39: And but, but I know, but choice depending on mainly on the project requirement and how it will be specific infractures we we are managing for terraform. 
 10:50: I primarily use it when we had infrastructures across multiple services or when we wanted to, wanted usable modular infrastructure as a core approach. 
 11:01: For example, I, I, it's in, in, in my current project, we have AWS resource such as like SD Lambda, IM rules, policies, and network components. 
 11:12: So, with the terraform, we can define those resources as a core and keep them at nugget. 
 11:19: And performing a plan or and review or before making any changes, and maintain the consistency across the environment. 
 11:26: And I have used cloud formation more in, more in the situation where, you know, the infrastructure was heavily on the A levels specific and the team, you know, wanted to use native ideas pre preing I can say, for example, when, when, you know, when, when, when deploying a lambda-based application with the state IM rules, permission, and event configuration and supporting AWS resources, the our formation can package those resources together as a stack and manage their life cycle. 
 11:59: So if we have to, like, if I have to choose between like both their terraform is my preference when I need usable module. 
 12:07: consistency across the environment, or, you know, potentially multiple cloud providers and the other side cloud formation makes sense when, you know, we are staying deeply with the AWS and want tight, like tight integration with the AWS Native Services, either. 
 12:23: Either is like the, I treat the infrastructure as a code, the important part for me, infrastructure changes code to the get code and CICI CDC like pipeline rather than, you know, being manually created or modified in the AWS console. 
 12:39: So yeah, that's, that, that's what was my choice. 
 12:44: OK, sounds good. 
 12:45: Thank you so much. 
 12:46: So I know you one of the benefits that you said was terraform is that you can have it as a, you know, modular component to the body, right? 
 12:56: Is that, well, does that apply for confirmation as well? 
 12:59: yep, definitely. 
 13:01: See, there is no, I can say there is some similarity, right? 
 13:04: And if, if I have to choose like for the terracom side and and cloud formation, the good point, the cloud formation does support like modularity as a well through the feature like nested stack and stack export import. 
 13:19: So it's not, not that cloud formation lack modular. 
 13:23: The difference I have seen in the practice that terraform modules tend to be more flexible and easier to reuse across the team's environment and yeah, and we created usable terraform modules for S3 IM and RDS. 
 13:38: Different teams could consume the same module with the different parameters without, you know, rewriting the infrastructure of the code. 
 13:46: And with the cloud formation, we can achieve something similar to using like Nester tech, right? 
 13:52: to the end. 
 13:52: So yeah, that's that's why, why I said. 
 13:57: Sounds good. 
 13:58: just to expand on that, so do you have a familiarity using with, the AWSCLI by chance? 
 14:04: Yeah, definitely, definitely. 
 14:05: So, I know, I, I have like comfortable with like on the CLI site, we have used alongside with the terraform and application deployment like all for operational troubleshooting tasks, and I have used CLI, you know, work, to work with, you know, service like S3 Lambda and RDS checking resources, validation configuration. 
 14:25: For S3 specifically, I might, you know, I might use the commands like AWS S3 LS or SDCP just to verify whether the files have been arrived or moved data and test data, during, you you know, during the development and for lambda, I can use CLI to inspect function configuration version or invoke the function, function adjusting. 
 14:50: So I also find it CI is useful. 
 14:55: OK, sounds good then. 
 14:57: Then how do you run these? 
 14:58: So it sounds like you're pretty familiar with the commands like invoke and everything. 
 15:02: So just out of curiosity, how do you verify whether what you're building is working before you actually deploy to the actual resource in the AWS. 
 15:14: Yeah, I guess, yeah, definitely see, it's normally try to, you know, validate as much as possible locally and CI Python before making any changes, right? 
 15:24: For Python application, we have, we have in a local deployment workflow using Invoke for common task, and for example, like I, I can use the invoke task to run formatting, printing, unit tests, another validation step consistency. 
 15:39: I use like black black for, you know. 
 15:41: You know, formatting taskscape for and piloting for code qualities, fire test for unit test, right? 
 15:47: And for AWS specific functionality, I don't want my unit test to depend on the live AWS resources where it's possible. 
 15:55: So, I, I, I mock the AWS interaction and external dependency during the unit test. 
 16:02: So that's basically allow us to test things like S3 processing, lander logic, or error handling. 
 16:08: You know, in the, in the production resources without, you know, without actually modifying the production resources, so yeah. 
 16:15: How, so I, I'm, I'm getting, I might be getting a little too specific here, but you know, for example, lenda, say that you're building a lenda. 
 16:23: Before you deploy to the actual lambda resource, say that you would like to, you know, test if this lambda is working locally first. 
 16:31: You're the AWCLR how older one that come online. 
 16:36: I'm sorry, so. 
 16:38: If I want, like, as you said, like if I want to, like if I want like test lambda locally before deploying creators, for example, if it's a Python lambda, I can invoke the handler locally without sample event. 
 16:52: Like if the projectorries, I can also use also random lambda container locally and move the local lambda runtime endpoint. 
 17:01: If lambda is already deployed to the AWS. 
 17:05: Then you know the AWSC CLI, you know, command would be something like. 
 17:10: Specific that this is AWSs lambda invoke on the fun I think functioning, then there is that there's what we feelload we are sending. 
 17:19: Yeah, that's actually, I'm not sure that's the correct command, but yeah, that's something the command related to it. 
 17:24: So basically to send the sample event Jason for BPload to the lambda, then write the response to the response of Jason whatever file, but important that command invoke the deployed either the lender, not local one. 
 17:39: Right. 
 17:39: And for local testing, I would typically run them like hander directly or use AWS lambda runtime interface emulator if we are using container, right? 
 17:49: And, yeah, I, I could start lambda container locally, then call the local in like invocation endpoint, the same type of event, right, and for you to send, to send data. 
 18:04: OK, no, sounds fair enough then. 
 18:05: Thank you so much. 
 18:07: OK, let's go into the other component then. 
 18:11: So I think you are also familiar with the KMS, the for the key manager services. 
 18:17: So you know. 
 18:20: So there will be several projects. 
 18:21: So within this one project, say that there are several services that we utilize and we have consolidated all these key, secrets in like single PMS, right? 
 18:33: So say that there's been a change in the naming convention. 
 18:37: So say that before it was, it was used to be all lowercase and in password, and then now there's a new rule around organizations saying that we need to rename these passwords to. 
 18:50: tunnel cases, right, then how do you manage change? 
 18:55: How do you manage the change safely across tech bubble rebounds without without a coordinated big bang release? 
 19:02: OK, for this scenario, like. 
 19:07: The reposed with the coordination, right? 
 19:09: So, I would treat that as a backward capability configuration migration rather than like trying to change all 10 + at the same time. 
 19:20: And first, I would, you know, avoid changing the existing secret or key difference immediately. 
 19:26: I would, you know, I, I would reduce the name camel case name, like a, like new camel case name while keeping the old name available temporarily. 
 19:35: For example, if, if the, if, if the existing witness is, is And, and like and password, I would, you know, introduce the end and password in the, in the camera case and have both available during the like transition. 
 19:48: This is basically block us you know kind of blockage any kind of, and then I will update the repository incrementally. 
 19:55: Each service would have changed to look for the new name first if necessary. 
 20:01: During the migration window and fall, fall back into the old name, I would put that changes to the normal PR or CSCD process to deploy service independently. 
 20:12: Once the services, you know, has been migrated, we can, you know, we, we are verified through the application logs, metrics, smoke tests that basically that new difference are being used successfully. 
 20:24: I would, remove the fallback from the e-service in a second changes. 
 20:29: Only after I am confident that all consumers have been migrated, would, you know, would I remove, deprecate the old cigarette key difference, and I also make sure, make, make the migration observable. 
 20:43: I, I would check like, which repository and environment have been migrated, and ideally add the automation check to prevent new new deployment from interruption or old naming conventions. 
 20:56: So that would be my, my approach, I guess, this will, this willful fulfill the requirement. 
 21:03: Sounds good. 
 21:04: Yeah, thank you so much. 
 21:06: I think you pretty nailed it there. 
 21:08: OK, so, next up, sounds like you have dealt with a lot of resource provisioning, and you know, you directly work with those resources. 
 21:16: So how do you search for in the cost metrics, you know, all of these resources? 
 21:22: So, like, so, yeah, so resource side like I treat cost tracking as a part of, you know, infrastructure design, not something that we check only after the resources are deployed. 
 21:33: First, you know, I make sure that resources are pro like properly red tagged for like, for example, like by, by, by application environment or environmenting project or call center. 
 21:46: With the tariff form, I can extend like those, those tags across the resources and we provide like pro provisions so, so that, you know, resources are attributable to the correct, correcting or application, then I use the AWS cost sector or AWS budget, budget to monitor the actual spend versus, versus, you know, the expected budget. 
 22:09: And for services like S3 lambda, S3, sorry, EC2 or RDS Dynamo DBI look at the users and patterns, use pattern, identify like unexpected increases, increases or not, and in some cases that happens so it's very helpful. 
 22:25: If S3 S3-based data pipeline suddenly start storing, you know, significantly more data than expected, I would look at the storage growth request or volume. 
 22:35: And data transform to determine whether it's a ligament venous diseases or the insufficient insufficient workflow. 
 22:45: And yeah, for, for the engineer perspective, I, you know, I, I look at the optimization, optimization opportunity, and yeah, that's that's the experience I have. 
 22:59: No, that sounds good. 
 23:00: You know, so to branch off that, you know, to branch off from, from the response, can you tell me about the time you led the cost optimization of reliability initiative on the AWS? 
 23:10: And what did you, what, yeah, and what, like, you know, what did you measure, change and achieve at the end of the day? 
 23:19: one example I can, I have in mind like. 
 23:22: during like, in the present and engagement, we was in around the optimizing our data processing workflow and improving its seem reliable at the same time. 
 23:32: We had a workflow where, where the data was landing in the S3 and then going through the validation and transforming using the Python and database faster. 
 23:42: On the, on, on, on one thing that I focused was making sure we, we were not, you know, unnecessary processing the same data multiple times because it's, it's basically directly impact the both complete cost and pipeline reliability. 
 23:56: And you know, the, the first look at the workflow from the end to one perspective, how, how often like jobs are being triggered, how much data each jobs was processing, where was, where's the failure we're happening, whether the, you know, we are doing the data processing or not. 
 24:15: And the one example I have one more like instead of like, instead of like treating every execution as a complete, complete reprocessing jobs, we could identify, identity like the relevant imports data and the processing only what, what was required. 
 24:30: We, we also made, made the new workload more like more on the designed by the having proper logging retry mechanism. 
 24:40: Yeah, that's what I really needed and like issue did not really require manually restarting entire if anything pills and. 
 24:51: From that side, I also look at the whole situation. 
 24:53: The important part me, for me like was the cost automation, you know, shouldn't, like should, should not come at the expense of the reliability side. 
 25:04: So I, I measured the impact through the jobs, eluation time, failure receipts, resource utilation. 
 25:11: Processing of volume before, you know, before, after any changes happens. 
 25:15: So as a technically my role was not just, you know, just making the code changes. 
 25:19: I also identify the bottle and discuss the trade-offs. 
 25:23: So these are a couple of areas which I have looked, whenever I get a chance to, you know, get the solution on the international site. 
 25:33: That sounds wonderful. 
 25:34: Thank you. 
 25:35: OK, so let me jump into all the components of AWS tools then. 
 25:39: so since you have a lot of experience in lab testing, let's go with that. 
 25:43: so say that there are services, right, there are two proposed for, this API endpoint where one is to just utilize, to just to create microsurfaces, create different API, and to the end, OK. 
 26:02: Oh Are you running the question? 
 26:09: Hello Sorry, are you done with your question? 
 26:12: Like, acting like you break somewhere. 
 26:16: Yeah, yeah, she was breaking up. 
 26:18: So you're breaking up. 
 26:18: Can you repeat the question? 
 26:20: Yeah. 
 26:21: Yeah, no, but, yeah, OK. 
 26:24: OK. 
 26:30: OK, I want to say, can you, can you hear me now? 
 26:32: Yeah, I can, I can hear you now. 
 26:34: OK, so say that, OK, so say that there are two approaches to the event-driven architecture. 
 26:42: One is using the REST API and another one is lambda with API gateway. 
 26:48: In what scenario would you rather propose using lambda with API gateway over rest API? 
 26:54: Hey, so, so. 
 27:00: Yeah. 
 27:01: I, first I, first, I clarify one thing like EP at this lambda I'll still the S AI approach if we are exposing the SD that point. 
 27:11: So I, so I would, you know, I'll compare the like traditional DS API, back in like back in by currently running service versa API gateways a slender. 
 27:20: I would, you know, I would recommend the APEC gateways. 
 27:23: Plus lambda when the endpoints are relatively lightweight, stateless, or, or maybe even even. 
 27:30: So, especially, you know, when traffic is unpredictable, intermediate. 
 27:35: So for example, suppose we have like endpoints that when your client send the request to validate or processing the healthcare data file. 
 27:44: AI gateway, you know, receive the request and invoke the lambda. 
 27:48: lambda then perform the validation or or trigger, trigger it. 
 27:52: So and as synchronous workflow and, and, and return the annual response. 
 27:57: If, if we only receive the request periodically, the, the lambda is not attractive like because we have, we don't want, don't have to keep the application server running continuously. 
 28:08: And I, I, I, I would also consider it when we have automatic scaling, low operational overhead, and APEC address handler, handle the APL layer. 
 28:19: And lender, lambda handler, you know, to the compute and we, we don't have to, you know, manage servers or manually scale the application. 
 28:27: On the other hand, I definitely, I would, I would not choose lambda just because it's a very even if, if, if the API has long running processing very high predictable or like a stable traffic, and I'll, I stick. 
 28:42: Low latency requirement, and I, right, so in that case, you know, I don't choose lambda. 
 28:46: I would probably use the, as service standoff, you know, set of lambda. 
 28:51: So my decision is that my decision criteria definitely would be, you know, traffic pattern. 
 28:57: There's some scenario which I look before making any changes, pretenency requirement, scalability or operation overhead of both side as well. 
 29:05: yeah, that's, that's really be my approach. 
 29:11: Sounds good. 
 29:11: Thank you so much. 
 29:12: Then, OK then that sounds good. 
 29:15: Would you be able to elaborate, so I, so upon reviewing your resume, I did also see you. 
 29:21: Integrated the lambda with other resources like SMS to us. 
 29:26: Would you mind elaborating your experience with that? 
 29:28: Sure, sure, sure, definitely. 
 29:29: I have, I have, worked on like, for like both like lambda and rendering services using like S3 or SQS SNS. 
 29:36: So one common pattern I have worked like S3 lambda, then SQS, for example, when, when, when, when the new data I land in S3. 
 29:46: An event, you know, can trigger the lambda function. 
 29:49: Lambda, lambda basically performed the initial validation of processing and can, you know, can basically, I can see. 
 29:58: basically land up from that like, and validation site, right, and, using SQS, you know, to, you know, I can say, giving them a buffer, buffering and and decoupling. 
 30:09: So if it's downstream service, you know, it's temporary unavailable, or there are sudden spikes in a file, we don't lose the work or. 
 30:18: Overwhelming consumers. 
 30:19: On the, on the consumer side, another lender can pull the SQS queue and process those messages. 
 30:26: I would configure things like basically visibility timeout, pre-try behavior, best size, dead letter queue or field of so field message can be isolated rather than concluly try. 
 30:38: And with the SNS I have used the more publish subscribe pattern. 
 30:44: And like when, when basically, you know, important event occurred, lambda or another service can publish notification to SMS topics and multiple subscri subscribers can react independently. 
 30:58: Once the subscriber might trigger, you know, another lambda, while, you know, another good. 
 31:02: Send the operational motivation. 
 31:04: So that basically benefit of you can say combining these surveys in, in, in, in that, in that we can get loosely coupled and scaleable and lambda basically provide the, the new compute SKS provide the rely reliability buffering and processing SNS provide, you know, fan out multiple consumers. 
 31:24: So yeah, that's, and I also pay attention for the IMD's previous side as well. 
 31:28: That's also important, so yeah. 
 31:31: That's all I know. 
 31:32: I, that's my experience in the. 
 31:41: Jenny, I do. 
 31:42: I think Jenny's, I guess Jenny's bandwidth I can see here. 
 31:48: OK. 
 31:51: Telling me. 
 31:53: OK, can you hear me better now? 
 32:01: Actually, yes. 
 32:06: That's OK. 
 32:07: I think, that's OK. 
 32:10: I will let Jenny come back, but meantime, right, I think, this, role is again, like, you know, with the former client, it is more focused on building an engine, right, right where they are deploying like application using the AWS text stack. 
 32:27: most of the services are in use. 
 32:29: Can you hear me now. 
 32:30: Yes, we can, we can hear you. 
 32:33: so sorry about that. 
 32:34: I, I saw you, so go ahead, please. 
 32:37: No, no, I think I'm good. 
 32:38: I, I, I would let you complete. 
 32:39: I was just giving the background part actually, so I would let you complete your first. 
 32:46: Oh, I was going to jump to another, topic you open search you, but so, yeah, please, OK, yeah, so also I saw that you had worked on the open search extensively for being for your at your current workplace. 
 33:00: So, say that there is a large open search cluster like say this is like over 1 terabyte EDS, you know, with 6,000s. 
 33:10: And, and then 500 megabytes per second fed by compared to open search pipeline. 
 33:16: how do you evaluate whether this cluster is the right size and what is your strategy for index life cycle management, cost control, and reinvesting with. 
 33:26: Well considering clusters I do. 
 33:30: Yeah, and see, for cluster side of the set side, I would not, you know, immediately start changing the instance type or reducing the nodes. 
 33:39: I would, you know, first establish the actual workload and identify whether its bottleneck is a CPU memory, or heap side or storage or network or shared distribution. 
 33:49: And I start, you know, by looking at the open search metrics such as like CPU utilization, GVM, deep pressure, GC activities, like desk utilization. 
 34:00: So, I would latency as well, the index indexing throughout the, throughout sites and such latency as well, there's a multiple options we have. 
 34:08: I would also know, look at the indexing date on the S3 pipeline and And, and the query guiding because cluster, you know, cluster optimize the heavily injection can look every different like very different from the one optimized or optimized for search and for tight, like tight sizing, definitely, definitely this is important word I would correlate those metrics with the workload over time rather than, you know, looking at these things. 
 34:34: single peak. 
 34:35: If its cluster is constantly like under utilizing, we can consider reducing the capacity. 
 34:43: If we are not seeing the sustained heat pressure or high disc futilation, they, they may, they may need additional capacity or different node configuration. 
 34:56: And many people, you know, not able to understand that, that part and for index and life cycle management, I would, you know, definitely separate data based on the access pattern, for example. 
 35:07: let me remember, yeah, like, for example, like if in the, in the recent data that we have acquired frequently and, and basically can like can remain, you know, on the hot tire or while, you know, while old data can be moved, moved to less expensive storage tire, we can, you know, We can also use the rollover based on the index size and age and, and define, you know, retention policies. 
 35:34: So we are not just keeping, you know, data, data in like indefinitely, indefinite indefinitely when, you know, when the fitness does not require it. 
 35:42: And that you mentioned the cost side, right? 
 35:49: yeah, yeah, yeah, so for cost to conference, I definitely, I would focus on the, like retention and like shared sizing, storage tires, replica storage, strategies as well. 
 35:59: These are a couple of areas which I have looked. 
 36:02: Have like having too many like small shared like shareded can be creating unnecessary overhead, while extensively large like shared can make, make recover and rebalancing difficult. 
 36:17: So, both are, both approaches have some pros and cons, so I would aim the appropriate like shirt size based on the workload rather than in just choosing the like any kind of numbers, right? 
 36:30: So. 
 36:31: That's, that's would be my approach and that's, you know, how I approaches or in the given scenario. 
 36:42: I guess I, I, I don't miss anything. 
 36:46: No, yeah, no, you covered everything, so that sounds good. 
 36:48: Thank you so much, and then another on the open source, right, so say that the cluster hits, so yeah, so say that the cluster hits, the threshold like 85% storage, and it just pipeline starts to fail. 
 37:04: What are your immediate mitigation on that, and then what are the next 30 days effects? 
 37:10: Like my if integrity to. 
 37:14: Like I would, I would handle these two phases, like immediate, like mitigation, and then the long term, like 30 day fix. 
 37:23: Immediately, if the storage is 85% and injection is failing, my first priority is to protect the cluster and restore the injection safely. 
 37:32: That's the first priority I would do and to confirm whether the issue is actually disk utilization and identify which is like indexes, indexes or nodes are consuming the storage. 
 37:44: I would also, you know, check the. 
 37:46: Cluster health, scheduled allocation, indexing pressure, then I will, you know, temporarily reduce the pressure. 
 37:51: For example, if there are, if there are old in like indexes that are no longer required, I will remove them according to the retention policy. 
 38:01: If we have no, if we have snapshot or another durable copy, I would make sure the data are protected before deleting anything. 
 38:09: And if the witness required, The business, business requires a retire basically. 
 38:13: So our priority is adding the storage or capacity rather than deleting it. 
 38:17: Some cases we thought we needed, and I also look into whether the relic replicas are contributing, like contributing significantly to the storage footprint, whether they're, and whether they are safe temporary adjustment. 
 38:30: And for like for the next 30 days. 
 38:34: I would address the address the underlying problem instead of like like repeatedly studying the storage, and like the storage growth and determine whether the main focus is is retention or replicas or insufficient insufficient shard sizing and Finally, I would know, I will load the test, simulate the expected injection growth, and stabilize the capacity forecast, how much storage we are, you know, consuming per day. 
 39:01: That also I can look at. 
 39:02: So when we reached the next threshold, we, we, when we are reaching, yeah, basically when we are reaching the next threshold, that will also we can consider. 
 39:11: So that, you know, two part, two part, have, you know, provided both sides. 
 39:21: OK, sounds good. 
 39:23: all right, yeah, so that's all for the episode from my end. 
 39:26: So, let me, do you have any questions that you'd like to ask real bit? 
 39:29: No, I think I'm good. 
 39:32: Rafik, as I was giving the background, this is more on the former. 
 39:36: It's a small engine. 
 39:37: This is, core backend engineering work where you have to elaborate the of the services and, essentially like you deploy them, to enable the engine, right, right. 
 39:47: There are many features which they are building, more details to come, I think, if we move forward, right, correct, There's going to be one final round of like client interview, OK, I will give you one feedback, right, right, if you move forward, try to slow down a little bit, right, but as you escape, try to slow down, that will help. 
 40:08: That will help them, basically understand the, the, the, the, the, the, the way you're solving for it, right? 
 40:15: Just slow down, nothing more than that, that will help you, OK? 
 40:19: Sure. 
 40:19: Any, any further questions real quick you have? 
 40:22: no, no, actually, they, no, actually asking about the question or. 
 40:29: Any questions you have? 
 40:29: Yeah, I have like, already cleared in a lot of like what is the requirement and, how many rounds. 
 40:35: There is only one round left, right after this. 
 40:37: Yes, OK, that's all, that's all good. 
 40:39: That's all I have. 
 40:41: OK, hey man, what's, yeah, yeah. 
 40:45: No, no, go ahead. 
 40:46: Sorry, quick question cause it just popped in my head. 
 40:50: how do you use AI tools daily work? 
 40:53: Oh yeah, I do. 
 40:54: Yeah, definitely, it's a, well, I definitely, I use in a productivity way and give, you know, give my work more productivity. 
 41:01: I do, I do use in a day to day and I sorry, I slow down my work and I used to like lord. 
 41:09: Another AI like check GPT for things like understanding the unfamiliar code bases because, you know, we are developers, sometimes we forget whatever we have written in the last 4 months. 
 41:19: So I use the AI for that also, whenever I have to check what's, what's in the requirement we had and how we can proceed further. 
 41:28: As for you know, architecture side or the codeba side, I also will use cloud and JGPD for that. 
 41:35: For example, if I'm working on the Python service or data disintegration, I might use AI quickly to like generate the starting point for a function or suggest a different implementation approach. 
 41:47: I also use AI for documentation because that's pretty much helped me, you know, throughout my, I can see when, when I've been since I started AI the documentation for definitely I use AI but definitely I cross check and it's it's correct or not. 
 42:03: Yeah, that's day to day, you know, yeah, I use IM. 
 42:08: OK, thank you so much. 
 42:09: Sorry that. 
 42:11: No, no, no, that's good. 
 42:13: I mean, like, are you, OK, sorry, I just got sidetracked. 
 42:25: So, like, as part of your job, right, it's a good question. 
 42:29: As part of your job, like, you know, are you integrating, like, are you using anything like, you know, say like cursor or as part of your, basically, What do you call it, like, you know, where you're writing the code and all that, right? 
 42:44: How you're integrating AI like, are you doing that right now or no? 
 42:48: Yeah, so if, if you may like it whether they're integrating the AI into the application themselves, yes, I have, you know, experience at that as well. 
 42:56: I did that, but some cases, you know, some, some projects require privacy side as well, so we cannot, you know, expose our code or our documentation directly to the AI, right? 
 43:08: So in that. 
 43:09: I did not directly use AI, but in, you know, indirectly ways I definitely did, and, yeah, in some of the project I integrated the AI in my, you know, code base and like, no, my question is more like does your ID or anything have like, you know, any of those, yeah, yeah, they provide like are you using them like cursor or something like that? 
 43:29: Yeah, that's my question they are basically provide initially they provide a co-pilot for the beta site and after that they are going to the cloud site. 
 43:38: OK, and of, of whom you're working right now, is the end, and that's your current employer. 
 43:44: What is the reason for change if, if you don't mind sharing? 
 43:47: Yeah, basically, yeah, yeah, that's so, basically, you know, my current contract is going to be end like probably like next week, next Friday. 
 43:55: So apparently session is going on. 
 43:57: So this is the main reason. 
 43:59: OK, that's good. 
 44:01: That's fine, I think, we will chat, about it, right? 
 44:05: Correct, I can guarantee you one thing that if we move forward to the client round, I need to go with the confidence on one thing and do well because this is a long term, moreover, and this is one of the lifetime experience you will be getting to develop some application. 
 44:25: Really exciting, so that, yeah. 
 44:27: OK, so that's all. 
 44:29: OK, and thank you, thank you. 
 44:32: Great, thanks for your time. 
 44:32: Thanks, thanks, and have a nice weekend, guys. 
 44:34: Thank you. 
 44:35: Goodbye. 
 44:36: You too. 
 44:36: Thank you. 
