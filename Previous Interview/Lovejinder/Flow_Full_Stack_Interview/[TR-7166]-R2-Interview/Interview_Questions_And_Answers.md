0:00: Nathanie. 
 0:01: Hi, good morning. 
 0:04: How are you? 
 0:05: Yeah, I'm good. 
 0:06: What about you? 
 0:07: I'm doing well. 
 0:09: I hope I've got your name right. 
 0:11: Loinder, is that correct? 
 0:12: That's correct. 
 0:14: OK, OK. 
 0:16: So Loinder, what I'll do is that I basically take care of the delivery for, the client from the HCL side. 
 0:22: The client will be joining in a minute. 
 0:24: keep the video on for the duration of the interview. 
 0:27: Any employment related questions, keep it to me or C, and not to the client. 
 0:33: Anything on the project and the text stack, feel free to ask the client and not an issue at all. 
 0:39: second one is I may drop off a post introduction so you'll continue the interview with the client and then I'll loop back with the client for the feedback and keep you posted. 
 0:48: Yeah, that works. 
 0:52: Just give it a minute for the client to join in. 
 0:54: I think he's here. 
 1:01: Hey, how are you? 
 1:03: Hi, hi, good morning. 
 1:05: Hey. 
 1:05: Hi, good morning. 
 1:06: But I don't know. 
 1:08: I've got, I've got your video on, but it's just the background? 
 1:11: Yeah, yeah, yeah, no, no, I, I didn't do no, no, I even actually what I is generally switches to, camera which is attached to the office machine. 
 1:27: I don't know why that didn't happen. 
 1:30: No, I was, I was like the video is on and where is Warun here, you know, I don't see on the video. 
 1:35: Yeah, yeah, OK, so Warun and Lavinda, just give me one minute. 
 1:39: I'll make you both the presenter so that if somebody drops out, you guys can let each other in and Warun. 
 1:44: I need to chase up the HR on a few transactions, so I'll drop off post-transaction post the introduction if it is OK with you. 
 1:51: Yeah, yeah, yeah, so Lajina, please go ahead and give a quick introduction about yourself. 
 1:55: We'll take it from there. 
 1:57: Yeah, sure. 
 1:58: So like, hi, I'm, like my name is Lajina Singh, and like I live in experience in back and development, primarily working with Python and Django. 
 2:09: like my core expertise is in Python, Django, fast API flask. 
 2:14: working with the APIs, microservices, and like SQL and OSQL databases, both, and a cloud. 
 2:21: And like, talking about like my most recent experience, I have worked with Selective Insurance as a lead Python developer, where like I was working on enterprise insurance platform, like, you know, like where we build backend services to integrate, you know, processes, policy and like claims information from, you know, like multiple streams. 
 2:38: And like my main responsibilities there was like, you know, mainly around designing and developing Django Django and like list APII and microservices, along with like, obviously, like database optimization, scalability and security. 
 2:52: And like one area that I worked heavily on was like AP performance where like as, you know, as a number of users and I would say downstream applications increased some APIs, you know, started slowing down. 
 3:04: And yeah, like I analyzed the application and I would say data database bottlenecks, optimized post-scale SQL queries, added indexing, and introduce, you know, the main concept like red caching. 
 3:17: And like afterwards I would like I have also worked with Azure Data bricks, Ice Park and like Delta Lake for like large scale data processing. 
 3:25: And like in my lead roles I have been involved in, you know, like architecture decisions, code reviews, mentoring developers, and like working, you know, closely with QA and DevOps teams. 
 3:37: So yeah, like, overall, I am hands on on back in and like engineer back engineering side. 
 3:43: And, you know, like to solve performance and like a scalable scalable problems. 
 3:48: Mhm. 
 3:50: So yeah, I mean that's good. 
 3:52: So let me introduce myself as well, right. 
 3:56: So my name is Varun. 
 3:57: So I've been with the Bank of America for close to 18 years, and then I joined SNBC in February, right, and to lead this platform called as chip, valuation control, so the role I'm looking for is A, a kind of a technical lead right who can basically understand, do the back end design work with me, understand the requirements, and, Kind of do the design discussions right as well as hands on coder as well, right? 
 4:36: It's kind of a senior engineer lead kind of the role is what I'm looking for. 
 4:40: So the current team size we have, one, front end developer, yeah, we have one back end, right, he's with junior and then I need one more to kind of, help him out and do the work right in the back end. 
 4:57: so the technical stack is, React, Python Django, and then we have data mix, and then also sequel it as well, alright, so yeah, so any questions along in there on the role of the technical stack. 
 5:11: No, like, yeah, like you said that, like you have been working on Python frameworks, So like one question that I would, you know, have is like around the back end architecture, like since you mentioned that React is on the front end and like Django on the back end, so like, are you primarily building rest APIs and like services between React and Django, or like is there a larger data processing workflow? 
 5:35: So there are both right. 
 5:36: So there is a data processing workflow and that happens every day. 
 5:39: There's a batch that runs every day, produces some results, and, stores those results in the data bricks, and, there is also, user part to this, right? 
 5:50: So we are then taking those results, displaying to the users. 
 5:53: And then the users are allowed to make adjustments on top of the data set. 
 5:58: OK, yeah, that, OK. 
 6:00: And then you take the adjustment, and then there, and also there is a big, big workflow around it, right? 
 6:04: So there is some approval workflow. 
 6:06: There is some sign off workflow. 
 6:08: There is a reporting. 
 6:09: There is a downstream feeds that this is a typical enterprise application, right? 
 6:14: so, and that's where, there is an interesting challenge given that all of our big data breaks is in the data lake, right? 
 6:21: How does this? 
 6:23: More like when you do an adjustment, which is more like an OLTP kind of environment, how does that work with a data? 
 6:29: So yeah, something that we need to investigate a bit. 
 6:32: I mean, those are the kind of challenges we'll get to work with in this project, yeah, yeah, yeah, that perfectly works. 
 6:38: Like you explained everything and like, you know, actually one of the, I would say like one of the more interesting parts of architecture. 
 6:46: Yeah, yeah, exactly, so. 
 6:49: So why don't you just walk me through, one example, right, what you have any of the project, right, and then what is the feature, what's your design, right, and what are some of the challenges you face when implementing that feature. 
 7:05: Yeah, sure. 
 7:06: So, like, one example that I can walk you through is like, from my recent project at Selective Insurance, like where we had a similar pattern of I would say, operational applications, you know, consuming data that we are coming from like multiple backend systems. 
 7:21: For example, like we had policy and claims information that we know, I was coming from different source systems. 
 7:27: So like at that time, we first processed and like validated data, that data. 
 7:32: applied business rules and like made it, you know, available through our, I would say Django-based APIs and like on the transaction, how did you run these data loads? 
 7:40: What, what technology have you used for the data loads? 
 7:43: Yeah, for the data loads, the, like specifically I have worked mainly on post SQL and, SQL databases including, I have also worked with Mongo DB and Azure database. 
 7:54: OK, after that. 
 7:54: OK. 
 7:56: And then, so you read from those databases, and then, so you have the different processes running. 
 8:01: how does your batch process look like? 
 8:04: Yeah, so like, for particularly like batch processing, so it like it was a scheduled pipeline that I would say like ran on a regular basis, but primarily with, you know, like for processing and transforming larger data sets and like we use Azure databas and Pipe Spark for like that processing. 
 8:21: And you know, like the batch would read data from that upstream or I would say like operation systems and perform validations there there were afterwards and like transformations and then afterward like apply the required business rules and like writing the process results into data tables. 
 8:38: No, like, yeah, so data tables and like, you know, optimizing the P spark transformation. 
 8:44: So, so you have used PySpark, right? 
 8:48: You're connected to a SQL database. 
 8:51: And then you loaded it into the deductible. 
 8:55: So how does the orchestration happen? 
 8:57: OK, so like, in, in that scenario, the orchestrations, is like, you know, like we use a scheduled workflow around the database processing and the basic flow was like that, you know, the pipeline would start on a defined schedule and first validate that the source data was available or not, and then like trigger the file is all this, schedule and everything is in, Is in data breaks only, yeah, everything is data breaks. 
 9:26: OK, yeah, OK. 
 9:29: So yeah, like I've. 
 9:32: No, OK, so, so you have this different pipeline set up to connect different data sources and load it into the database tables, OK. 
 9:39: So how did you ensure that these processes are they run right into different tables, are they right into the same table, like, like for, for that, if we are writing on the same table or not, like it depends on the type of data and like the processing stage. 
 9:53: So like we generally didn't have, I would say like every pipeline, writing directly into the same table. 
 9:59: like we separated that data into, I would say, a logical layers and like tables. 
 10:05: So, you know, like, so that like each pipeline, I'll say has a clear responsibility. 
 10:09: For example, like the raw or source level data would be landed first. 
 10:14: And then the IP for transformations would create the processed or like a standardized data tables and like from there on we could have curated tables that were like specifically if I have to show a report joining the data between all these tables that been produced by multiple jobs how do you show it to the user. 
 10:37: OK, so like if it is produced by multiple jobs, so if, if, so I have, so you have the same case, right? 
 10:43: You have the data that you need to fetch from 5 different systems, then the requirement is to join them and show it to the user. 
 10:51: OK, let's say you have a report, and then you say, OK, this is column A, B, and C, and then this is the value X, Y, and Z from System A, value, something else, alpha beta gamma from System B, something like that. 
 11:08: You want to show it, right? 
 11:10: So how does your design work for that? 
 11:14: Yeah, so, like, yeah, that's a pretty good question. 
 11:17: like, like to be in that scenario, like I would firstly, I would avoid making user facing application for like all five systems every time the report loads, for like that would make the application tightly coupled to those systems and like, you know, could create performance and availability issues. 
 11:35: So rather, like I would design it as a, I would say a data aggregation pipeline. 
 11:39: For example, like, let's say, let's say like we have a system, and, you know, System A, through System E. 
 11:46: So like each system provides a different, I would say part of information. 
 11:50: And yeah, like we would first ingest the required data into databas and like preferably, you know, like, say incrementally, you know, where the, where it is possible. 
 11:59: And then in databas I would use Spark or SQL, you know, to standardize the schemas, validate the data and like join the data sets using, like the appropriate business keys. 
 12:11: For example, like, let's consider like if we have a customer ID or, let's say an account ID, let's say these are the common keys. 
 12:19: So like we could build something, I would say like a system A that has, let's say, let's say it has a customer information. 
 12:27: we have a System B that has account information and you know from there on, many more. 
 12:31: So like then we create a, I would say a curated, reporting data set that contains, so when do you do the join actually? 
 12:38: So, so when does the joint happen? 
 12:41: OK, so like in that process join typically happens, I'll say like in the data breaks data processing layer, particularly before the data is presented to the user. 
 12:52: So I have, OK, yeah. 
 12:55: So my Django API is calling. 
 12:57: So what does it call, right? 
 12:59: It calls the report table. 
 13:01: Or what is that my jango AP calling to show it to the user what data that you are exposing to the Janway AP. 
 13:09: So like the yeah, you currently feel like the Django API is like it's, you know, it's calling the the that and like, yeah, like I would expose a curated or like report reporting ready data set to the Django APA in that scenario and like rather than, you know, exposing the individual source tables. 
 13:28: For example, like after database processes the five source systems, like in that case we could have a curated data table like a reporting, like, let's say a reporting evaluation results, and like that data set would already contain the required fields, from the system A, through System E, and you know that join. 
 13:47: OK, so if you have, so you have a stored table from System A to system and you have all the columns from System A to System A. 
 13:55: Now your job. 
 13:57: The pipeline for System A is running right. 
 14:00: So what do you do? 
 14:02: And the pipeline from System B is also running, right? 
 14:05: So let's say both of them have completed at the same time trying to update the table. 
 14:10: How do you handle the concurrent issue in that case? 
 14:13: OK, so like in that case if System A's pipeline would, would load, yeah, so like, is it System A and System B, right, the pipeline from System A and System B trying to access the same table and trying to upgrade for the same key, it's corresponding loads right you're running into a concurrency issue. 
 14:33: Great. 
 14:33: How do you fix that? 
 14:35: Yeah, like that's a good concursion scenario. 
 14:37: So like to be in, and like, in that scenario, like I would first avoid having both pipelines, to directly overwrite the same target table at the same time. 
 14:46: For example, like each pipeline can write its own, I would say staging or, like source specific data table first. 
 14:54: And once, like, you know, both pipelines completed successfully, or downstream orchestration at that time, like, downstream orchestration step can perform, I'll say the final merge into the curator table. 
 15:06: So how do you configure this downstream orchestration? 
 15:09: So like how to conquer it. 
 15:10: So you're basically synchronized serializing it, these, jobs, right at the downstream market, orchestration, right? 
 15:19: How do you concealize it, during that time? 
 15:22: OK, so like for, for the for serializing that, like I wouldn't necessarily serialize the entire pipeline, because, you know, like that would reduce throughput. 
 15:32: like. 
 15:33: I would let System E and System B run in parallel and like only and serialize only the shared table update. 
 15:40: And yeah, like I would handle that in orchestrationally using like that answers your question. 
 15:45: So like in orchestrationally using your dependency or I'll say your fanning pattern. 
 15:50: So yeah, like the orchestration, we like orchestration beats. 
 15:54: So when you say dependency, right? 
 15:55: So how do you do the dependency? 
 15:57: How do you use dependency? 
 15:59: Oh, so like using dependency there. 
 16:02: How do you use the dependency to serialize this, issue, right, the concurrent taxes. 
 16:08: Oh, so like, I would implement the dependency in database, like workflow, workflow layer, and, so see like if, so, so that's what, right? 
 16:16: So see what I'm trying to answer is. 
 16:18: It's a simple cooking, right, so you have two pipelines Source A source B. 
 16:23: We have one single table. 
 16:25: That's a source A and source B both have completed. 
 16:28: So now you say you have another pipeline which is dependent on both A and B right now. 
 16:38: How do you implement the dependency so the system AA are updated first and System Bs are updated next. 
 16:46: That way you are not overriding, right? 
 16:48: Yeah, yeah. 
 16:49: OK. 
 16:50: So, like, if I want that to be there, like. 
 16:54: If, if the requirement is specifically that system A must update first and like System B must update next, no, it's not, it's not one of, one of it has to update first and one has to update next, right, but we don't want both of them overwriting each other's updates. 
 17:09: Yeah, so, like if, yeah, in that scenario like. 
 17:15: In that case, like, I would avoid having both pipelines directly right into the same shared table as I discussed, and like I would have a System A and System B right to like separate staging delta table first and like then a single downstream job would be, I, I say like would be responsible for updating the shared target table and like if, if so in that single, downstream job, right, so how do you do that, merging when do you do that merging, log in. 
 17:44: Yeah, so like in that a single downstream, what is your logic in that the downstream, pipeline? 
 17:51: So you write the its one after the other and prepare the final table. 
 17:56: So like I would do the merge after both source pipelines and like have completed successfully and you know their staging tables have, like past validation. 
 18:06: For example, like is, like if the downstream merger would use the common business key, say like account ID or say like a record ID to determine whether a record already exists. 
 18:17: So like if it exists, we update the appropriate columns, and like if, if it doesn't exist, like we insert a new record and like particularly with the Delta lead, I can use like a merge into operation. 
 18:30: So like you know that like that update is, I would say a transactional anatomic. 
 18:35: So yeah, like, so the important point is like I don't know why, you know, A is still running or like while B is still running in either cases. 
 18:43: I will wait like until both are complete, validate the data, and like, you know, they have own, you know, controlled downstream job, perform the, you know, merge into the shared curated table. 
 18:55: So yeah, that would be my approach. 
 18:58: OK What, alright, so once you get the table now you give it to the user, right, now user wants to do an adjustment, right? 
 19:08: He wants to adjust a few columns, right? 
 19:11: So how do you design the adjustment. 
 19:15: OK, so like for the, for the adjustment part, like I would treat it as an OTP operation firstly, not directly, you know, update the database batch, table from the UI. 
 19:26: So like when the user changes a few columns, say, the react application would send the adjustment to a Django APP, and after that, like Django would validate the request and like check authorization or like apply the business rules and then store the adjustment in say like Azure SQL or any like transactional database. 
 19:45: And yeah, like I would keep the original batch, like, you know, batch result unchanged and like store the adjustment separately. 
 19:53: For example, like we, we like we could have an adjustment table with fields, so like with fields like record ID column name, or, you know, the, or the adjusted values. 
 20:04: So like if, if, if there is an approval workflow, in that case, like the adjustment would initially be something like pending. 
 20:12: And like after that, the appropriate user approves it. 
 20:15: So like it becomes approved. 
 20:17: And yeah, like then the reporting layer can combine the original I'd say like it can combine the the like the original databa result with the approved adjustments. 
 20:29: like, if, if, if, so you are going to, so let me understand. 
 20:33: All right, user comes in, user uploads an adjustment, right? 
 20:37: Overwrite some of the things you first store it in the other SQL database, OK. 
 20:42: So when are you going to then take other SQL database adjustment and override it? 
 20:46: When do you do that? 
 20:47: Oh, so like for that, like, like I would, but yeah, I, I would not immediately override the database best data when the user submits the adjustment. 
 20:57: The adjustment like is the stored first in address given or with the status like pending and like yeah once the required approval or sign off is completed it becomes approved at that time and like then I would then I would have an incremental downstream process you know pick up the newly approved adjustments yeah so like that process can run on a should be but how do you, how does that process run? 
 21:19: Is it like, how do you trigger that process. 
 21:22: OK. 
 21:22: OK, so like for, for triggering that process, like I would use, I'd say like different mechanisms depending on, you know, how quickly the disease needs, needs the adjustment reflecting, reflected in data breaks. 
 21:38: like for, for like normal batch oriented requirement, there is, there is no need of any sign off, right? 
 21:45: So what the user's requirement I need to upload, I need to upload it. 
 21:50: and as soon as I upload it should get upgrade and refresh the report should refresh. 
 21:56: OK, it's more like a real time that you need to do. 
 21:59: So how do you change your design in that case? 
 22:03: OK, so like in that case I would make the adjustment flow, like near real time, rather than I would say like waiting for a scheduled batch. 
 22:11: So like when a user uploads the adjustment, the Django API could, say like validate it and save it to as your rescuer. 
 22:18: And yeah, like once all the transaction, the transaction succeeds, then I will trigger the downstream process immediately, you know, ideally through an event or you can say a message-based mechanism like the processing service would pick up that adjustment. 
 22:32: So how do you invoke it, so you have your, data in a data breaks or a data lake, right? 
 22:39: So how do you invoke? 
 22:41: Do you know the mechanism by which you can invoke that process to any aspect to any of these data leaks, like, If the main data, yeah, yeah, so if the main data set is in, database or data like I would use that mechanism. 
 22:57: I would use the event driven mechanism for that immediate, you know, adjustment requirement, and, yeah, the key is like to like that like I wouldn't have Django directly modify the data table, and Django handles the user transaction and records the adjustment in Azure SQL. 
 23:13: So like once the transaction is committed. 
 23:16: Like then it publishes an event, containing something like an adjustment ID or like a record key, you can say where do you publish this event. 
 23:27: Like pub publishing, like where do I publish this event, so like, like I, I would typically, I would typically publish the event through an event broker rather than directly calling the data with job from Django. 
 23:41: Why can't you call the data pick up from them. 
 23:46: So like, why can't I like I, I don't know right, why you want don't want to call the job from junk. 
 23:55: yeah, like if. 
 23:58: Like, in that case, like I, I would say like I don't, if I, if like I don't want to call or pull the data from data lake, correct? 
 24:08: That's what you're asking. 
 24:10: Yeah, all you need to do is apply the adjustment. 
 24:13: Now the adjustment is buying in another sequel. 
 24:15: Your actual report table is in data bricks. 
 24:18: You need to somehow apply that adjustment on the data break, the table sitting in the data bricks, enrich it, and then show it to the user. 
 24:26: OK, OK, so how do you do that mechanism, right? 
 24:31: You are saying, OK, event broker, which is fine. 
 24:34: I just want to understand, how do you then set up the, the, let's say data breaks to basically listen to this, right? 
 24:41: Is there a listener? 
 24:42: Have you worked on any of this event brokers? 
 24:45: there's a simple solution which is invoking the data bricks job from a job, right? 
 24:50: So why you don't want to use that? 
 24:51: What are the downsides you are seeing to use that? 
 24:53: I would say let's use that. 
 24:56: Let's remove the job which then just reads the table from SQL, applies it on your table, and then goes for it. 
 25:05: So what's the problem with that? 
 25:08: like, firstly, like that's a very fair point. 
 25:11: like I have, but I have worked with, there is a problem. 
 25:14: See, you, you, you have a point in using broke, right? 
 25:17: There is a problem with, invoking the AP. 
 25:20: I want you to tell me what the problem is. 
 25:24: OK, so like the problem, main problem, I would say is that latency. 
 25:30: If, if like Django directly invokes a database job, like the job as a startup and scheduling overhead, in that case, like the user expects the report like to refresh immediately, so like waiting for a database job to start and like complete, you know, that may not meet the requirement. 
 25:47: And yeah, so like, and also like what about if there are multiple APA calls happening because multiple users committed transactions? 
 25:56: What if multiple APA calls are happening, multiple jobs are running. 
 26:00: All right, and the processing it, how do you handle that? 
 26:03: So like, in that case, I would not let every API request blindly start the separate, database job. 
 26:09: So like if, if, like if I have 50 users submit adjustment at the same time, like that, that would create, you know, 50 database job runs. 
 26:18: So like first each Django request, you know, permits the adjustment to say Azure SQL with a unique adjustment ID and let's say a status such as pending. 
 26:28: And like after that, then I, you know, I would I would like decouple the processing from the API request. 
 26:35: Then you know the API can trigger or in the work, but, but the actual database processing, that would be, that should be controlled so like multiple adjustment can be processed safely. 
 26:45: And like on the database side, like I would, I would like to process the pending adjustment incrementally as a batch. 
 26:52: Oh, for example, let me give you an example. 
 26:54: Like if, like if we have one job that could pick up an adjustment IDs, say like 101 to 150, you know, rather than starting 50 separate jobs. 
 27:04: So like for the shared data table, I would use delta transaction merge operations and like appropriate business keys. 
 27:09: So yeah. 
 27:11: OK. 
 27:12: All right. 
 27:14: OK, so we have 3 minutes long and that's any questions for me? 
 27:19: so, like, I would So, I like, I would want to know like what will, what would be the rules and responsibilities, particularly for this, like if I, I'd be high for that one. 
 27:29: So, so, so it's a hands on development tool, right? 
 27:33: So we do have the same stack, right? 
 27:35: We have a data base we have, where we have the data stored in delta tables, and we have this adjustment capabilities. 
 27:42: We have a jango layer, so you will be working on, developing the back end API. 
 27:50: designing for the features, right, the entire back and design for some of the features, right? 
 27:54: So one of the things is we have a calculation process which runs and the, saves the report down, and then we need to have this kind of a adjustment, but adjustment is not just enriching the report, it needs to retrigger the calculation, OK, and, recomputte some of the values. 
 28:12: It's not a straightforward adjustment, right, so. 
 28:18: Yeah, so basically those are there are requirements that are going to come our way to build this evaluation control platform, and we should be basically building out of it using this Django and data breaks. 
 28:32: It's mostly like a database design, hands-on coding, and delivery of the requests, and delivery of the stories, right, yeah. 
 28:41: OK. 
 28:43: So yeah, that makes sense, like, based on what you described, like it sounds like the biggest challenge. 
 28:49: The biggest challenge is like really the boundary between data breaks data like and like transactional user flow, workflow. 
 28:56: Yeah, yeah, OK, alright, log in that then. 
 29:00: Thanks for your time. 
 29:03: I appreciate the time. 
 29:03: I will talk to Sunday. 
 29:04: I have, like one major question. 
 29:07: So, like, what, what would be the further rounds? 
 29:10: Like what would be the number of rounds? 
 29:13: Oh, there is no number of phones. 
 29:14: This is it. 
 29:14: This will be the fun or maybe a submit that's it from my end to send it, yeah. 
 29:20: Yeah, OK. 
 29:20: Yeah. 
 29:21: All right. 
 29:22: All right. 
 29:22: Thank you. 
 29:22: Have a good day. 
 29:23: Bye-bye. 
 29:23: See you. 
 29:24: Bye. 
