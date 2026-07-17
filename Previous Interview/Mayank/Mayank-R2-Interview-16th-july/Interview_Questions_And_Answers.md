0:00: , just, you can see me, right? 
 0:02: Yeah. 
 0:03: Yeah, hi, nice to meet you. 
 0:06: Nice to meet you too. 
 0:06: I'm good. 
 0:07: What about you? 
 0:08: Yeah, doing good. 
 0:10: OK. 
 0:12: I can see you, but, like a shadow appearing at your face, I can't see clearly. 
 0:18: Let me check. 
 0:20: I mean to say that your face is not visible to me properly. 
 0:23: Like it's not like I mean at your face. 
 0:26: OK, I turn off my background. 
 0:27: Is it now good? 
 0:31: Yeah, somewhat. 
 0:33: OK. 
 0:35: Let me turn my. 
 0:39: Yeah, can you tear it, tear it down, so I think it was what, no, yeah, yeah, yeah, yeah, yeah, it's it's working. 
 0:48: Finally, yeah, sometimes you don't have like but right now I'm in the basement, so might be. 
 0:59: OK. 
 1:07: OK, let's start the call. 
 1:09: So we can start with your technical background, your experience, expertise, your current solutions, and your, experience working on different domains and projects, and then we can go ahead. 
 1:21: OK, OK, so can you let me know about your yourself? 
 1:23: Sure. 
 1:23: So, hi, my name is Mayank Kumar Sade, and I have around like 13 years experience building applications, primarily only using Python,.NET, No GS, and, React, and the, Modi in the database site and more on the distributed system and cloud native application as well. 
 1:41: Currently I'm working as a lead Python developer in financial service project in the Mogodivi. 
 1:46: And we're building, you know, we're building a trade blotter airport platform that is used by the compliance state surveillance and this operation team. 
 1:55: Basically to generate report on larger volume and trade data, my day to day work, you know, include designing, WS APIs, optimizing, DB queries, aggregation pipeline, reviewing the code, also, like adding some extra aggregate pipeline and, fetching new, new kind of report from blotters, and, over the, you know, one of the biggest projects I have worked was, you know, modernizing the core that is existing system. 
 2:23: Had, you know, performance issue. 
 2:25: So, so every new report required custom development. 
 2:28: I designed report required custom like, design, you know, metadata-driven reporting framework, using Python, MongoDB React that is basically support, filtering, sorting, imagination, configuration columns as well, and we use educate educate in the front end and because that, that educate, you know, is, also come connected with the back end, so we are sending the columns and, The schema data as well and basically to this is reduce the development efforts for new reports and simplify the improvement reports into a performance over the new optimization aggregation pipeline introducing right indexing strategies as well and I also wanna work on the dotnet in my licensing last last work last job. 
 3:13: So yeah, and I have a couple of years of experience in the OGS and react as well. 
 3:19: So yeah, that's all, all about pretty much about me. 
 3:25: OK, can you tell me about, your one of the latest projected no more DB trade bottle and reporting, right, yeah. 
 3:33: OK, so, basically, OK, so, carry on. 
 3:38: OK, so basically, in, basically in right now in Mongodivi we had, as, as I said, we have, you know, data reporting paid, and that is basically, you know, paid of this client, and we are dealing, we are handling the Bank of America which is BA, we're dealing with that client, and I was, you know, work with the. 
 3:54: As a lead Python developer, mainly on the back end side, and the platform is used by compliance and trade surveillance, as I said, and it's a basically financial trade data which we are dealing with and these are basically large volume of data. 
 4:09: I, I can say daily basis we are dealing with the. 
 4:13: Lots of, lots of, I can say millions of data and this is basically, comes under whenever we have to work on performance side and this is crucial because we are dealing with the sensitive data as well and, and, one more thing like I can say our trade, we also work on trade activity operational analysis. 
 4:32: When I joined the project, one of the biggest challenge was reporting regeneration was too slow and it's, it's basically very is every new report required custom backend development. 
 4:42: And and that made that made the system maintain very difficult and slow down and delivering new new new business requirement to solve this basically I lead the design metadata driven report framework using like Python. 
 4:56: Nobody can react on the back end side basically we use that and I designed and developed press API supporting server side imagination. 
 5:03: And filtering and another, you know, major part of my work is optimizing my MoDB education pipeline because we are also migrating to the different database like previously we are using Cassandra and but now we are shifting into the MongoDB so that is basically SQL based to non-SQL. 
 5:21: So it's more challenging to, to, to do the project, but, we successfully deliver requirement. 
 5:31: OK, how do you inspect, the aggregation performance of a manual Mogodivi? 
 5:37: How do you decide next strategy? 
 5:41: Is there an issue with my voice? 
 5:43: No, actually, but your camera is like previously you turn off your camera, I guess. 
 5:48: I don't know, I, I turned off for a bit, but I am turning it on right now. 
 5:53: Yeah, yeah, you can see it. 
 5:54: Yeah, I can see it. 
 5:56: So yeah, yeah, so, yeah, I was saying that how do you expect when would be aggregation performance? 
 6:02: How do you decide strategy? 
 6:05: Can you tell me a bit more about it? 
 6:07: Yeah, sure. 
 6:07: So whenever, like I see that aggregation query is taking longer than expected, I don't immediately, you know, start changing the pipeline because it's a really big changes over, you know, over the code. 
 6:18: So first I try to understand where the time is actually being spent. 
 6:22: And the first thing I do is review, you know, application pipeline stage by stage. 
 6:28: I look for a stage like lookups, groups, and short or unwind because those usually, you know, have biggest impact of performance when dataset is large. 
 6:37: And when, you know, when, when I use normal we explained method to, you know, understand execution plan plan and I checked, you know, whether the query. 
 6:46: Using indexes or doing the full collection scan because if, if the, if you know queries, scanning complete complete collection, it will, it will easily, I can, I, I can say this is actually that this is going to take longer time. 
 6:59: So, so how many raw documents are being like explained and whether they are staged or processing far more data than necessary because we are using project projection. 
 7:09: So whenever whatever. 
 7:11: Data required we, we need to send into front end. 
 7:13: That only data we are going to send. 
 7:15: So creation is also going to help us and in basically take product reporting platform, we, you know, generating reports, millions of trade data, and some of the reports are reported we are slow because filtering was happening after expensive aggregation stages. 
 7:31: There are multiple pipe filterings we have provided in the front end. 
 7:34: And we redesigned the pipeline so, so that, you know, filtering happen as early as possible and reducing the amount of data flow throughout the remaining stage. 
 7:43: And after every, every optimization, we tested the query again and compared the exhibition plan and compared the time as well, how much time it will like we have optimized so far and we validate, we validate the performance. 
 7:57: Performance improvement did not, you know, change the report results because sometimes if we change the pipeline might be chances we lose the outcome which we are wanted to, from the API. 
 8:08: So we make sure we have, you know, validate those results as well because that, that is not going to be changed as per expected. 
 8:16: So yeah, that's how I know I'm going to, solve this kind of issue. 
 8:21: OK, and how do you avoid loading too much memory into, I mean, basically loading too much data into the movie. 
 8:32: Yeah, so, so when, when we are working with the large data set, so the key is avoid processing and returning more data than the application actually needed. 
 8:42: So in my project, one of the, you know, one of the, one of the first things we did was apply filtering as early as possible as, as aggregation pipeline so that later stage work with the much smaller data set. 
 8:53: And we also, you know, we also use project, the project in, in the aggregation to determine only fields required for the report instead of loading entire documents, and that is reduced both memories usage and amount of data transferred. 
 9:07: And since, you know, since our report, API is just supporting large data set, we have implemented server side, pagination, so user, you know, user only. 
 9:16: Receive one page result at a time instead of loading thousands of reports in a single request. 
 9:22: So this is actually also optimize us and we also optimize the lookups operation by like making sure the joint fields are wearing indexes only joined the the data was was actually required. 
 9:34: And finally if we continuously monitoring query performance using explain method. 
 9:39: And optimize the aggregation pipeline whenever we notice unnecessary document is scanned, expensive. 
 9:44: This is basically help us to change that, keep memory users under control while, you know, while processing millions of records and also improving our overall response throughout the report system. 
 9:59: OK, let's suppose, the compliance team says that the trade boer, report total does not match the source from the Turkishan. 
 10:11: Basically, the UI source, let's say 0 reports, but the source says 1000 reports. 
 10:19: So what are the areas you're going to investigate and why? 
 10:23: OK, so basically for this kind, this kind of scenario, I can, I, I can actually, to be honest, this is the same, same last week, this kind of issue I we have faced because, you know, this is actually, let me, let me give you an example. 
 10:37: First I, I, this kind of issue I have faced. 
 10:39: So first I reproduce the issue using same filters. 
 10:42: I connected with different. 
 10:44: And other teams to what they what they are basically targeting and what kind of scenario they are, you know, applying on it. 
 10:50: So I, I fetch those, those requirements, same filtering and compliance team uses such as trade data, business unit amount and status. 
 10:58: I want, I want to know, make sure I'm comparing exactly the same data because sometimes if we are, you know, if you are not. 
 11:05: with the teams, we had you know sometimes we had, like solve a different kind of problem which is not, they are targeting. 
 11:13: And next I will verify the source data. 
 11:15: I would check whether the source, system actually has thousands of records for those filters. 
 11:21: If the source itself is correct, that I would start tracing the data flow through our application. 
 11:26: So, so, basically next step would be to check the backend APIs, verify whether the API is returning only 98 records or whether they're returning correct round of count or UI is displaying the incorrectly. 
 11:39: So since sometimes front end is not, you know, bind up together correctly. 
 11:44: So that is also causing the issue. 
 11:46: So I make sure the, the issue is not from our side in the back end. 
 11:51: And, since I work extensively with the rest API, I review the API response and application log. 
 11:56: And if the API is returning only 98 report, I will investigate more DBation pipeline. 
 12:02: I would check the match condition filtering out report unexpectedly and whether there is issue in lookups or group stage or whether whether the rule-based security hiding some reports or some the particular users because if we are, you know, if we are added some kind of a compliance and policy like these are, these are only user which is going to she, I can see. 
 12:24: Display this kind of record. 
 12:26: So, so that is, that is also a kind of issue. 
 12:29: So, that's how I know I'm going to, investigate this kind of issue and resolve it. 
 12:36: OK, let's suppose we have a legacy system that has.NET or C or Angler. 
 12:44: And I want you to replace it with new, tech that is Python node react. 
 12:53: But the condition is that I want you to modernize it using business critical set also but without breaking the users. 
 13:03: So what are the strategies that you're going to adapt to modernize the legacy application. 
 13:10: Actually this legacy kind of thing and I can say the good, I can say this is, that's a good modernizing scenario and my approach would be migrate the system gradually instead of replacing everything at at once and especially, you know, it's a business critical application, first step, first step would be, you know, I understand existing application. 
 13:31: I would work with the business teams and identify the critical workflow, APIs integration. 
 13:36: Our business rules that cannot be changed before writing anything in code, it's important to know exactly how the current system is behaved and then, then I would break down the application to the smaller modules and priority is the which part can be modernizing first instead of, you know, replacing entire application at once, and I would, you know, migrate one module at a time while, while the rest of the system continue on the, on the, on the previous one. 
 14:02: And this is basically reduce the risk of, this can allow the user to continue working without, you know, distributors. 
 14:07: And and yeah, for each migration module, I will build a new backend backend using Python or Nodes and expose the functionality through the well-defined rest APIs. 
 14:18: If the UI is being modernizing, I can see, I, I will, I will double the new screens in the React while keeping the remaining angularid screen working until they are ready to replace. 
 14:29: And throughout the migration, I would validate the new models, like to see the same business results. 
 14:37: As a legacy system before switching user over and I would also closely work with QA business users to verify the business rules haven't changed and this, this is actually quite similar to my current project and in previous job we had, you know, we, it wasn't, you know,.net migration we're modernizing this, I can say legacies reporting platforms instead of rewriting every report individually we build that usable metadata. 
 15:05: Driven report and frameworks. 
 15:07: So yeah, that's how we actually achieve the moralizing transaction. 
 15:13: OK, can you talk more in perspective of like pipeline. 
 15:18: needs and tested. 
 15:22: OK, so pipeline requirements, CIA, right? 
 15:27: Yeah, so, yeah, so, basically, you know, absolutely for, for the deployment and this perspective, I would focus on like minimizing the risk, risk, and because business critical application, right, and first I would, I would release, I would not release the entire moder modernizing application in the world deployment deployment. 
 15:47: I would migrate and migrate the dep deploy one module at a time, as I said earlier, and each module would go through its own development and testing and deployment cycle before moving into the one, like moving to the next one. 
 16:02: And for the pipelines, every code change, go to the code reviews and followed by automated unit test. 
 16:09: Once those pass, we will deployed to the, document environment for like integration testing or make sure, you know, new Python APIs or RA component work correctly with the existing system. 
 16:22: And after that, we deploy the QA QA team is going to test, going to like all staging the environment that we, that was close production as possible. 
 16:31: So this is, this is where, you know, we perform the end to end testing, regression testing as well, most of the important com important part of the development and compare the out output with the new system and with the new legacy system. 
 16:46: Since that the it's a report platform, I would verify the same both systems generate same result or same input data before, you know, considering the release. 
 16:55: And once QA sign off, I would involve, you know, business users or UAT, UAT because they are no business schools better than anyone's, and they, you know, they validate, validate critical, special compliance reporting application. 
 17:10: So I guess, yeah, there's, this, this is I can say 45 and and the department and I will take action on that. 
 17:18: OK, let's suppose, during the security scan before release, it was found that the public facing services have the permission to financial and tax documents and. 
 17:36: Like we have to release tomorrow. 
 17:37: So then what critical features are you going to go with? 
 17:42: Oh, so if, if, you know, if securities can found some of the public facing service like had access of sensitive financial data or tax documents just before, you know, released. 
 17:53: Yeah, actually, that's, quite, difficult, difficult scenario, but yeah, I would, I would treat that as a critical issue and, would not, you know, proceed with the release until we understood the resolve the problem because protecting the sensitive customer data is more important than, that, you know, meeting the release date and, first I would, Confirm whether the findings validate or not. 
 18:18: Understand which service API endpoint has extensive permissions, and then, you know, then, then I can say I, I would investigate why those permissions were granted and determine whether, whether it's a configation issue or authorization issue or mistake in the application logic. 
 18:36: And once, you know, once I identify the root cause, I would immediately restrict the exit by applying the principal or the lease privilege. 
 18:43: So the service, only the only, only you know permission is actually needed. 
 18:48: And after making the changes, I will work with security and security teams to rerun the security scan and verify that is, that, that the issue is being resolved or not, that, that no business functionality has been affected or not. 
 19:02: And yeah, actually, in the initial days, we also faced this kind of implementation issue, rule-based detect and visibility compliance issue. 
 19:10: So, yeah, that's how I know why we have fixed this. 
 19:15: OK, Mi, what are your thoughts on AI? 
 19:18: See, AI is going heavily used by police, by engineers, right? 
 19:25: Velocity is increasing, but what about quality? 
 19:28: And I've seen people, like doing a lot of code using AI, and if they're asked like why it's failing. 
 19:36: Yeah, they are saying we don't know, yeah, definitely cuts on the open side and the cloud, it's a really, you know, great, great models have. 
 19:46: And I think the AI is great for productivity tools, but I don't think it replaces engineer judgment. 
 19:54: It can definitely help the developers with the guide faster and generate unit test like cleaning unfamiliar code, or if I write, you know, like, like 2.5 months, a half month, back a code. 
 20:08: I, I don't, I don't know how about the logic, so I can use AI for that. 
 20:11: Can, can you reexplain to me that the logic and. 
 20:15: That's for the speeding debugging that's also, you know, help us to development velocity, but when I, when it comes to quality, I don't believe it should be accept AI generated code without reviewing it. 
 20:26: And the engineer is still responsible for understanding the code, validating the understanding, the, I can say validating the logic, checking the age cases, make sure it meets the security of business requirement because, sometimes AI gives, I can say. 
 20:43: Not, not, it gets, they give us the code, but it's not the match, the security and our like policies which we are following our code format we are following. 
 20:53: So we have to make sure this is actually, not, not, not at the age of the our, I can say project and we follow the, all the formats and all the rules and relines of the project, make sure so ID check always whatever I could, taken from the AI. 
 21:09: And yeah, my, my view is that AI helps us spend less time and repetitive tasks, more than time on resolving complex business problems, designing good architecture, making, making the technical decision is easier to with the AI. 
 21:25: So I see AI, AI is as sometimes, some, something that improve developer productivity. 
 21:31: But quality still depend on the good engineer practice and human review. 
 21:36: So yeah, that's, that's my thought process. 
 21:38: And that's my. 
 21:39: Yeah, sometimes we use it for productivity, but it uses. 
 21:44: Yeah, definitely, I totally agree. 
 21:48: OK, can you please share it again so we can have one handsome. 
 21:56: The issue. 
 22:05: OK. 
 22:06: Are you able to see my screen? 
 22:10: not yet. 
 22:11: No, I can see it. 
 22:13: are you sharing the chat. 
 22:14: Can you please check? 
 22:36: OK. 
 22:39: OK. 
 22:42: So is it what I can say. 
 22:45: Is it, yeah, it's a system like the application right in.net this is just a reminding myself OK, you're reading. 
 23:06: and to react and while. 
 23:10: OK. 
 23:13: So is it I have to. 
 23:16: Work on the front end or in the back and side and the starting. 
 23:25: OK. 
 23:28: So for this, Yeah, for this problem, I can say this is actually a legacy application, right? 
 23:35: This is your, like this is a migration thing I can say the Lexia patient is in the.net and she's up and Angler and the new application in the Python and no GS and React and I think it's want to introduce AI gen to speed development but AI should only assists the same task, OK. 
 23:58: OK for security text number is OK. 
 24:03: You know. 
 24:05: OK. 
 24:06: Understood. 
 24:08: So, OK, so where do you want to write it? 
 24:12: Like how can we implement this and that is you're going to cover it? 
 24:17: I want to see. 
 24:18: Right, the architecture, right? 
 24:23: what would not code it from the scratch. 
 24:26: Give me the implementation details and cover all the experts, OK. 
 24:32: This is OK, so for sure, first of all, my approach would be separate the business critical workflow from AI assistant workflow, not verbally. 
 24:46: I mean, I wanted to write it. 
 24:49: OK, let me, should I use notepad or, or draw any architecture? 
 24:55: You are, we are comfortable to use anything. 
 24:58: OK, let me draw your architecture. 
 25:00: OK. 
 25:10: OK. 
 25:30: me. 
 25:46: You this. 
 26:13: And deer and. 
 26:18: And. 
 26:19: it So basically the acti years. 
 26:42: I will go to authenticate and read. 
 26:53: And The request is entered through the react-based application. 
 27:03: The UI basically validated, send it back to the rusty place. 
 27:09: OK. 
 27:11: OK. 
 27:30: OK, so this is the inside. 
 27:34: Ma. 
 27:48: OK, so basically API gateways, AI gateway they act as a single entry point and it's route that requesting. 
 27:59: request to the appropriate back end service and can also provide the load balancing security and request. 
 28:12: And for the back end side this is actually where the main business logic run. 
 28:16: And And basically you know the back end validate the request, applies the business rules and store the task information but. 
 28:29: Good afternoon. 
 28:31: I'm going to repeat that. 
 28:34: Let me commute first then I can continue. 
 28:43: You know just a snake can be. 
 29:04: Please don't judge me, I'm not good at drawing. 
 29:12: It always looks like I can manage. 
 29:16: Because we are more on the cold side, not in the. 
 29:21: Fake muscle. 
 29:47: OK. 
 29:49: He went on books and and cues. 
 29:52: I. 
 30:28: OK I like OK. 
 30:44: OK. 
 30:49: I work for. 
 31:02: OK It's gonna be monitoring. 
 31:34: You OK. 
 32:33: The first of all, the end user. 
 32:37: Basically this is a business user who, who has an application. 
 32:42: It could be customer complies, analytic officialal user, internal employees. 
 32:48: They can access the system through the web browser. 
 32:51: And why we start like with the user because every request oriented here, right? 
 32:56: And second is React intake UI and React React basically React application is front and rear user interact with the system and it's basically responsible for displaying forms, accepting user input, showing the dashboard, displaying the reports, showing the approval status. 
 33:16: And and basically react, you know, react application does not contain business logic. 
 33:20: It's basically only collect the user input and send it to the back end. 
 33:26: I basically, for example, users submit their new claims request to the reactiveI. 
 33:30: So this is all about renting and third is actually authentication. 
 33:34: This is JWT. 
 33:36: Actually, before user can access that application, they must authenticate, the user logs in, in the user using or or or or or another identified provider. 
 33:50: After successful login, the servers generate the GW token. 
 33:55: Every API request into this token, and that backend basically validate the token before, you know, processing the request and would would be an API gateway and load balancer. 
 34:06: And basically this is API, API gateway is a, a single entry, for all back and requests. 
 34:13: It's basically responsible for, routing, request, authenticate valid validation, rate limiting, SSL, termination, unlogging, load balancing, anything, and, Fifth one would be Python and backend service. 
 34:29: Basically, the Python, service contain only code logic and their responsibility include like valid, validate the request exe including the business rules, reading the, writing the data, calling other service, returning the response on the front end. 
 34:46: For example, like create new requests and need reports, this kind of, you know, example I can see. 
 34:51: And 6th 1 would be next, node GS service and at least some service may be implementing Node GS, for example, a motivation, motivation service but we agree with the Node GS. 
 35:01: And real-time update and that's also I think best fit for with you know just web socket communication, email service, background processing, and this basically demonstrate the entire so enterprise can be have multiple technology working together. 
 35:19: And the 7th would be like business rules like engineers and basically this is one of the most important components instead of HDB instead of spreading the business logic across the bus multiple APIs all business rules are centralized here. 
 35:35: I can give you an example like should we, should this request require manager approval or not, should tax can be calculated or not, and in this, customer eligible or not. 
 35:47: So this basically make the application easier to maintain because changing business rules only require updating the, updating one piece, and it would be like, would it be? 
 35:58: MoDB like store all the, all the, all the application data and typically, you know, collect includes like users request, approvals, audit reports, and the backend reads and write data to the MongoDB. 
 36:12: And actually then, then, then next is event outbooks, outbox basically instead of you know directly calling another service after after saving data, we first write the event to outbox table or collections and like save the request in MumgudiB or save the event in the outbox and basically actually this is actually ensure ensure no events are lost in other service temporarily unavailable. 
 36:41: And the next day is event queue. 
 36:44: Basically, the, this is the groundworkers read the, read the event and our books and publisher them into the event queue and other service to satiscribe these events like sending emails generated reports. 
 36:59: And last one, I think this is the major part which is the AI genetic service and the AI service is send the developer, assist the developer and users generally the documentation such as the unit test, migration analysis, valerate code, and however the AI does not make final decision critical as you said in earlier we discussed and. 
 37:23: the approval workflow as well and if the AI agent is changed, it does not, you know, it doesn't, does not, go through, go through the approval process and AI generate the code AI AA review, and I, review, then security team review it, only then we can accept it. 
 37:43: So this is like approval workflow medical decision always required human approval. 
 37:48: And human approval as well that this is a step incrementally for sensitive operations such as like tax calculation, payment processing. 
 37:57: Sometimes, yeah, I can't, can be failed, so we have to test manually and then execution changes as well while like this code in the, I think I can say once approved code is merged, instructions code is applied, business logic becomes active. 
 38:14: And we have to also use monitoring and logging alerts because once the application is running, we continuously monitoring and application logs, API logs, data and data logs and performance, metrics, error rates, CP memories, and, CICD. 
 38:32: deployment and pipeline, it's also going to be put in this place. 
 38:36: Every code, you know, change, follow automated, deployment pipeline like typically stage like code comment build, then unit test going to run code quality checks also going to run, security scans. 
 38:46: So there are multiple stages in the CIC and yeah, this is actually end to end flow and it I I guess I, I'm fulfilling the requirement. 
 38:59: Sorry, I guess, I got actually, this is all about my like the flow and also this will fulfill all the requirement or the as you asked. 
 39:13: Yeah, yeah, it does, it does, OK. 
 39:23: What are you using for observability? 
 39:25: We can use CloudWatch if we are using AWS. 
 39:27: We can use CloudWatch and yeah, that's a, that's that will give, give us like event, I can say logs and the metrics and CPU, CPU or the docs as well. 
 39:40: So I definitely use CloudWatch and all ready tools and application log is also give us, yeah, cloud watch is more I. 
 39:52: OK man, I think, I'm good from my side and become one of the career. 
 39:57: So thank you so much for your time. 
 39:59: Thank you for. 
 40:00: Yeah, thanks and nice talking with you. 
 40:03: OK, yeah, it was everything. 
 40:05: Thank you. 
 40:05: Thank you. 
 40:06: Have a nice day. 
 40:07: You too. 
 40:07: Bye bye. 
