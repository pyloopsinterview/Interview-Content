0:01: Hey Xiong, how are you? 
 0:09: I hope I'm audible. 
 0:10: Santosh. 
 0:11: Yeah, can you hear me? 
 0:12: Yes, I can hear you. 
 0:13: Good afternoon. 
 0:14: hold on. 
 0:16: I can hardly hear you. 
 0:17: Oh, you cannot hear me? 
 0:19: Oh yeah, yeah, now, now it's working. 
 0:21: OK. 
 0:22: Hey, yeah. 
 0:24: Hi, how are you? 
 0:26: Pretty good. 
 0:26: Pretty good. 
 0:28: or depends on your location. 
 0:30: Good good morning. 
 0:31: Good afternoon. 
 0:32: Good afternoon. 
 0:32: You can say it's 1:30, like, it's like 12:30 CST. 
 0:37: so we are in the same region. 
 0:39: OK, got you, got you. 
 0:42: give me a second. 
 0:46: Arno will join us. 
 0:49: he, he said he's going to join, join us. 
 1:04: Hello, am I audible? 
 1:06: It became a couple. 
 1:10: Couple of minutes, Well, while we're meeting, just to, briefly, Give me like a 2 minutes to introduce yourself, especially the journey of, dynamic 3C5 for finance and the operation development. 
 1:30: Sure, sure, sure, yeah, like, so yeah, like, hi, this is Santosh, and I'm working as a senior lead Microsoft and then the advanguard, and or I would say I have a lavi years of experience working with the Microsoft technology stack with the majority of my experience focused on the, dynamics is finance and operations, dynamic is regards CE as our integration services, our platform, and the enterprise application architecture. 
 1:58: And then my current role at Vanguard, I would say I work as the technical lead for a team of 6 developers where I. 
 2:05: I'm responsible not only for development but also for the technical architecture solution design, as well as the code reviews and mentoring the developers, and I would say like I would like to work closely with the, owners, functional consultants. 
 2:22: I would say, as well as the business analyst, QA teams and stakeholders to understand the, business requirements and translate them into a more scalable, secure, and maintainable enterprise solutions. 
 2:35: And if I talk about one of my biggest initiatives I have led it that was the vanguard was the, modernization of the procure to pay and financial management platform as a part of the like organization. 
 2:48: The cloud transformation program where we have implemented and like what I say like implemented and extended the finance and operations across models like accounts payable, accounts receivable, general ledger, as well as the proper brand sourcing, vendor management, and also the fixed assets. 
 3:09: Since I would say it was a large enterprise environment, we also had to like integrate DC65 with. 
 3:15: Multiple, external systems including SAP Service now, and, if I particularly talk about from my architecture standpoint, I would say I designed overall integration strategy using the Azure logic apps, Azure Servicebos, rest ABIs and older services. 
 3:31: We are here we follow the, service like event driven architecture because it had was like I would reduce, system dependencies, improve scalability, and make integrations easier. 
 3:42: And particularly if I talk about my development side, I, I like, I guided the team in implementing the Microsoft commanded extension-based customization using the H++ as well as the electronic reporting, workflows, bad jobs by making sure. 
 3:58: Like we minimized overlay layering and followed around the Microsoft best practices, and I would say like I also own a type of delivery courses including the Bachelor refinance and planning and all and also like security and I would say governance were also a key part of my responsibilities work with the compliance and security team to implementing the security side as well, and I would say like one project I am particularly proud of was like redesigning our vendor invoice automation process. 
 4:26: And because like the existing process involved multiple manual approval steps and cause delays in, in like invoice processing, I like where I like the design of workload IM solution from like 65 workflow and as integration. 
 4:40: So yeah, that's pretty much about myself like what did I did so far in my career. 
 4:44: So yeah. 
 4:46: Mhm. 
 4:47: OK, great, great. 
 4:50: I think the, He's not, he's offline. 
 4:56: We'll see, let's get start. 
 4:59: first of all, I just want to, Questions on the integration. 
 5:07: so for, Primarily we're talking about inbound integration, So for the inbound integration, what options do I, do we have, are they, or put this way, for if you're asked to, create an inbound integration, what, what's your approach, List all options, are they, tell me, are they synchronized or asynchronized? 
 5:56: OK, got your point. 
 5:57: Got your point. 
 5:58: So like when I design an integration for the financial operations, the first thing I try to understand is the business requirement rather than like jumping directly into the technology. 
 6:10: So for this I really start by Like asking a few questions like, like where the data is coming from, whether the integration needs to be real time or bad, or like how much like data we are expecting and what the validation rules are. 
 6:24: And once those requirements are clear, then I move decided the most suitable integration approach. 
 6:31: So like if the source system needs to send the data to the D65 in the real time, so I generally like prefer using the custom services slash APIs on the on the or radar like depending on the business scenarios, for example, like if another enterprise application needs to create or like. 
 6:49: Update the records instantly. 
 6:51: You know, the APIs are usually the right choice because they provide immediate processing. 
 6:56: And if the requirement involves like a large volume of what I say, like the transactional or master data like the customers, vendors, products, or any data that I normally recommended using the DMF that is the data management framework. 
 7:11: It supports high-level inputs, data validation, staging, error handling, and all. 
 7:17: And for integrations involving like multiple enterprise applications such as the SAP ServiceNow or any banking systems, with there I prefer using the Azure integration services, especially the Azure Logic apps and the Azure Service like, like, like at Vanguard, this, this was our primary architecture for the logic steps like handle documentation, transformation, routing like wire service bus like. 
 7:44: Like, like, just enable the Synchronous messaging and I would say like I also like pay close attention to the security and monitoring where we secure the indictations using the Microsoft and prior authentications, as well as the man identities where application HD-based communications and we all those access controls are required. 
 8:07: So yeah, that's my like with the extent with the education sector yeah. 
 8:13: Mhm. 
 8:14: Yeah, you mentioned the customer service and the DMF. 
 8:18: What other options do we have? 
 8:21: OK, apart from the customer services and the DF, I, I would say like, there are like, I would say several like other options available and the choice definitely depends on the business scenarios. 
 8:34: For example, like one common option is old data. 
 8:37: So, where I typically use the old data when the external application, like needs to perform the standard current operations on entities and the data. 
 8:46: Data volume is like relatively moderate. 
 8:49: It's a good choice, I would say for the what I said for the real-time indicators wherever the business needs immediate access to the DCD data. 
 8:58: Another option is like the recurring integrations which work on the top of the DMF, and this is very like useful when the external systems need to exchange files with the DCTF on a scheduled basis without any manual intervention. 
 9:11: And also we also like use we have the business events which are very useful in the event driven architecture. 
 9:18: So instead of like analy systems continuously like what I see using the like pulling the B65, the application can publish an event whenever a business section occurs. 
 9:29: And for like more complex enterprise integrations I generally recommend the logic apps, long variations of business. 
 9:37: So yeah. 
 9:42: OK. 
 9:44: So, For When, when can, when do you, give me a typical samples when you use the logic app. 
 9:59: OK, for the logic apps, OK. 
 10:02: like, let me, like, give you one, like, example where, like, one good example like as for my like previous experience where like where was our integration between the FNO and the external systems like, SAP, and, and, internal financial operation. 
 10:19: So like whenever a vendor invoice was like approved in the dynamics where we need to needed that information to be, what is synchronized with the staff and And a few downstream financial systems. 
 10:32: So instead of like building point to point integrations, there we use the Azure logic apps as the application layer and like the way it worked was that the DST5 generated the what I see the business event or like expose the required data and the logic app picked up that particular information and like inside the Logic app, we perform the, data transformation, then validated the mandatory fields, applied like, like a few business rules, and then routed the data to the appropriate target systems and in cases where the immediate processing was not required or we like wanted any like any better residency, we also placed the message on measures of his birth. 
 11:21: That we set for another downstream application was like temporary enabler. 
 11:25: The message remained in the queue and could be like what is the process once the target systems become available. 
 11:31: So yeah, that's where I use the logic. 
 11:34: Mhm. 
 11:36: Well we have a, a large volume of, which one you are going to choose. 
 11:43: OK, OK, OK. 
 11:46: If I like just to talk about, a very large amount of data, that like I would say that my definitely choice will be the DMF rather than or data or logic app. 
 11:57: Let me clarify you. 
 11:58: Like, the I'm using. 
 12:00: The main reason is that the, DMF is specifically designed for the high volume data processing. 
 12:08: So it supports the staging tables, bulk imports, as well as the parallel processing. 
 12:15: So if I need to import like hundreds of thousands or, or like even the millions of records such as. 
 12:21: The customers, vendors, or like any historical, financial transactions data. 
 12:27: So here I would say the DMF is much more efficient and scalable. 
 12:31: I like, basically I really like avoid using the old data for very large data sets because I would say like it's more suitable for the, the real-time transition operations with the moderate data volume. 
 12:44: So yeah. 
 12:45: OK, OK, good, good, very good, so, since we're talking about, we're here, so if I'm having, a performance issue, the, for example, the, the customer service interface. 
 13:07: You know, the, the, the, the, customer service, if we're facing a, a performance issue, what's your approach? 
 13:19: OK, got your point. 
 13:20: So basically performance issue is one of the issues we are facing. 
 13:24: So like if I am facing a performance issues with the customer service. 
 13:28: I would say I don't immediately assume that the problem is like the they justify itself. 
 13:34: So like definitely my, my first step is to like get identify like where the bottleneck actually is and where for this I usually break it down into I would say like like 44 like I guess the client application, the net network, the service layer, and last one is the slow down. 
 13:54: What, what's the first one? 
 13:56: The first one is the client application. 
 13:58: -huh. 
 13:59: Then the network. 
 14:01: Then the 2nd 1 is the network. 
 14:03: Then the 3rd 1 is the service layer, and the 4th 1 is the D65 back end. 
 14:10: OK, what do you mean service? 
 14:14: OK, so basically if I talk about, the, if ID what is service they are in apart from my four areas, so let me, let me, let me clarify you, like it is basically I would say the interaction between the, finance and operations and the external applications. 
 14:32: So like, like instead of like the external systems accessing the database directly, like they communicate with the D65 through the service layer did you got you get my point here. 
 14:43: , yeah, let me, do assumption, we know it's a DCC5. 
 14:53: What, what, what area do you are you going to, approach? 
 14:59: OK, OK. 
 15:00: OK, OK, so for delivery, like, if like, if you already know, like the, know the issue in the inside the, D65FNO, so then I would like, like I would say narrow my investigation to the applicant itself. 
 15:14: So the first area I would look at is the access. 
 15:17: This this is logic behind the service. 
 15:19: So here I would like to review the implementation to see like, like if there are any unnecessary loops or any, any inefficient coding patterns we have or like any like the multiple data which is all that can be optimized. 
 15:34: So the and the second area is the database queries where I would check like whether the queries are literally only the record data or whether the approciate indexes are being used or like whether they are like, like any full scans or expensive joints causing delays. 
 15:51: Next, like I would review the USS exhibition to see whether the service is consuming excessive CPU or memory of multiple requests are. 
 16:01: Like, like competing for the same resources and I would like also check whether the services involving invoking like any synchronous processes such as the workflows, business events and all. 
 16:14: And definitely another important area is the data volume because sometimes like the services like trying to process thousands of records in a single request. 
 16:24: So in that case I would implement the paging issue and batching or like filtering so that each request like like handles a manageable amount of data. 
 16:33: So yeah. 
 16:34: Mhm, mhm. 
 16:35: OK, OK, good. 
 16:39: come jumping to a different topic, the batch, batch, services, and, to come to want you to create a new batch, what the two mechanisms, you, what option do you have? 
 17:01: OK, OK, OK, I got your point. 
 17:03: I got, so, like, as for my understanding, like if I like need to create a, new batch process in the I don't know, there are like two, like two primary approaches that I manually consider. 
 17:16: So the first and the most common approach is like using the, operational framework which is like the Microsoft commanded approach for like developing a new batch processes. 
 17:28: So in this framework we separate the Solution into like different components like the the data contract service class and like the controller class. 
 17:38: So here like the business logic like basically relies in the service class while the controller handles the execution scheduling and like whether whether the process runs interactively or at the best. 
 17:51: So here I prefer this approach because it's more clean, scalable, or easy to maintain. 
 17:58: It also supports the parallel execution and batch scheduling. 
 18:02: The second approach is like using the like run-based batch framework. 
 18:07: This is the other framework, and you will still like find it in many I guess implementation. 
 18:12: It basically allows us to create the bad jobs with the dialogues, pack and and pack methods, and also like execute them like through the batch framework. 
 18:23: I would say like, although it's like still supported, like I generally use it only when the enhancing existing funcility that was like already built using the run-based patch, so yeah. 
 18:36: Mhm, mhm. 
 18:37: Good, good. 
 18:41: So, another development question is, when we have, like, transactions, to the database, we have used, in X++, we use TDS begin, TDS commit, and so on and so forth. 
 18:59: how do you prevent those becomes unbalanced? 
 19:04: OK, OK, OK, got your point. 
 19:07: So, like, like, like I would say like there's like very, like very important aspect for the expressive development because if tedious begin and tedious commit become like unbalanced, it can like leave the transitions open. 
 19:21: Cause a lot of logs or event results in one time errors. 
 19:25: So in my deployment development like I always make sure like that every begin has a corresponding GTS commit. 
 19:32: So I typically like wrap the transition inside of triage block. 
 19:36: And if everything executes successfully, I like come back to the transaction. 
 19:41: Sorry, sorry, slow down. 
 19:42: You wrapped it with the what? 
 19:44: Oh, OK. 
 19:45: So I like, I typically like wrap the transaction inside the track catch block. 
 19:52: OK, yeah, and if everything like executes successfully, I commit the transaction, and if an exception occurs, I, I like allow the transition to roll back automatically by, by throwing the exception or handling it appropriately and. 
 20:10: Here I also like avoid writing the the code that exists the transitionally using a written statement or like conditional logic before reaching the DS commit because that's one of like one of the, I would say most common reasons transition become unbalanced. 
 20:29: And apart from this, like, I also like to try to keep the transaction scope as small as possible. 
 20:36: Like I perform validations before entering the transaction, and then only the actual database and so update or data operations are placed between the, between these, and I think this reduces the log duration and improves the overall system performance as well. 
 20:54: OK, OK. 
 20:59: So, I, I saw I you joined. 
 21:02: do you have any questions, before I move on? 
 21:07: Yeah, I don't know, yeah, Sean, if you, if you started, I, I joined late, sorry, client meeting, but, Santosh, can you give me a background problem is that about your overall work experience? 
 21:22: Yeah, yeah, sure. 
 21:23: So basically, like, as you know, like, I have 11 years of experience working with the microtechnologies. 
 21:31: Majority of my. 
 21:32: Experience focused on the Apinoite and dynamicy as your integration and like recently I worked as a senior lead Microsoft like like lead at Vanguard where I led a team of like 6 developers where my responsibilities go beyond development. 
 21:50: I where I own the technical architecture, design, code reviews, as well as like mentoring the developers. 
 21:58: And also like end to end delivery of enterprise CRP solutions. 
 22:01: I would say like I would like I work closely with the donors functional consultants as well as the QA teams to make sure the solutions we deliver and I both like the business schools and like Microsoft best practices and so yeah like that's that's a like a little bit before that, yeah. 
 22:23: OK, and then trauma, And that's all. 
 22:32: so. 
 22:33: In the last role, what are the, the models that you have implemented for FNO in your last project? 
 22:42: OK, if I talk about like my, like, like major, like major models, I would say I like I primarily worked on the profile. 
 22:52: Finance and procurement models and the major models I have involved in the with the general ledger accounts payable, as well as the vendor management, fixed assets, as well as the financial management side. 
 23:06: So yeah. 
 23:09: OK. 
 23:10: And How many? 
 23:16: Companies you had configured in your FNO system. 
 23:21: OK, OK. 
 23:23: OK, I got your point. 
 23:24: So if I talk about like, as per my understanding, like in my wellguard implementation we had like, like multiple legal entities that is like configured in the FNO environment. 
 23:34: So I have like, I don't like directly on the, functional sector of creating legal entities, but particularly from a technical and architectural perspective, I would like, I worked like across around 8 to 10 legal entities. 
 23:46: It is that like supported different business units and the financial operations. 
 23:51: So like from like our development pers standpoint, one thing we always kept in mind that was like company specific versus any cross company processing. 
 24:01: So whenever we were like developing the integrations for any bad jobs or like any custom services, we made sure that the, solution like respected the, current legal entity and if a business process required working across multiple companies, we use the concepts like the cross-company queries or the change company and the actress whenever I approach it. 
 24:26: For example, like some of my, like my, like of financial reporting and Intention scenarios required like collecting data from multiple legal entities and sending the consolidated information to down, downstream the system. 
 24:40: So, in those cases, we designed the solution to process the, each legal entity correctly while maintaining the proper data isolation and security. 
 24:49: So, yeah. 
 24:52: OK. 
 24:54: How do you, how do you make sure that, yeah. 
 25:01: The customer, vendor accounts are shareable across legal entities. 
 25:10: Mhm. 
 25:11: OK, OK. 
 25:12: OK, if I need to make sure like, basically, like I would say like the way we make customers and vendors like, shareable across the legal entities is by using the, like the global address book along with the, with the like the party model. 
 25:29: So basically, the, as you know like the global address book stores the, the core information for our customer. 
 25:36: vendors such as the names, addresses, contact information, and any party details, that means like we don't have to like create duplicate records for like every legal entity. 
 25:48: Then if the entire customer or vendor like needs to transact with the multiple companies, we associated that same party record with the legal required legal entities. 
 25:59: And like from technical perspective, like when we are developing customizations or integrations, we make sure we replace the party record and global entities correctly instead of like creating like any duplicate customer or vendor data, and we also like making sure like that any integration respects the legal entity context while still leveraging the shared master data maintained in the global address book. 
 26:27: So yeah. 
 26:31: OK. 
 26:34: Kong, you can continue. 
 26:35: I'll probably ask. 
 26:37: OK, yeah, OK, thank you. 
 26:41: so come back, to the, performance, So what to your available when somebody say there's some performance problem. 
 26:54: OK, what's the procedure are you going to take? 
 26:57: hm, OK, whatever. 
 26:58: So like whenever like someone tells me like there's a performance problem, so definitely my first response is that I don't like start optimizing immediately. 
 27:07: I first try to like identify exactly where the bottleneck is so the performance. 
 27:12: Issues can like come like from different layers so I prefer to take a structured approach. 
 27:17: So if we have already confirmed the issue within the FNO, I start by checking whether it's related to the aspects of business logic, any database queries, batch processing. 
 27:28: So here I review the code to see like if there are any unnecessary loops or any, repeated database calls or inefficient joints. 
 27:38: like, like, like, like that are like retrieving more data than required. 
 27:43: And apart from this, like I also like to verify that we are using the site-based operations wherever possible instead of like processing records one by one. 
 27:52: Next, I also analyze the the database performance where I check whether the appreciate indexes are being used, whether there are any blocking or logging issues and whether any like wrong running queries are affecting the response times. 
 28:07: And like I also like to check whether the delay is caused by. 
 28:10: But particularly for the integrations I like, check whether the delays like scheduled by a synchronous communication with the actual systems and if the, if that's the case, I evaluated whether we can move to any asynchronous support using the Lio services or like redesign the integrations to improve the responsiveness. 
 28:29: So yeah. 
 28:30: Mhm. 
 28:32: what you are going to use to identify the, those, Diagnosis. 
 28:42: Use, OK. 
 28:43: You're going to use, OK, OK, OK. 
 28:45: So, like, like if I'm like, like troubleshooting, like, like a performance issues in the, I like I use like different tools like depending on where I think the issue is coming from. 
 28:56: So my first tool is the, I'll see that is the life cycle Services where I use, use the. 
 29:02: Environment monitoring and the aspirin sites to check the overall health of the environment or any longer queries and other perform metrics. 
 29:12: And if I believe the issue is in the access code, I use the trace parser. 
 29:18: This is one of the most valuable tools because it gives what I say the detailed education trace and has also helps to identify risk methods, data calls or operations are consuming the most times. 
 29:31: And for, for the custom code, I also use the performance timer and the Visual Studio debugger to like measure the execution time of specific methods and understand where the delays are occurring, so yeah. 
 29:45: Mhm. 
 29:48: OK. 
 29:54: Yeah, very good. 
 29:59: Checking my notes, Yeah, That's so pretty much, I, we wanna ask, I want, I wanna ask, I, I think I'm good right now, and, I'll ping you, X, I have a call and I'll ping you once that call wraps up, OK, so we can chat about it. 
 30:27: OK, great. 
 30:29: All right, thank you. 
 30:30: Thank you, San, for your time, yeah. 
 30:34: OK. 
 30:36: You 
