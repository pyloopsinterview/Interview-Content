0:00: Good good afternoon. 
 0:03: Susan. 
 0:03: How are you? 
 0:04: I'm in a meeting, OK, OK, and, Suheil is gonna conduct the interview. 
 0:10: Susheel, are you there? 
 0:15: This you. 
 0:18: That It you. 
 0:24: But Is she in? 
 0:30: I've been. 
 0:34: yes, sir. 
 0:36: I, especially, that's, I think it's, he has a bad connection. 
 0:42: connecting OK. 
 0:45: OK. 
 0:48: Hosanna, how's everything, man? 
 0:50: You're going back and forth. 
 0:53: All right, I've seen your resume. 
 0:55: Your resume looks really good. 
 0:57: Thank you. 
 0:57: So, there is this thing, where, you've been, back and forth between C Power Platform and SNO. 
 1:07: So like. 
 1:10: OK. 
 1:13: So what's, what, what is your main thing? 
 1:16: Is it, FNO or is it C? 
 1:19: So I would say like FNO is the main thing. 
 1:24: OK, that's good. 
 1:25: That's what we want, right? 
 1:27: OK, but do you, have you ever worked in, because you've worked in both the pieces, have you worked in, the one, right? 
 1:35: yes, I have worked, with SCE as well. 
 1:40: Oh dual right, yeah, you understand what dual right is dual right. 
 1:44: OK, yes, absolutely. 
 1:46: Like, in, in dynamics 365, like dual right is the capability like that keeps data synchronized, in near real time between 65 FNO and data. 
 1:58: So both applications can work with the same business data. 
 2:01: So yeah, I would say yeah. 
 2:06: Mhm Yeah OK. 
 2:18: You is to see bad days. 
 2:27: Yes, is here. 
 2:28: So, can you take the interview, Yeah, I think I was gonna ask the first question to you then, how do you, design, like, function test cases for, FNM module, FNO modules. 
 2:44: So like for designing test pieces like FNA module, like I would start by understanding the business process and like requirements for the specific FNO module and then I identify the major workflows and positive and negative scenarios, integrations, validations and business rules, of course, and like, for example, like, for sorry to cut off your how you set up that thing. 
 3:11: How, how would I set up that? 
 3:12: OK, so like for setting up that I would say, it, it will be, set up in a structured way. 
 3:20: Like first I would, identify the, give me an example based on your experience what we have done in the revision project. 
 3:29: OK, like, for, for example, like I would say, for an accounts payable process, like I would create the required master data such as, vendor, procurement category, and item, and like, and then make sure the appropriate, financial dimensions and posting profiles like are configured or not. 
 3:49: And then, then I would define the preconditions and test data like, like, for example, Like I would use a specific vendor purchase order amount item tax code, and financial dimensions and like after that, I can you, can you explain me about the current you sure, sure, like, I would say, in like my current engagement like with RWJY members I'm, I'm, I was like working on a large scale, 65 project like whereby main role is mainly focused on performance load integrations and regression testing like across the whole B365 and like it's also connected with enterprise systems and I would say like I work with the functional and development teams to understand critical business or what what in the accountable what you do like the account entity what it does. 
 4:47: So, OK, like at the account level, I'm mainly focused on understanding the business processes, validating the, critical account-related transactions, and making sure the data flows like correctly work across D 365 and the connected systems. 
 5:04: And like from the testing side, I create functional and performance scenarios around like Account creation and updates required field and business rules validations integration as well. 
 5:18: And I, I also validate the data synchronizations between D365 data APIs and downstream system. 
 5:28: So yeah, it, it will be the approach I will use. 
 5:34: OK, so let me go and the simple thing, we are simply using the client-side scripting as a yes. 
 5:40: OK. 
 5:41: Are you aware of that part of the client side scripting? 
 5:44: Yes, OK. 
 5:46: So supposing the account, the phone phone number we have the out of the box. 
 5:53: Yes, OK, I have this scripting, to maintain certain business rules. 
 6:00: Now define me how you'll validate those things, what that means, and how you will plan, how to write your test cases, or how you'll do it so that it will be a quality deliver how you'll do that. 
 6:14: OK. 
 6:15: So, yeah, definitely for this kind of scenario, like, first, I would understand the business rule and we define the expected behavior. 
 6:23: Like, if I talk about example, like suppose, we have a business rule that the account phone number is mandatory, when the account is marked as an active customer, and like I would create test scenarios for like both the positive and negative cases. 
 6:38: And after that, like I would, open an account and, keep the phone number blank and set the required conditions and then like verify that the appropriate validation message appears and that the record cannot be saved if the like who actually requires it or not. 
 6:57: So, after that, like, I would then enter a valid phone number and verify that the validation is removed and the like record saved successfully. 
 7:06: And I would also like to test different formats such as, as I have mentioned, valid and valid, phone numbers, boundary conditions, blank values, and, existing records. 
 7:17: And after that, finally, I would test different types of, user roles and browsers if like actually applicable, and then check the browser console for like, you know, JavaScript errors and perform regression testing. 
 7:32: So it will be the approach. 
 7:36: Now, coming to the functional part, you have worked on the sales module. 
 7:44: Yes, yes, I have worked with the sales model. 
 7:48: So tell me about the only the features and the functionalities about the opportunity entity. 
 7:54: OK, so I would pick up only functions and like yes, like I have would say. 
 8:04: Like it, it will be the main functionality and will be like in the sales module like the opportunity entity like represents a qualified like potential sale like once, once a lead is qualified, like it can be converted into a, into an opportunity like where we actually manage. 
 8:25: The sales process from qualification through closer so I would say like from a functional perspective the key features I, I have worked with like opportunity creation and qualifications, customer stakeholder management products and pricing, sale processes and stages product, sorry. 
 8:47: Tell me about the product. 
 8:49: OK, so, product is actually like, in like in, in an opportunity the product like, is used to define like for the potentially pur purchasing like, I would say I have worked with the adding products to an opportunity, selecting the are you like this product. 
 9:08: I'm sorry. 
 9:10: How you add the product. 
 9:11: So, I would say like for adding the product, like I first open the opportunity and go the, go to the product section, then I select the add product to the appropriate like. 
 9:24: Sorry to cutrupt you, but what about the business organization level? 
 9:27: How you'll add the product? 
 9:29: OK, so in the opportunity, OK, at the like a business organization level, I will post, like make sure that the product is properly configured in the product catalog, and assigned to the correct price list, unit group, business, business unit, and yeah, the organization level security. 
 9:46: As well, and after that, like when I add the product to an opportunity, I like select the appropriate price list, choose the product from the available catalog and like specify the unit and quantity and, verify that the correct organizational pricing and so. 
 10:07: Yeah, in a, in an organization you have a different department or the different regions, OK, and for the different regions you have, different types of products. 
 10:17: Now you tell me how you differentiate the reason A should have a specific product and the reason we have a specific product. 
 10:25: The Reason A should not be seen that, product A from the reason B. 
 10:29: It should be a suppression. 
 10:30: How you'll do that, OK, like, Suppose region A can sell products A and B, while like Reg B can sell products C and D. 
 10:40: So, like, 1st, 1st I would understand like whether the restriction is based on a business unit, region, or sales organizations and like I would say like at the functional level, I would first define the product catalog and a price list accordingly and then, then I would configure the appropriate business, business units, teams, security rules, and, access. 
 11:05: So like users from region A only have access to the products applicable to the region and like, if, if the requirement is like more in more dynamic way, like for example, the same user can, Work with multiple regions, I would use a business rule or custom validation to determine whether the selected product is like. 
 11:27: Valid for the opportunities region or not and after that like during testing, I would verify like scenarios such as region A selecting region A product or not. 
 11:37: So yeah. 
 11:40: Coming to the point of the plug-in side, are you already yes, there will be a plug-in as you. 
 11:46: So for the plug-in, how are you do these things. 
 11:49: OK. 
 11:49: So if I talk about like for the plug-in side, like, yeah, absolutely, I would first understand the plug-in registration details such as the messages, entity, state, execution mode, and after that, then I would create test scenarios like based on the appropriate business logic. 
 12:09: Like, for example, if the plug-in runs when an opportunity is created. 
 12:14: or updated, so I would test like valid and invalid data, different field combinations and user roles, and like I would also cover both the positive and negative scenarios including exceptional handling and cases like where the plug-in should actually not execute and yeah, after taking the plug-in, I would verify the expected changes in the file. 
 12:41: So suppose consider the plug-in is getting fed. 
 12:44: What will be your steps to take care, what you do? 
 12:48: So I would say like if a plug-in actually fails, so like my first step is to reproduce the issue consistently and capture the exact error message, timestamp, record, and transaction details, and then, then I would check the plug-in trace log and review the plugin execution details, including everything, the messages, stage, execution mode. 
 13:10: And I would provide the like developer with the complete reproduction step like test data, error details, and place information. 
 13:19: So I would say like, yeah, once the developer fixed the issue, I would retest the same scenario then I got it. 
 13:27: That's it, coming to the point of same scenario, but you have we have implemented the power of the flow as well, yes. 
 13:34: We do have it. 
 13:35: So for that one, how you'll do the testing same. 
 13:39: So, if the same business like, scenario is implemented using powers in, automate flow, like I would test it end to end. 
 13:48: Firstly, like, I would say that I identify the trigger condition and the expected business outcome. 
 13:54: Like, for example, suppose an opportunity is created like for a region A. 
 13:59: So, like a power automate flow is used to like send an approval request to the appropriate, regional manager. 
 14:07: So I I would create that opportunity with the required data and like then verify the flow is triggered or not. 
 14:13: So then I will validate each, each, every each and important step whether the correct manager is identified, the approval request, OK, got it, got it. 
 14:23: But what happens like when the plugins, you'll get the message, but when, when your automated flow sales, how, how you'll track it down, there is no any pop of what you'll do. 
 14:36: so in that case, like, if a plugin fails, especially a synchronous plug-in, the, that the user can receive an error message, I would like first open the flow and check the failed rank to identify like which step failed, the error message inputs and outputs, and like I would say like from a functional perspective. 
 14:55: I would also validate whether the expected business outcome occurs or not. 
 15:00: And like, if, if I didn't, I would capture the event details and raise a defect and like for production. 
 15:08: I would also recommend an error handling mechanism such as, a failure notification or a logging mechanism. 
 15:15: So like the support team is coming to the point of dashboard and the views. 
 15:20: What is the difference between it? 
 15:22: So dashboard is actually, I would say, the main difference like a view firstly used to display and work with a specific set of records by. 
 15:32: Like a dashboard gives you a broader visual summary of the detail. 
 15:36: So like a dashboard combines information from multiple views and represented visually using charts, graphs, lists, and KPIs. 
 15:47: So it, it means contains the major difference. 
 15:53: Whatever the related with that entity is, suppose you are having a dashboard of the account entity, and along with that related entities like contact, we already had a relationship with the account and we contact the entity. 
 16:06: So what happens if I want to see if they sold both of the record information on the dashboard. 
 16:12: So, yes, exactly, like accounting contact, have, like, for the, I would say, have a relationship, typically, 11 account can have multiple contacts. 
 16:25: So like, if I'm building an account-focused dashboard, so I can use components based on the account data as well as related, contact information depending on the reporting requirement. 
 16:38: And if the requirement is to show detailed related contacts for a particular account, I would use, account forms related contacts, subgrade like, if the requirement is an overall management dashboard, I would create appropriate, views and charts, and charts, based on the related data. 
 16:56: So, yeah. 
 16:59: And, what about the FLSA you are aware about this one, yes, yes, yes. 
 17:11: So what, what it does. 
 17:13: So,, firstly, yes, I am familiar with that. 
 17:16: So FLS is used, then we need to actually control access to a specific field just rather than giving or removing access to the entire recorder entity. 
 17:28: It was considered a user new user has been like onboarded usually on the involvement of the organizer. 
 17:36: Now how you'll add that, your new user onto that, SMS? 
 17:41: How you'll do it. 
 17:43: OK, so firstly, like I would make sure that the user exists in the organization identity system or not, like, and then the user is available in if available in the business environment. 
 17:56: I would go, I would go to the user, select the, a new user, and assign the appropriate security roles based on their, job and responsibilities. 
 18:05: And then I would make sure the user is like assigned to correct business unit team and security profiles like depending on how the organization has designed its security model and like if the organization uses field level security, I would also add the user to the appropriate field security profile like if they need access to secured fields or yeah. 
 18:28: So tell me about the access thing. 
 18:31: Are you aware of on that one? 
 18:32: Yes, So why, why we are using, why, when you'll be using this access thing? 
 18:40: What? 
 18:41: So like I would say like an access team is like for example, suppose we have an opportunity owned by a salesperson, but a sales manager or solution architect or also need to work on that particular opportunity. 
 18:56: So instead of changing ownership or giving them broader security privileges, like you can use an access team and provide. 
 19:04: The required access to that specific record and then then the access can be based on privileges such as read, write, append or append to. 
 19:13: So, so I would say like there, there are generally two approaches like owner teams where the team can have their own records and accessing that which are like primarily used to grant user access to specific records. 
 19:37: So, have you worked on the part of the Fend side also, or my core. 
 19:46: OK, that is your fault. 
 19:52: How you'll maintain the module of. 
 19:55: Any new, organization come up how you set up. 
 19:59: OK. 
 19:59: So like, I would say for like setting up that, if like new organizations or legal entity, is there, so firstly, I will like understand the legal entities and operating units, countries, currencies, and everything, and then I would set up the legal entity or company and then define the required organizational hierarchy. 
 20:21: So next will be like, I would configure the chart of accounts and then. 
 20:25: Accounts like financial dimensions, account structures, and, a fiscal calendar. 
 20:31: After that, I would configure the required modules like for, for finance, I will configure things like ledger, currencies, tax, posting profiles, payment methods, and then I would work on security, defining the appropriate roles, duties, privileges, everything. 
 20:50: OK, in the dynamic side, what are the basic, rules we should first. 
 21:02: We should provide to the end user so that they can access the application or you can see the. 
 21:08: Modal driven apps, whatever you are we're working on it either it's a canvas app or the mobile driven apps. 
 21:14: So like for an end user, I would first make sure the user has the required DC 65 license and environment access, and then I would assign the appropriate, security role based on what the user needs to do. 
 21:29: And after that I would also make sure that the user is in the correct business unit or team or. 
 21:35: What will be the basic role we will assign to the users? 
 21:42: Out of the box will be there, yes. 
 21:44: OK, so in that case, like it, would be typically be a customer and user security zone or a customized like, for example, for a sales user, I would, provide access to the required table set. 
 21:59: As account contact lead and opportunity with like privileges like recreate right append and append to based on there so I would also make sure that they have the required model driven app access and appropriate business unit or team level access. 
 22:17: Mr., if you, if I can ask, one couple of questions, OK, yeah, I, I asked you about, Hosan, about dual right. 
 22:29: So how do you validate, like, FNO bad jobs, data entities, and, dual right mapping. 
 22:37: OK. 
 22:38: So for dual right validation, like I would, validate it end to end between FNO and dataverse. 
 22:45: Like, first, I would verify the dual right link and mapping configurations, like including the data entity, map fields, filters, and transformation rules, and then, then I would create or update the recording. 
 22:59: FNO and verify that the corresponding, record is created or updated correctly in database or not. 
 23:06: And yeah, I would also like to test the reverse direction where the map mapping actually supports it or not. 
 23:12: And like for batch jobs I would verify that the required, jobs are running successfully and, check the execution history for. 
 23:21: Failures or retries or any, any type of performance issues and for do well writing mappings, I would specifically test field to field mapping business rule lookups, reference data and error handling, yeah. 
 23:38: Hm OK. 
 23:42: All right, thank you very much, Joan. 
 23:46: I think, I'll just get the feedback of Sushi, and obviously I, you've answered my questions. 
 23:55: So yeah, and Ibrahim will be in touch with you. 
 23:58: OK, thank you very much. 
 23:59: Thank you, but like I have some kind of, questions. 
 24:03: May I ask? 
 24:05: Yeah, yeah, yeah, go ahead, please. 
 24:06: So like I want to just ask firstly, what will be the next, process, after this? 
 24:15: Hi Hussein, I'm, so, so I have my firm and then, we work with other people as well. 
 24:24: It's a big engagement, so now we. 
 24:28: To submit you and it'll be on their side it'll be two rounds. 
 24:32: OK. 
 24:32: I think if you call by our state and you get selected over there. 
 24:37: -hum. 
 24:37: I think you should be fine. 
 24:39: OK. 
 24:40: OK. 
 24:40: But, there are a lot of, like, people applying for it. 
 24:45: OK. 
 24:46: And, hopefully we get you the interview and then you, I think you. 
 24:52: You'll get it from there, OK? 
 24:55: OK, OK, thanks. 
 24:56: All right, so I am going to pitch you, even if, if, on this one, you're a little bit late in the game, but I'm still gonna push you and then obviously it'll be easy for me to push you on both. 
 25:12: Dynamics front and FNO because they have both so they have a power power page they have dynamic sales over there they have marketing a little bit and then on the background they have the FNO, a big process of FNO as well. 
 25:31: OK. 
 25:32: Any other, any other questions? 
 25:34: No, no, you have like, given me the overview of everything. 
 25:38: Thank you. 
 25:39: OK, brother, thank you very much. 
 25:40: Thank you. 
 25:41: Thank you. 
 25:41: Bye-bye. 
 25:41: Have a good day. 
