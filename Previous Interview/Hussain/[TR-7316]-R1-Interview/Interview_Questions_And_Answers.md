0:01: Oh good. 
 0:02: So for the for the interviewer, OK, OK, let me check with them. 
 0:45: OK. 
 0:51: OK, thanks. 
 0:54: Hey how are you? 
 1:02: so, before that, can, can you please show the ID. 
 1:08: is it? 
 1:11: Yes. 
 1:27: And is it done? 
 1:30: OK, thanks. 
 1:39: Send me a that phone. 
 1:43: Yes. 
 1:45: OK. 
 1:45: So, are you recording this, sir? 
 1:56: OK, yes. 
 1:59: OK, so how are you? 
 2:03: I am fine. 
 2:04: How are you? 
 2:04: Thanks for asking. 
 2:07: Yeah, doing good. 
 2:09: OK, so can you just give me, let's walk you through the resume, walk me through your resume, and, Be some Technical background and expertise you do have. 
 2:26: OK, OK, sure, sure. 
 2:27: So yeah, like currently I'm working as a dynamics 365 and power platform engineering with RWJ B's Health, like where I'm involved in an enterprise healthcare transformation project. 
 2:40: And I have about 11 years of experience in DG 65, Power Platform, Dataverse, Azure, and enterprise integrations. 
 2:49: And in my current project, like my role is mainly focused on solution architecture, technical design, data work, security, integrations, ALM and deployment as well. 
 3:01: And like on from the database perspective, kind, I would say like, I work on data modeling tables, relationships, ownerships, and Business unit teams and security rules and like a a big part of my responsibility is like just making sure different business groups get, get the right level of access to the data like based on their business requirements without giving any unnecessary permissions and another like important area is power platform ALM and environment strategy and I would say like we maintain a separate development testing. 
 3:40: UAT and production environments and like we use solutions and control deployment process to like move move changes across environments and yeah I work with development QA and like teams to you know just to manage dependent dependencies, validate deployments and make sure changes are like promoted safely into production. 
 4:05: So yeah, it's pretty much about me what like so far. 
 4:12: Interesting. 
 4:16: So what are the modeling. 
 4:18: So I would say like in in the DC 65, like if, if I qualifying I talk about in my current health healthcare project I have like mainly work around that DC65 and power platform ecosystem like rather than just being limited to just just one out of the box module and. 
 4:41: In BC 65 I have worked like many multiple like cross modules, but like my, my strongest experience has been around customer service, sales and power platform data was layer and I would say on the on the customer side I worked with things like accounts, contacts, cases, queues, SLAs activities and security and I would say I've also experienced, have experience with the D65 sales modules like mainly, mainly around the customer life cycle including leads, opportunities, accounts, contacts activities, and sales related processes and beyond the functional yeah yeah. 
 5:26: OK, OK, I. 
 5:28: So I'll just give you one scenario, where, let's say. 
 5:32: As you mentioned, you have an exposure on the customer service, right? 
 5:36: So how, how are you managing the support tickets? 
 5:41: Let's say I'm just a. 
 5:44: There is a tag boat which is enabled in our website, right, and there are multiple customers come in and they initiate the cha so our representative. 
 5:55: I will attend to chat, right, so let's say I'm just chatting regarding the credit card issue and Sachin is there and Sachin is starting. 
 6:09: A concern about their they are just inquiry about the projects, right. 
 6:16: So how this can be managed and how this ticket can be assigned to the correct team member. 
 6:24: OK, so that's a good question. 
 6:27: Like, yeah, particularly for like this type of scenario, I would, like recommend that, I would manage it using D 365, customer service with like omni-channel capabilities, uses, and routing rules and like, agent skills or classifications, and the main idea is that, we don't want, every incoming chat to, you know, just to go into one common bucket. 
 6:53: And then have somebody manually decide who should handle it or not and like we want dynamics to understand the type of customer request and automatically route that conversation to the right queue and the right available agent. 
 7:11: So like, let's, let's take an example like if, if, suppose you are initiating a chat from the website regarding a credit card issue while such in initial. 
 7:22: It's another chat, regarding, or, sorry, regarding, product inquiry, like when, when those conversations came through the chatbot or any digital messaging channel we can, probably capture the context of the conversations such as the customer category, product priority or any issue type is there it is and like based on that information we can classify the conversation and like for example your Our conversations would be classified as credit card support while such could be classified as a product inquiry. 
 7:57: So from there I would configure like queues and routing rules, and we might have a credit card support queue containing agents who are who are actually trained to handle or any issues with card related and another product support or product inquiry. 
 8:17: OK, got it, got it. 
 8:18: Thank you. 
 8:20: there is another scenario, let's say, There is an organization who is working in 3 different locations, right. 
 8:32: And each location there is a manager and under that manager, let's say 10 members are working. 
 8:42: So from the one location, they, the sales manager can see their record and, as well as their team member report and the another. 
 8:55: But the manager can't see each other's records. 
 9:01: How you can implement it. 
 9:03: OK, so, like, particularly I would say for this type of scenario, I would like just implement this using a combination of, data host business units, owner teams or users and security roles as well, like, depending upon, depending on, how strict the data boundaries need to be. 
 9:25: And since there are 3 different locations and like each location has one manager with 1010 team members, I guess, I would first understand like whether the locations need complete data isolation or whether there are, there are some records that like need to be shared across locations and like for, for, for an example, like, let's say we have New York, New Jersey, and California, I would create separate business units for. 
 9:55: Like every each location such as New York, BU, New Jersey, BU and California, BU, then the manager and the 10 employees belonging to the New York would be associated with the New York business units and similarly for, for every other locations and then, then I would create an appropriate security rules that like provide the employees with access to their own records or any records that are owned by them. 
 10:26: So, can you go with the, can you go with the specific, like, the team, team member, what role they will have and manager what they, what role they have? 
 10:36: OK, sure. 
 10:37: So like, for, for the, like, specifically, I would, keep the security model fairly simple and use like two primary security roles. 
 10:47: Firstly, sales representative and then the sales manager. 
 10:51: And for the team members, I would create a sales representative security role and they like their access would generally be at the user level, meaning they can create, read update and like work with the sales reports that they own and for the manager, I would create. 
 11:08: So like sales manager security role, the manager needs, broader access than the team member. 
 11:15: So like I would give the manager business unit, level or any higher, higher rates. 
 11:22: It's just depending on the exact requirement. 
 11:28: What is hierarchy-based access? 
 11:30: So, actually hierarchy-based access, I mean, it's, like, it's in a dataverse means like access is granted like based on the manager to employ reporting structure. 
 11:42: So like instead of just manually sharing every report with the manager, data was can like automatically determine access based on like the reports. 
 11:54: Yeah How many types of relationship. 
 12:00: So, relationship behavior like consists of, talk about, especially like for one to many or many to one relationships, there are like several standard behaviors, we can configure like the main ones I usually consider are, referential, parental, cascading and no cascade. 
 12:22: So yeah. 
 12:25: OK. 
 12:29: And OK, did you get a chance to work on the plug-in telephone? 
 12:34: Yes, I, I do. 
 12:37: OK. 
 12:39: So, Let's say. 
 12:45: What is the, what is the pre-image and post image? 
 12:49: OK. 
 12:50: So, I would say like 3 image. 
 12:55: It's actually the snapshots, they are the, they are the snapshots of our database record that we can make available to a plug-in during execu during any execution and like they are mainly useful when we need to compare the record values before and after an operation like without. 
 13:15: Without making any additional retry calls through data work and like pre pre-image actually represents the record before the operations happens and whereas post image like represents the record that are actually after the operation has been completed so these are the main terms. 
 13:37: And let's say there is in the plugging you are calling an external API and that API having the. 
 13:48: Security key or API key. 
 13:51: So what, what approach you will do to keep the, keep the API safe. 
 14:00: OK, so, yes, in that situation, I would like, firstly never hard put the API key or, secret key directly inside the plug-in port and like, from a security and maintainability perspective, I would keep that, secret outside data was cod and, retrieve it, securely at runtime and like my, my preferred approach would be to use as your keyword and I would, store the API or like client secreting keyboard and then allow the integration component to just access it using a secure identity, ideally like manage identity or Microsoft ID based authentications it's depending on the architecture. 
 14:42: So I'm just asking you about plugin. 
 14:45: So you have just written a plug-in where you are calling the external API. 
 14:50: This is not a part of services. 
 14:53: And you are not going to use the injured services, right? 
 14:57: So how you will keep those API and maybe you are just there are three different APIs. 
 15:04: One is for, Team involvement and then maybe UAT involvement they have the different API and also there are different DPIT and the products and they have different API and FBIT also. 
 15:20: So how would you manage those? 
 15:24: In case of clogging. 
 15:26: OK, so, like, yes, if like, as your services are like completely out of scope and I have to call the external API like directly from the plugin, then I would manage the API endpoint and, API key as an environment specific configuration like rather than just hard coding in them in the plugin and like where you manage I just wanted to know. 
 15:53: yeah, like, where would I manage for that? 
 15:57: Where would I manage for that, right? 
 16:00: Yes, OK. 
 16:01: So, OK, let me tell you, like, I would manage it in first, two places inside the power platform, database setup and like for the API URL or endpoint, I would, manage that through a database environment variable inside the solution. 
 16:18: So like in, so in depth. 
 16:20: The environment variable like current value points to the dev API URL or in a UAT it points to the UAT API URL and like in production it points to the can you, can you, can you just give me the syntax how you will get the environment variable from plug-in so I would recommend like yes, for from a plugin I like. 
 16:48: Normally retrieve an environment variable by like like for example if my environment variable schema name is new_external API URL I can write it like this, it's like, yeah. 
 17:04: OK. 
 17:08: OK, I'll just give you one scenario. 
 17:10: So let's say there is a limit approval process, right? 
 17:14: So whenever I just, raise a Leap, so it will go to the 3 level of approval process, right? 
 17:24: So it will go to the reporting manager and then the above one and then above one how you will do that. 
 17:31: OK. 
 17:34: So I would say, yeah, yeah, like for like particularly, I would implement this using power automate the database because like this is a business process, approval scenario and like we want the approval chain to be configurable rather than just hardported and when an employee like submits a lead request I would first create a lead request record in the database with information such as employee lead type start date. 
 18:03: entered, etc. 
 18:04: and the employee's reporting manager as well and like for for the first level, the flow identifies the employee's charity reporting manager and then sends an approval request to that manager. 
 18:18: I would like normally get the manager from the. 
 18:20: Employees user information or from a config organizational hierarchy rather than hard coding a person's names and if if the manager approves I update the lead request status or approval level and then identify the like managers. 
 18:39: Yeah, what action will be used in a power automate to send the notification? 
 18:47: so it would be like for the actual approval process, I would use the approval action like start and wait for an approval in power automate and. 
 18:59: I would dynamically, populate the assigned to like field with the email or, user identifier of the, current approval such as, employees reporting manager and like if I only need to send an informational notification and I don't need like the person to approve or reject, then in that case, I would use an action such as send an email or we do through like Outlook or or or just post a message in chat or channel through Microsoft Teams. 
 19:29: OK. 
 19:34: OK, and, I can. 
 19:39: Hi, thanks, Dave. 
 19:42: Hi. 
 19:42: Hi, hi, I have few questions related to power and health applications. 
 19:48: I hope you have already done some work, yeah, yeah, I have, I have been, I'm familiar with that. 
 19:55: So, do you know what is the difference between Canvas application and model-driven applications? 
 20:01: So yeah, the major difference is that, like for, for Canvas app, like, are more UI driven and model-driven apps are more data and process-driven. 
 20:12: Like, with, with the Canvas app, I have more control over the, user interface. 
 20:17: I can design the screens almost like a custom application design that, web controls, but, forms, galleries, and Other components appear and connect that app to database or any other data sources and for model driven API like it is primarily built primarily around the dataverse model like we define table columns, relationship forms views. 
 20:43: So yeah, basically like a canvas app is used from buildings from scratch to end and while model driven is just for for like backend type, yeah. 
 20:57: So in the model driven, can we customize the screens or not? 
 21:01: So, in model driven, I would say like, yeah, it's we can definitely customize the screen in model-driven app like, but the level of customization is different, totally different from a canvas app. 
 21:13: Like I would say, in, in a model-driven app we primarily customize the experience to like the forms, views, dashboards, business process, command bars, etc. 
 21:25: so. 
 21:26: I would say like, yeah, we can definitely customize the skills. 
 21:31: In in this case we have to choose the canvas. 
 21:35: What is the particular use cases where we should go with the moderable one and other case we should go for the campus, OK. 
 21:46: like, I would like decide if. 
 21:49: I would decide it based on the business requirement and the level of UI flexibility we actually need and like if the application is primarily data-driven and process-driven, especially when the data is already in database, I would recommend the, with the model driven app and like, I, I would choose a Canvas app then the primary requirement is, highly customized user experience. 
 22:15: So yeah, there are. 
 22:17: there are also some cases like where I would also use both together. 
 22:23: OK, yeah. 
 22:24: And the Gilma's application, have you experienced the validation? 
 22:31: What is delegation and how we can minimize it? 
 22:34: So yes, I have worked with navigations in Canvas like delegation. 
 22:39: Oh, so sorry, so sorry, so sorry. 
 22:41: I'm so sorry for this in my bad. 
 22:43: Yes, I have worked with delegation in Canvas app. 
 22:46: actually delegation basically means that instead of power apps bringing all the records from the data source into the application and then, processing them, locally, Power apps like sends the query to the data source and, I would say let, let the data source perform the filtering, sorting, or searching and like if, if the, if that operation is supported for that particular data source and column, column type, Power app sends the filtering request to dataverse and dataverse returns the matching records. 
 23:20: So yeah, it's, it's the. 
 23:25: OK and what is the limitation of delegation into power apps? 
 23:28: So, the limitation is like, firstly, it depends, but I would say the main limitation of delegation power apps is like canvass, canvas apps is like is that not every power. 
 23:41: , FX functions, operator, connector or column type supports delegations and like when an expiration is non-delegable power apps like cannot send the complete query to the server so like it retrieves a limited number of records and processes them locally. 
 23:59: Yeah. 
 24:00: And what is the maximum number of records we can pull? 
 24:03: I guess it's like, 2000 records. 
 24:08: And if I have more than 2000, maybe 10,000 reports, so now I can get the data on our end. 
 24:16: OK, so in that case, like, I, I think I am using non, believable like, yes, if, if, if I need to work with more than 2000 records, like for example, as you have given like 10,000 or even, more than 100,000 records, like I would not try to, load all of this, all of those. 
 24:37: Records locally into the canvas, the better approach will be like to make sure the query is deleable. 
 24:44: So like power apps or send the filtering and sorting to the data source like data or SQL and like only it drives the records that are actually needed. 
 24:55: So yeah. 
 24:57: OK, and in the canvas and application and the data source, can I use database or SharePoint list. 
 25:07: it's like, yes, I, both database and SharePoint list can be used as a data processing Canvas app. 
 25:16: And same if I go with the model driven, can I use on the model. 
 25:22: So in model driven like if I talk about, the primary data source will be like has to be database and, so like I would not create SharePoint list the same way as I would in the Canvas app. 
 25:36: So yeah, basically, in formo drive even the data was, plays a, a bigger role in the picture. 
 25:45: OK, but in case if I wanted to use SharePoint list, can I do as a data source in the model, like, yeah, I can say I can still integrate like, if, if we specifically, like, can use a SharePoint list directly as a table or data source inside a mode, then like, I think no, not in the same directory as database. 
 26:07: But like a model driven app is built on database table so like the tables shown in the app need to be database based. 
 26:15: Like if, if I have existing SharePoint list data I would handle it through an integration or synchronization approach. 
 26:23: Yeah And how would you design an ALM into power that application? 
 26:31: What, what strategy you follow? 
 26:34: For designing the application. 
 26:36: OK. 
 26:37: So, like, ELM, like in PowerA application, I would design it around separate environments, solutions, source control, automated deployment, pipelines, etc. 
 26:49: I, I would say like in my current project, I would, typically have development, UAT and, production environments where developers build and testing development. 
 27:00: the solution is validated in UAT and only approved changes are like promoted to productions, like I would, I would avoid making direct changes in production because that makes the solution difficult to, control and troubleshoot and like for packaging I would use, power platform solutions and like during development I would work with them unmanaged solutions where like we can make changes and for UTM production. 
 27:27: I would deploy the solution as manage solution so that the particular, particularly the target environments are like controlled and the components can be managed through the release process and I would, I would also like separate environment specific configuration from the like actual application logic like for example if the UAT and production are different APIULs I would use environment variables, yeah. 
 27:55: OK. 
 27:56: You, you share about the, solution. 
 27:59: So what is manage solution and then manage solution and when we should use it? 
 28:03: So, I would say like for manage solution and so manage solution, it's like a different ways of packaging and deploying for platform components. 
 28:12: basically I would say like in. 
 28:14: The the key difference is whether the like whether and manage solution is typically like what I use in the development environment developers can add components, modify. 
 28:27: Everything and in manage solution what I would like normally use when moving the solution into a UIT or production like it's basically a package version of solution where the like developers cannot modify or make the changes on its own and in and like yeah this will be the most major major. 
 28:51: So in a manage solution, can developer change anything in managed solution like developers cannot change or cannot modify anything. 
 29:00: They can only do it in unmanaged solutions. 
 29:05: I have one question on this, So let's say we deploy a managed solution on the production, right, and, we realized that there is a one component was attached to that managed solution. 
 29:23: Now we are in the position to delete that. 
 29:27: Let's say there is a field, so we are in the position to delete that. 
 29:32: So how we can do this. 
 29:34: OK. 
 29:35: So, I would say like if, if, if a particular field is a part of manage solution and I want to remove it from production, I would like not try to directly delete the field from production. 
 29:50: the correct approach would be like to remove that component from the source solution in development and then deploy a new version through ALM like. 
 30:01: For example, let's say customer type is a custom field, included in version 1.0 of my, of my own manage solution. 
 30:09: So, in the depth, I would remove that field from the solution and make sure that there are no dependencies on it, such as form, view, business rules, and etc. 
 30:18: And then, then I would create a new version of the solution, like for example, 1.1 and then deploy that updated solution to UAT for actual testing. 
 30:29: So, once UAT is successful, I would like to import the updated managed solution into production. 
 30:35: So, yeah, that's perfect. 
 30:41: OK, yeah. 
 30:44: And a person, for example, if in the power of application I'm creating multiple multiple screens, right, but in a, in all these things I would like to utilize common sections just like a header or put up right so how I can utilize common sections for all the screen should I have to create every time. 
 31:09: this section on every screen, just copy and paste there, or is there any way we can do the comment sections and utilize everywhere. 
 31:20: OK. 
 31:21: So I would say like, yes, there, there is one, like there is a better approach. 
 31:27: Like, firstly, I would not, create the same header or footer, separately on every screen and just copy paste it like because that becomes, you know, difficult to maintain. 
 31:37: So, in a, in a canvas app, I would create reusable component for the common section. 
 31:43: Like, for example, I can create a header component that contains the company logo, Application title, user information, and navigation buttons, and then, then I can add that same component to all the screens and like if, if I need to change the logo, title or any navigation behavior, I can actually update the component once instead of just modifying every screen individually. 
 32:11: So similarly, I can like create a photo component as well and reuse it across all the screens. 
 32:17: And like I guarantee can believe the music company. 
 32:21: sorry, how about technique of how you can create reusable component. 
 32:25: OK, so, particularly for creating like this, like in Canvas app I can create a usable component from the components area. 
 32:35: Like for example, if I want a common header, I would create a new component called the header component and then add the controls like I need inside it, such as a big logo title and everything. 
 32:50: OK, yeah, and, I just wanted to relocate, my question for power of global. 
 32:59: Did you work on power of the? 
 33:00: Yeah, yeah, yeah, I have, I have done. 
 33:04: I have actually, I have many experiences with that. 
 33:07: What kind of power documents available in the power. 
 33:12: So type of file. 
 33:15: So there are several ways like I work with power to and like I generally categorize the flows like based on what triggers them and how they are used. 
 33:24: I would say the first one is automated cloud flow. 
 33:27: this is triggered automatically when an event happens, and the second would be instant cloud flow where the, flow is triggered manually by a user, and the third one is like a scheduled cloud flow. 
 33:41: Like this is a useful when I need something to happen at a, particular, particular interval, and there are also some like business process flow which are like different, different from, regular cloud flows and like. 
 33:57: For integration scenarios like, I've also worked with the flows that connect data was with the other systems using APIs or connectors. 
 34:04: So yeah, majorly 4 types are. 
 34:08: OK. 
 34:09: And did you work on the custom collector? 
 34:12: Yes, I am. 
 34:15: And have you used the HTTP action? 
 34:19: Yes, I have used. 
 34:21: So what is the difference between both and when we should use? 
 34:26: OK, so the main difference between the HTTP and the custom connector is like I would say it's reusability and like how we expose the API like with the HTTP action, I am making the API call directly inside a particular power automate flow and I would provide the endpoint like HTTP method like get or post headers authenticate. 
 34:52: and like become custom custom connector I am essentially creating a usable interface around the external API like I, I define the authentications operations parameters, requests and response definitions. 
 35:08: So yeah, this is the major difference they make. 
 35:12: OK. 
 35:13: And can I reuse the HTTP actions if I'm having multiple flows in a solution? 
 35:19: So can I utilize that, like, no, I, like, no, I, I wouldn't consider an STTP action itself, usable across multiple flows because, you know, an STTP action is like a part of the individual flow where like I configure it so. 
 35:38: Yeah, if I have different, different flows that need to call to the same API I would normally have to configure the HTTP call in each flow unless like I create a reusable traction around it. 
 35:53: OK, and, in case if you have power commit flow you wanted to do a code for the error handling, so how you can do. 
 36:04: OK. 
 36:06: So, like, I would say like for error handling in power automate like I actually normally design the flow so that the main business logic is separated from the error handling and notification logic and I commonly use scopes with configure and after to like just control what happens when action fails, time out, or escape like if I talk about example like suppose I have a flow that creates a database record. 
 36:36: and calls an external API and then updates the data was record based on the API response. 
 36:43: Like I, I would put the main action inside the dry scope, then I would create another scope for catch and like on the catch scope, I configure run after so like it actually executes when the dry scope has failed time out or has been skipped, so. 
 37:00: Inside the CT scope, like I can capture useful information such as the floral details, error message, record ID API response, Etc. 
 37:12: and like then, then I would like also create a final scope and if I need or, you know, clean up or final status updates like regardless of whether the flow succeeded or failed. 
 37:25: So yeah, the dry catch and finally it, it is the steps. 
 37:30: OK, and in the power of application, for example, I wanted to submit some data. 
 37:36: I have different types of functions. 
0:00: or edit the data. 
 0:02: yes, I know, like, I would say in Canvas Power app, like for saving or editing data, I commonly use functions such as patch or submit form and, update it, depending, it's depending on the requirement, like if I'm using an edit form. 
 0:20: So the simplest approach is submit. 
 0:22: Form, so like the form is connected to our data was stable or another data source and like power apps handles creating or or updating the record based on the form mode and like for, for more customized scenario, I would prefer patch. 
 0:37: Like with patch, I can create a record or update or specific existing, existing records and control exactly which fields I want to modify. 
 0:48: So like if I want to say like if, if I want to update also multiple reports based on the conditions, then in that case, I will use updated. 
 0:58: So yeah, that. 
 1:01: OK, tell me the power of application if, you find out any exceptions or any error. 
 1:08: So how do you take it, using because Microsoft provides some tools to check the application error. 
 1:16: But do you know what tool is available from Microsoft or are you doing? 
 1:23: testing with that tool before creating the package for deployment. 
 1:29: Yes, in like Canvas Power app, the main Microsoft tool like I use for troubleshooting is Power Apps monitor or live monitor. 
 1:36: Like, it lets me see what is actually happening while the application is running, including data source, calls, like errors, warnings, response times, and like I would normally start with the app checker during development because it identifies formula issues and every. 
 1:55: Other problems directly in the app. 
 1:57: Like then if I have runtime issue, so like for example, a patch is failing or a database query is returning an unexpected result, I would like to open live monitor to reproduce the issues and look at the failed event to like understand what the error details and underlying data operations and like I can also use the trace functions like. 
 2:23: important parts of the application such as on select, on visible, or on start as well and that, that actually allows me to write custom diagnostic information into Life monitor. 
 2:35: So like if, if I were explaining my Debugging approach, I would say like first I use app checker for formula and design time issues and like for runtime issues, I like use power, power apps monitor or live monitor to trace the applications, emails and a data operations. 
 2:59: OK, Jay, I'm good from my side I think we have a. 
 3:04: Yeah, OK, so I have just a few questions and then we will wrap up, so, I have one to tell you. 
 3:16: Yes, yes, I do. 
 3:16: Thank you. 
 3:17: Thank you so much. 
 3:18: Thanks. 
 3:21: By a team, I would be. 
 3:25: OK, so I have one scenario. 
 3:26: Let's say. 
 3:29: There is a sales order, right, and, the sales order is created and the sales order amount is more than 1000, then, I would say like 10% discount will be applied, but, when it is less than if the amount is less than 1000, so it should not apply that discount over there. 
 3:53: Now you need to implement this using plug-in. 
 3:57: So what would be the process? 
 4:00: OK. 
 4:01: So, for that scenario, I would like, I would implement this using a database, plug-in registered on the sales order, like, most likely on the create and update messages, like depending on when the business wants the discount to be calculated or not, and I would say the first thing I would like to clarify is whether the discount should be applied automatically when the order is created or also recalculated whenever the Order amount changes. 
 4:35: So like for the execution stage, I would, normally consider pre-operation if I like want to calculate and set the discount before the sales order is committed to database or not that like I would say like for the for the or inside the plugin I would first get the sales order amount from the target entity and for an update message I would also consider the pre-image if like if I actually need the previous value or. 
 5:05: So if the amount isn't included in the update request, and then I would apply the business loan. 
 5:11: Like if the if the if the order amount is greater than 1 lakh, I would calculate a 10% discount. 
 5:18: So you will, you will register this again in what event? 
 5:23: It's, is it in pre-operation or pre or post-operation. 
 5:29: So I would register the plug-in on the like create and update events of the sales order, you know, like because the discount needs to be, so this is the message event I'm just asking about the event. 
 5:39: So what event you will register like for like I would say for pre-operation stage. 
 5:46: I would register it in the pre-operation stage so like I can calculate the 10% discount before the record is committed to database like particularly for the yeah OK. 
 6:01: Did you get a chance to work on the custom accent? 
 6:06: OK, so what kind of work you have done on So, for custom actions I have worked with like in BC 65 or data was mainly when, needed to be encapsulate a specific business operations that could be, called consistently from different parts of the applications like for example, in one scenario we had a business operations where multiple validations and updates, Needed to happen together. 
 6:34: So like instead of putting that logic separately in different power automate flows or client-side JavaScript, we could expose it through custom actions define the required input and output parameters, and I have worked with the like input parameters and output parameters like where the calling application. 
 6:53: provides values such as record ID or business specific information and actions that returns like results or status and like the advantage I see is that the business logic is centralized and reusable, like multiple consumers can involve the, you know, same operation rather than just duplicating the logic, so. 
 7:15: I would say like I have mainly use custom custom actions for like reusable business operations, centralized validations, record updates, and yeah, it's excellent. 
 7:26: OK, and so what scenario you will choose, like definitely hear about the custom API as well, right. 
 7:36: OK, so what's your you will choose to use custom API and the custom medicine. 
 7:43: OK, so yeah, just give me a short answer. 
 7:45: OK, like I would choose between custom API and custom action based on the requirement and the direction of the architecture. 
 7:52: Like, both can expose custom business operations in data works. 
 7:57: So, but for implementation, I would generally prefer custom API because it is, designed as a more modern and flexible approach for creating any custom operations, yeah. 
 8:08: OK. 
 8:10: OK, and just give me, just tell me the process of how you can debug the plugin. 
 8:18: OK, so for debugging the plugin, I would like to, normally through a structure process like the first thing I usually use is a plug-in trace logging. 
 8:31: And like, I, I enable tracing in the environment and use eye tracing service inside the plug-in to write like meaningful information such as plug-in, execution stage, record ID, important field values, and like which part of the business logic is being, executed and like after reproducing the issue, I check the plug-in trace, OK, that's fine. 
 8:56: And I just need to, check code line by line. 
 9:01: Of the code, how we can debug that. 
 9:05: my load code. 
 9:06: OK. 
 9:07: So like for line by line debugging, I will use Visual Studio with the database plug-in profiler and like I will first register and profile the plugin using the plug-in registration tool, reproduce the plug-in, execution and capture the execution profile, and then I open the plug-in project in Visual Studio, make sure the corresponding, Source code and symbols are like available and then attach the captured profile to the debugger and I, I can put breakpoints inside the plugins and then after that, I like replay the captured profile and Visual Studio stops at the breakpoint and like I can use step over, step into and step out to like execute the code line by line. 
 9:59: OK, OK. 
 10:00: OK. 
 10:01: Thank you. 
 10:02: I'm done from my side too. 
 10:06: so yeah, thank you so much, Thank you, thank you so much. 
 10:10: Thank you so much. 
 10:11: Have a good day. 
 10:15: So I actually have some questions with you. 
 10:17: Can I ask? 
 10:18: Yeah, please. 
 10:19: So, like, I would just want to ask, like, firstly I want to like know what will be the major, roles and responsibilities will be there for me, like if I get hired. 
 10:31: OK, I think I can answer on this. 
 10:40: Sure and let you know, OK, you can connect with. 
 10:46: OK, so one last question with that like, what will be done? 
 10:51: Like, is there any, any other rounds or like apart from this? 
 10:58: Yes, there will be, more, interviews, like maybe one or two, will update you accordingly. 
 11:05: OK, OK. 
 11:06: Thank you. 
 11:07: Thank you. 
 11:07: Bye-bye. 
 11:08: Have a good day. 
 11:09: OK, thank you. 
 11:10: Thank you bye bye. 
 11:16: Bye. 
