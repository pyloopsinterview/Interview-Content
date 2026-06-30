0:00: To join the call, but somehow it's taking me like pull back a lot of time. 
 0:06: We are sorry for the inconvenience you are facing. 
 0:11: Yeah, no, no worries, sir. 
 0:16: Sure, sure, yeah, how are you guys? 
 0:19: But And I'm also playing tech. 
 0:24: Yeah, let me introduce myself. 
 0:27: So this is that I'm working as a senior architect for one of the projects from RSC. 
 0:34: So this is for a solution architect role, Where we use everything, taking the meditation and develop our rules. 
 0:45: It's a combination of both architect and development and also we try to interpret it. 
 0:52: So that's the introduction for the I can start with your introduction. 
 0:57: OK, sure. 
 0:58: So hide. 
 0:59: Like, like this is Raj, and I have around, I would say 10 years of experience working with the, Microsoft Dynamics. 
 1:07: This is GFC power platform as well as the Power apps, Power Automate and.NET, Azure, as well as the ALover and Power BI, and over the years I have worked, I would say, across multiple industries. 
 1:22: Sure, sure, no worries at all. 
 1:29: OK, so yeah, I would say like over the years I have worked across, multiple industries including the, healthcare, financial services, the insurance and telecommunications where I have like, been involved in the, company project life cycle starting from requirements gathering and pollution design. 
 1:51: And all of the way through the development, the integrations, testing, deployment, and the production support as well. 
 1:59: And I have like recently I have worked as a lead dynamic disease developer and at, at the Dignity Health where the dynamics also as a like a central platform for the patient and customer engagement. 
 2:13: And in this role, I design and develop the dynamic to justify solutions, build the custom entities and This process develop a lot of plugins using and and SDP creating the power automate workflows and also building the power Pages portals and implementing implement the like the integrations with external healthcare systems and all and one of the key areas I have worked on is building a secure self-service solutions using the Power PGs data rules and dynamics and, from political. 
 2:53: And as an as an integration perspective, I have, have been working with the Azure functions, logic apps Of CP management and all and, in addition to development, I, I actively participate in the like the architecture discussions, code reviews, troubleshooting the production issues, also mentoring the junior developers and, working directly with the stakeholders to prostrate the process requirements and. 
 3:21: scalable technical solution. 
 3:22: So yeah, that's, pretty much about myself. 
 3:24: So what should I have like, pretty much do no, no, like I'm working as a remote like but my contact has been a little bit dignity help last week. 
 3:38: OK, I'm working. 
 3:40: All right, which location? 
 3:41: Oh, I'm, I'm working as a remote. 
 3:43: I would, I, I see. 
 3:45: I'm working as a remote. 
 3:52: No, no, I'm currently in Mcanee, Texas. 
 3:57: Oh yeah. 
 4:03: since this is, the tech, mostly technical questions and as well as, It some developers questions. 
 4:13: So total 4 years of experience in 10 years, right? 
 4:17: Yes, absolutely. 
 4:21: It's around, I would say, I would say totally around like 8 years I would say. 
 4:29: So you, you have 10 years in US or all 10 years in like some of them in US, some of them in. 
 4:37: No, no, like I have like a field basically I started like from my career from US only from, like my first company was like a charter communication as a software developer. 
 4:48: It's in Stormport, so I have started my career in the US itself, yeah. 
 4:54: OK, thanks. 
 4:59: can you explain me the recent plug-in which you have? 
 5:01: Sure, sure. 
 5:03: So if I talk about my just recent plugin, so yeah, hype like and my liking, basically I have written like, as you say, like multiple plug-ins based on the different business, but one example that I usually like to discuss from my recent project that is like where one of the requirements was like that when whenever a patient refer. 
 5:23: Record was created or like updated where we had to perform several validations before the record could move to the next stage. 
 5:32: So we have, we needed to verify that all the like the the validatory patient information was available and we need to validate the business rules and like to automatically populate some of the like the calculation. 
 5:46: fields based on the related reports and since these validations had to happen immediately before the data was permitted to data was so where I implemented like the pre-operations that plug in their main main basically the main reason for choosing a plug-in was that the like logic had had to execute within the. 
 6:11: Same transaction ensuring the data consistency and preventing the invalid record from being saved. 
 6:18: And another scenario was when when like a referral status changed to a code after the status update the actually needed to create a some of the let's say a follow-up task, update the the related record. 
 6:34: write the audit information and also the trigger downstream integration with some of the, the external healthcare systems. 
 6:43: And in another case, we needed to prevent the, the duplication records based on the specific business criteria and for that, I also use a pre-validation plug-in because it executes before the platform. 
 6:57: Performs the database operation at all and what is the do you differentiate? 
 7:05: Sure, sure. 
 7:07: So basically pre-validation and the PLA operation is basically, when is when like the exeitude in the the dynamics event pipeline and what kind of business project they are best suited. 
 7:20: So, so basically the pre validation is the valid postage as it runs before the platform the platform performs security checks and before the database translation starts and on the other hand, like if I talk about the pre-operation, it basically runs after the security checks have passed but before the data is actually written to the database so that's the major difference. 
 7:44: OK, now, you said, you have written out like you know preoperation right to perform some vigations. 
 7:53: I mentioned it is, it is. 
 7:56: From which entity it has been. 
 8:00: OK, so, basically, I'm, and, and one of my, like I wrote, like basically I wrote a few patients again on the patient refer, basically the patient different entity because the DMB business requirement was that before the referral record was saved, so we have we had to, validate, a lot of, referral record was saved. 
 8:21: So here we had to validate these business conditions like for example. 
 8:27: OK, so you have it done it like, you know, patient, the patient, right. 
 8:35: So I give you the same plug-in. 
 8:37: So you can tell me the same plugin. 
 8:39: I have written it on contact and get it. 
 8:41: Let's assume that you have red it in pre-operation. 
 8:46: I have registered it in contact pre-evaluation. 
 8:50: And we send the data using some API. 
 8:52: We will try to send the data to both entities, same data, and at a certain point of time it will fail. 
 9:01: So the data is set, the data is sent in such a way that the validation plug in which you have written tends to fail. 
 9:10: So what will happen in your case and what will happen in my case? 
 9:14: Will the patient or contact gets created in your case? 
 9:18: OK. 
 9:19: In the pre in the pre-operation will the patient be created and in my pre-evaluation the keep the contact will get created. 
 9:28: OK, I like, I like, I understand your question, like, in my case, like, because the plug-in is registered on to your patient, so the basically the request have already passed the, initial platform validation and security check, and now it is inside the, the database foundation. 
 9:47: So if my validation fails in the pre-operation and I throw and, the Invalid plug-in exhibition exception, then the current create or update operation will be rolled back and that patient record will, I would say, will not be saved in the database. 
 10:07: And if I change any fields in in the target entity before the exception, those changes will also be rolled back because everything is part of the same transaction. 
 10:20: And particularly for in your case, where the same validation plug-in is registered on pre-validation of the contact entity, the plug-in will execute earlier in the pipeline before the main database transition starts. 
 10:37: So, If the validation fails there, I think the request will be tagged, will be stopped immediately, and the, contact record will not even reach the, the pre-operation stage, and here the API will, receive the failure response earlier and the, database will not continue with the, the create or update operation for that record. 
 11:02: So, functionally, functionally, I think in both cases if the plug-in throws an exception, the record will be saved, but the key difference is timing and transition period and in pay validation, the failure. 
 11:18: The record will be saved. 
 11:23: The, the record will be saved just like, like basically, it's, it's like, yes, like the record to be saved in both directions. 
 11:35: So if I update the plugin and so if I perform a creation of a record and the plug-in files on both stances it was one exception. 
 11:50: an exception, like if the same create test causes both plugins start to execute and validate validation and condition fails in both, then yes, both are capable of throwing an exception, but, practically the first plug-in that throws the exception will stop that operation. 
 12:11: So the later full, states will not continue for the same record, I would say. 
 12:19: Yeah, and then the record is particularly, I could see here it's it's gonna be for the as a, as a, as a, especially for the API or NDS scenarios, but I would not record it inside the same paying transaction if that log also gets rolled back down, yeah. 
 12:44: I'm not getting an answer. 
 12:45: Can you repeat it a little bit, so we have a record. 
 12:50: So the contact code is Paresh, Paresh, it's your Raj Paresh Patel, right. 
 12:58: So I'm updating your phone number, updating your company name from XYZ2 NUC because of some, listed failed. 
 13:10: Now, in your case, in your case, in your pre-operational plug-in, what is the new value of the company? 
 13:19: OK, for what was the, oh, OK, so I think, as for this scenario, if the plug-in is running in the, the pre-operation and update this page because I throw an extraction then the, the for the then the new company value will be not safe, so the record will remain within the old company value which is the because the pre-operation. 
 13:44: Runs inside the database transaction and any update coming in the target and entity is still not committed to the database. 
 13:53: So if the validation fails at that stage, the whole update operation is rolled back out. 
 13:59: That means the phone number changed, company name changed, and any other field changes, in that same update request will not be committed. 
 14:08: So yeah. 
 14:09: You look reg. 
 14:13: If we throw an exception there. 
 14:15: Could you please come again? 
 14:19: In the periodization, if we throw an exception there. 
 14:22: OK, if, if, if, particularly for the pre-valuation plugin, if, if available app prove an exception like then, then, then the update stops before it enters the, what I say, and then before you enter the main database transition, so the new value will not be saved, right. 
 14:45: Have you worked on any Israel-based complaints? 
 14:49: Yes, I have worked on. 
 14:52: OK. 
 14:53: OK, so, particularly I have worked on some of the as well like, in my, in my project where especially at the video where I have worked, I would say work with the several services. 
 15:04: It's a part of my overall, platform. 
 15:07: So one of my primary is the Aure services where I have worked with the as your functions we use the other functions whenever we have to, Integrate the dynamics with any external healthcare systems. 
 15:20: I have also worked with the idea of Bo for the, asynchronous messaging and world and the service. 
 15:26: I have worked with the, with the API management where I which has acted as a securely gateway for RS APIs and all. 
 15:35: And also I have worked with the Azure I work for So control and CICD. 
 15:40: So yeah. 
 15:43: OK. 
 15:45: Can you explain to me why did they use as your services? 
 15:48: OK, why did they use as your service was here with. 
 15:53: Mhm. 
 15:54: you are talking particularly about the address of this birth. 
 16:00: Yes, OK, so if I majorly talk about the service bus, so yes, I have worked, a lot of it as a service bus. 
 16:07: So, and, so at that, at that time, we mainly make our implications, very helpful as, reliable and loosely coupled. 
 16:16: For example, in my project where, when, when, when an important event occurred in the time. 
 16:21: Dynamics such as patient referral being approved where we needed to send that information to, multiple external healthcare systems, instead of calling those systems in directly from the dynamics where we first publish your message to measure of business and here, this basically the advantage of this approach in the dynamic. 
 16:43: It doesn't have to wait for the external system to respond. 
 16:47: And once the message is placed on the service bus, the user can continue working and then as your function then need the, message from the secure topic to perform the required versus logic and send the data to the external systems and also, yeah. 
 17:11: In this, in this scenario where, the patient is not approved, so you're sending a, you're sending an event to urgent services. 
 17:23: So Which mechanism have we used to read the message? 
 17:29: OK, for, particularly of the suggestions, as I have, if I talk about the mechanism, I have, I think, as for my understanding, I, I, I, for the, for the patient discharge that is, that was approved in the dynamics, so that it in basically I, I, we use and particularly, as your functions within us, so this was triggered to read the message because. 
 17:56: I would say the flow was that basically the flow was that once the dynamics generated and even for example, when a patient referral was approved here we published a message to the as your service bus queue then and as your function configured with the service was triggered automatically sent to the queue as soon as. 
 18:19: new message arrived where the function was like triggered, I would say automatically without any pooling. 
 18:26: So, and, inside the other function we visualize the messages, perform the required business validations and all of that to all the external healthcare system so the rested years and also, yeah. 
 18:48: Yeah, sure. 
 19:09: I was, so I want to know how it has been triggered. 
 19:13: So is it patient getting discharged or patient? 
 19:16: , a little like. 
 19:21: Patient waiting. 
 19:22: OK. 
 19:23: Oh, OK. 
 19:23: So yeah, got it. 
 19:24: So basically, I, in my, in, in, in our, in our, you know, particular scenario, it was when the patient referral was approved, not when the patient was discharged, because once they, once they, OK, OK. 
 19:42: Mhm mhm. 
 19:44: So, when the patient referral is approved, how do you know that referral is approved. 
 19:51: OK, yeah, OK, OK, got it. 
 19:53: So, basically, like in case like, let's, like, for example, give you one example. 
 19:59: Let's see. 
 20:00: like the patient confirms an appointment through the portal. 
 20:04: So, once the appointment status changes to, confirmed in dynamics, that, that event is published to the Azure services where we don't call the external systems. 
 20:17: Directly from dynamics because that would make make the user we can tightly couple the systems. 
 20:24: So instead of wait wait wait wait wait, let me ask, let me ask her some I have some questions. 
 20:31: So let's take it one by one. 
 20:33: So you will come to the portal at a later point in time. 
 20:37: So you are sending the email to the service first whenever the appointment is confirmed, right. 
 20:46: How, how, how are you sending the event? 
 20:49: OK, OK. 
 20:51: So basically if I talk about like how I'm sending, like basically the event is sent to the address of immediately after the business event occurs. 
 21:01: For example, whenever a patient confirms an appointment, the status and dynamics changes to confirm and at the point, our business logic publishes a message to the services. 
 21:11: And it is not based on a, scheduled job or a fixed time interval. 
 21:15: It is event-driven. 
 21:16: In our implementation, the message is published as soon as the transition is successfully completed. 
 21:22: And after that, the azure function with the service was triggered automatically picked up the message almost immediately the processes is like, did you use plug-in tool? 
 21:33: Did you use auto flow? 
 21:34: Did you use workflow? 
 21:35: How did you do that? 
 21:37: OK, so yeah, mhm, I got it, I got it. 
 21:40: So yeah, I basically, I use the in this and I use plug-in to publish the messages to your services because the reason, because the design is that the business event such as an appointment being confirmed happens inside the dynamic device. 
 21:54: So yeah, I use the plugin. 
 21:58: So is it synchro? 
 22:01: OK, yeah, basically if I talk about the plug-in set it's totally, it is using asynchronous post operation plugins, yeah, yeah. 
 22:10: As port for the services that you have created, is it production? 
 22:15: Is it initially you created as data, right, in the de in the dev resource. 
 22:22: Mhm changed, right? 
 22:29: Mhm. 
 22:30: Absolutely, it's OK, so yeah, and basically business connection details change from one, for example, it, it, I, if I talk about like how I gonna, handle the situations, I would say, as long as we don't, like. 
 22:49: put these spell in the code because instead we keep them in in the application settings we have the other function app configurations or use any environment variables because during the deployment to the Azure DevOps the associate configuration is applied for each environments so yeah. 
 23:10: OK, sure, sure, sure, sure. 
 23:16: So basically we, we store the environment specific values ID, as your service connection can you name or any other. 
 23:26: Settings in the Azure function app configuration they are inside the Azure function we read those using the.net configuration API instead of hardboarding them since Azure functions for developing the C we typically access them using the, what was the name and you know that that is the environment or that environment variable, for example, we would, give the service was connection string and queue name from the application cert at that time. 
 23:55: So this way when the solution was deployed to development queue or production, the code, remain exactly the same and only the configuration values change. 
 24:04: So yeah. 
 24:07: But how did you read it like from the environment variables. 
 24:11: How did you read the values and plug it? 
 24:13: OK, so yeah, basically, if I talk about like how can I, like read, in, in basically I don't like the like operating system environment directly in like instead of we typically use either the, environment variables available in the power platform or the, or any the secure and unsecure configuration provided during the plug-in of the registration there. 
 24:40: OK, so you published the went to as a service first. 
 24:45: Is it To which mechanism have you used in your circumstances? 
 24:53: OK, to publish something to, to publish something to as your circumverse, where do you publish it? 
 25:01: OK, so, basically, pointedly in our implementation, we use the Azure Service bus.net SDK from, CRA address poster plug-in to publish that message whenever the appointment status changed to confirm the plug-in created a message payload containing a details such as appointment ID, patient ID, or status tensions, and all, and using the. 
 25:24: The service bus can be plug-in authenticated using the service bus connections being created a service bus queue messages and all. 
 25:32: And yeah, basically the publication, means we here we're sending a message from dynamics this is there to service bus queue and also in our case the message was published from an Ayport operation plug in using the Mervice bus.net as as I mentioned. 
 25:49: How did you get the data from a surface? 
 25:53: How did I get the data from? 
 25:55: Service first, OK, OK, so particularly if I talk about like how can I read the data from the, service first, basically here we, if, if, if it will be using an as your function as I say like there within a, within like the service bus figure where the function was configured to listen to a specific, service bus queue whenever a new message was published by dynamics and as where we are automatically triggered the function. 
 26:29: OK, now you said that the portal from portal or someone confirms the apartment, right. 
 26:37: So how did you, how, how does the end user, the new contact come from from the portal? 
 26:44: How, how was, how do you achieve this? 
 26:46: Sure, sure, sure. 
 26:47: So for achieving the portal implementation like in power to this like the the end user who first logs into the portal using the configure identity there. 
 26:57: So like the. 
 26:58: Like the IO ID because you or any external authentication. 
 27:01: So after logging the user is actually like mapped to contact recording data and based on their webro and table permissions, they can see only their own appointment records. 
 27:15: because on the portal, we had an appointment details page or Any, appointment list where the, like where the user could see the upcoming appointments, like whenever the user click the confirm appointment, the portal, submit the update back to database and technically that button or form update the appointment report status from something like pending to confirm, so yeah. 
 27:45: In the first time it is a referral, the portal user will not be a contact. 
 27:51: So he will not be, he will not be able to log into it, yeah, like so. 
 28:00: So Yeah. 
 28:04: OK. 
 28:06: So. 
 28:07: OK, so basically your, your point is totally valid. 
 28:11: What I'm trying to say is like, initially the portal user may not have a contact record. 
 28:17: The first time a user registers or signs in power pages, the ISD provider such as Azure and all, and during the registration or any successful against power pages, each the contact record automatically. 
 28:30: The database or links the user to an existing contacted one already exist. 
 28:34: After that, every subscription login is associated with the same contact record. 
 28:39: And initially the user is like not a, like a not not a contacting database. 
 28:46: The order does not happen through the contact report. 
 28:48: It basically, I shared earlier, like it happens to the identity provider such as the Azure A B2C Aroid ID A or another configure, configure provider. 
 28:58: So yeah. 
 29:02: OK, I worked on, like the sales, worked on the, like, migrating side as well as the functional side as well, and, we are, we have mostly for centers around the customer like the customer service where we manage the patient referrals. 
 29:21: Service request and all and I also work on the as I say, a sales model in previous projects where I customize the entities like the lead account quantity of as well and additionally I have like have some more exposure to customize journeys as well yeah. 
 29:43: OK. 
 29:45: In the customer service now you have to work on. 
 29:49: A contact center or just the support just the cases and queues. 
 29:54: OK, yeah like I have, like have, worked on like worked on the customer service cap such as the cases as well as, case routing as well, not like not also extensively like what I said on the, the case management side we are customizing the case entity and all, so yeah. 
 30:14: OK, what about marketing? 
 30:17: What did you work on marketing? 
 30:19: OK, for baseball, particularly, I think like I like work with marketing motivate although my experience is like more on the technical side rather than designing marketing templates, but in one of my previous projects where I have worked with the, teacher marketing, where now known as the customer insights, journeys where my responsibility is including the, like, I would say what I say like customizing the marketing related entities, integrating the customer data with dianalysis 65, automating the, customer journeys using the power automate and also supporting some of the email communications and camp process and also yeah. 
 31:03: OK, coming to, marketing, whenever you send, enough. 
 31:10: Whenever you're, I'm sending out emails and if they're constantly going to spam. 
 31:17: So I avoid that. 
 31:19: OK, OK, OK, OK. 
 31:22: So avoiding these, I, I, I, I think like that's a very common challenges. 
 31:28: than the email marketing because simplify sending the emails from dynamic marketing doesn't guarantee like, how they will catch, they will really, reach the inbox. 
 31:39: To, to avoid emails going to spam, we need to, follow both, I would say technical and email best practices. 
 31:46: So first, make sure the, like sending, sending domain is properly. 
 31:53: authenticated using the, keyboard IC the SPFDKM reports because this helps email providers verify that the emails are coming from a trusted source. 
 32:04: And second, we use, definitely use a verified custom domain instead of any generic email address and maintain a good tender reputation. 
 32:14: And from a content perspective, we avoid the, like what I say, the, this time triggering words, or any excessive images or any too many links and, and misstating subject lines or, so here we also monitor the delivery rates, bounce rates, and also, yeah, that's our idea. 
 32:41: Let me give you one my final scenario before we wrap up the call. 
 32:45: So we are working on a sales implementation, OK, and the and the requirement is to, there are 2 users. 
 32:55: One admin user. 
 32:56: The second user is agent. 
 32:59: Agent should see a list of records, list of lead records. 
 33:05: OK, the list should be, the list should be coming from a predefined criteria. 
 33:12: Defined by that. 
 33:15: So, things can or pandemic seems to play. 
 33:19: Like they want to define the criteria saying areas which are qualified in criteria which are disqualified in the last 3 months. 
 33:29: That's their 1st 2 criteria iss which are. 
 33:34: But it's included in the last 1 week. 
 33:38: That's the 2nd criteria. 
 33:40: 3rd criteria is Leeds, whose region is East Coast. 
 33:44: That's the 3rd grater, and this. 
 33:47: 123 are the priorities, and these priorities will keep on changing. 
 33:53: The priorities filters will keep on changing. 
 33:55: It's not constant for 1 week or for a certain period of time. 
 33:59: They will be keeping it constant, and it will keep on updating. 
 34:04: If they don't update it frequently, more frequently as they can. 
 34:07: So that they can focus on certain aspects of needs. 
 34:13: So the two complex implementations here are one, defining the criteria for the elements. 
 34:21: The second thing is to show that list of leads for the revenue for the agents. 
 34:28: Thank So, who are you? 
 34:32: OK. 
 34:35: OK, OK. 
 34:37: So let me see a bit of think about the same, you have given me some of the scenarios, so I have to think based on the criteria. 
 34:47: OK, so like, like I think. 
 34:51: For particular scenario, I think I would, like I would like to implement this as well I think, what I see, hmm, I think I would like implement this as a configuration driven lead priorization solution, not. 
 35:06: As any, any hardcoded view or any, or any hard hardcoded plug-ins because the admin needs to change the criteria and priority frequently. 
 35:17: So here I would create a custom configuration entity, something like the, like the lead privatization rule. 
 35:25: And then that entity, the admin can define the ruling, priority orders or any date range, something something at all. 
 35:35: For example, rule one can be disqualifying leads in last few months or like the rule two can be leads to closing in next 1 week. 
 35:45: So yeah, the important point is that the rules are. 
 35:49: Like stored as data configuration so the admin can like update from update them from the moral-driven app without requiring the code changes or deployment and particularly for showing the leads to agents, I would not create the three separate static views because the criteria and priority keep changing. 
 36:11: So instead I would create either a custom agent lead both book table or, or any calculated prioritization process. 
 36:19: So you, I think like like, like, like a schedule background process such as power automate schedule flow or any anything plugin or or like or or, or like what for for large volume use the as your function can. 
 36:37: Evaluate the active rules finding the matching leads and all and like if the lead volume is small to medium I would use the I I would definitely use the I want to make or any plugin for the evaluation but if the volume is large and rules are much more complex does create the rules. 
 37:05: Basically I'm Edwin, I'm admin I create, I open this data and roll it. 
 37:12: How do I define the criteria? 
 37:14: OK, so basically, as we know, for this, we can go to the center where the admin can vertically, add the, rules, rules, for the initial that that that we are to travel. 
 37:29: How do I do that? 
 37:31: How do, how you have given me the solution. 
 37:33: You have some out and given me the solution and the admit. 
 37:37: I open the prioritization door. 
 37:38: I click on new prioritization door, then what I will say. 
 37:41: OK, so here, how, how can we admin, give the, like, what, what, like, sorry, pardon, like, getting confused in the last point, like what do you think? 
 37:54: So you gave me the solution. 
 37:57: You gave me the solution, and that. 
 37:59: I want to define a. 
 38:01: I want to define a para should do. 
 38:03: So I keep on the you, you have papers. 
 38:07: I go to that meeting. 
 38:08: FIFA new. 
 38:10: I see the form. 
 38:13: But I should have plan to movement. 
 38:15: I should have plan to. 
 38:18: Number 1234. 
 38:20: Then how do I define the criteria here? 
 38:23: OK, for defining the quantity of defining the criteria based on the, solution like, really here the I defines the criteria using simple contribution field on the prioritization rule format, not by writing the code, for example, on the lead prioritization rule form, I would, give fields like the lead status or on a status reason or any data field or any active like so the admin can create rules like this. 
 38:49: Rule one, like will be the priority level one. 
 38:53: Or lead status, I mean be disqualified or data field may be modified on or or like operator would be like the any, any last month duration 3 months or for or for particular for the rule to for example the priority number. 
 39:10: to be 2 or date 3 to be the estimated closure and on and also for rule 3 the number so is this out of the room. 
 39:19: So whatever, say for example, to start with one word which says status goes to disqualify. 
 39:26: So I want to defend that. 
 39:30: So you're gonna be typing that saying that of the status because disqualified or? 
 39:35: Is there anything which I want to select here? 
 39:38: OK, so, OK, OK, got it. 
 39:40: So for this criteria, yes, it's like definitely, this like I would not ask the admin to type, typically conditions like the, like the status it was disqualified, that would be risky and not people that's user friendly. 
 39:55: So I would give them a dropdown the speeds on the priization rule form, so the admin experience would be like this they open the transaction. 
 40:08: OK, have you worked on? 
 40:11: Yes, I worked with Paris. 
 40:14: But I'm, I'm done with that. 
 40:17: Do you have any questions for me? 
 40:18: Yes, my, I have one major question like what would be like the majors and responsibilities for me, for this particular position. 
 40:29: So, before I answer that, did you read the J? 
 40:35: Yes, I have. 
 40:37: OK, so this is small screen to. 
 40:41: solution architectural, so where we will be working for 70% as developer and 30% as architect. 
 40:50: And responsibility would be we would be interacting with the client directly to get the requirements with the help of a BA and give them the best optimal solutions at that time. 
 41:08: And also coming to you. 
 41:12: And then transform it into user stories, tasks. 
 41:17: To keep with implementation details so that the developer can work on it. 
 41:23: And then you will, if whenever you find time apart from the architectural activities, you have to work on this, work on the items as well. 
 41:32: OK, got it, got it, yeah, that clarifies my question, and I have one more question like what will be the next step from here. 
 41:42: I think so. 
 41:43: This is your 1st round, right? 
 41:44: No, it's my 3rd round. 
 41:48: Oh yeah, that, with the Avimanu, I think, the name, I think, yeah, but for the second round I have with Avi, and, for the first round I, I like, I, I don't remember the name of the, the. 
 42:10: well, that I'm not sure if you is the right point, but there will be one more row. 
 42:15: if this is, this is successful, then there will be one more wrong. 
 42:18: OK, sure, sure, is it on. 
 42:21: And that's not a technical role. 
 42:23: It's just a manager role explaining everything. 
 42:27: OK, got it, got it. 
 42:28: Sure, sure, thank you so much. 
 42:31: Thank you so much. 
 42:32: Bye-bye. 
 42:33: Yeah, you too. 
 42:33: Bye-bye. 
 42:43: Oh yes. 
 42:45: Right 
