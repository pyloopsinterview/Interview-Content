0:00: How are you? 
 0:01: I'm good. 
 0:02: I'm good. 
 0:02: How about you? 
 0:03: Fine, fine. 
 0:04: Very good morning. 
 0:07: Great, let's start now. 
 0:16: can you transfer me, you know, sure, sure, yeah, thank you. 
 0:17: So yeah, my name is Shina Ross. 
 0:18: I have, 3 years experience and as a Python and AWS data engineer like design. 
 0:23: And then looking like enterprises scale data engineering solutions and like cloud needed ETL platforms and also like high performance data pipelines like that and also like I have my core expertise lies in like Python, AWS Apache Workflow and like. 
 0:42: Also, like on the Snowflake side, DBT SQL and enterprise like data integration and also like we have just build our scalable and reusable and like a production ready data platform for like large healthcare organizations and also like like like my currently I I'm working with Tic Healthcare and like where I'm part of like detention team like which is like responsible for the, let's say building and maintaining the enterprise data platform and like that like that process them like millions of clinical and claims like records and provider records pharmacy and like operation records for the analytics and compliance and also like and also like my primary responsibility is like developing like reusable Python EDL frameworks and also like Apache flow that DAGs and. 
 1:37: And that like that automate data ingestion and transformation and also work on the APIs and S3 EWS S3 and external data sources. 
 1:47: So like that also if I talk about like on my EW side I have worked extensively with S3 ECS and IM and EW Slamda to build like secure and scalable data platforms and I follow like, we did with security best practices for like implementing IM will be success and script encryption standards like secure the like coding guidelines and control access to DVD profiles and enterprise data data sets. 
 2:16: So yeah, that's major, work of you know to know. 
 2:22: Oh, perfect, perfect. 
 2:23: So let's say that you have an S3 bucket which is containing very critical logs, right, and must be accessed by ECS tasks, right, for analysis, right? 
 2:36: But you recently found out that there are unauthorized access attempts, right, which happened. 
 2:43: So how would you investigate this incident. 
 2:48: like, remediate the exposure and prevent future unauthorized accesses, right? 
 2:55: And you should consider definitely IAM, bucket policies and monitoring. 
 3:02: OK, OK. 
 3:03: If I have to like, consider this, I am and bucket policies. 
 3:07: So first of all, I would say like, for that part I, like. 
 3:14: I would check like cloud trails logs first of all, like to see where who tried to access the 3 bucket and when the like access happened and like from which I enrolled or like whether the request were, you know, successful or denied and I would say like along with that I would also review that clog box logs and any application logs from the, you know, ECS. 
 3:36: As to, you know, understand whether the access came from the our application or from an unexpected source. 
 3:42: That's really important because, next I would then review that I am rule attached to the, you know, it's, easiest task and I will verify that. 
 3:52: the task are using the correct IM task rule or that, that rule follows the, you know, principle of, least privilege, first of all. 
 3:59: So, and after that, I would see that, I would review the ST bucket policy and I would, make sure that bucket allows only like access only from the required ECS, IM rule and then, then explicitly like, denies the public, access, first of all. 
 4:17: and then I would also verify that it should, that block public access is, is enabled first of all because sometimes maybe we are making some silly mistake and remove any like overly per like permissive policies and then ensure that only trusted like principals can access the bucket. 
 4:36: And if I identify like any compromise credentials or unnecessary IM rules, users or rules, then I would revoke or rotate that those credentials immediately and update the affected applications. 
 4:50: So overall, like my approach is like this first investigate and the full access and then next time rules and, you know, and bucket policies then. 
 4:59: , I mean fixing that and after that remove unnecessary permissions and rotate, compromised credentials if needed and finally like strengthen the monitoring and auditing the similar incidents. 
 5:16: Perfect. 
 5:17: So now let's say a company stores sensitive customer data, right, again in S3 and they run containerized apps in ECS, right? 
 5:28: During a security audit, you found out that some ECS tasks are like no overly permissive, like I'd say permissive in IM rules, right, particularly. 
 5:42: So with full access, how would you redesign the IM policies? 
 5:46: Right, to minimize the risk. 
 5:49: While ensuring that the whole functionality is functioning smoothly. 
 5:54: OK, OK, got it. 
 5:55: So, yeah, of course, in this case is also, I would say very general, take care of, things we have to take care. 
 6:02: So I would say like, in this situation, the first thing I would do like, understand exactly what the ECS application needs to access, and I would review the application flow and identify like which is the bucket and you know, and actions are actually like required and for example, like if the application only needs to read files from a specific bucket. 
 6:27: Then it, it only needs permission like if we get object only and if required, then if we list object and there's no reason to grant, you know, full S3 access to someone or for, for any reason. 
 6:40: So like there should be proper handling of the access first of all and then I Update the ECS task rule by like replacing the broad permission, you know, such as S3 we we report start through that and with with only the it's a specific actions and resources application required and I would like to put the. 
 7:03: Policy to the, you know, required bucket or even like a specific folders like instead of, you know, having access to all buckets. 
 7:10: And after making changes like I would test the application in our lower environment to like make sure all the required functionalities are still working. 
 7:18: And if everything goes like correctly or perfectly, then I would deploy the updated IM policy to the production and to further improve like security, we can continue to, you know, like following the like same principle of the lease privilege and like avoid the like using long term credentials or like. 
 7:38: IM rules, for the, you know, easiest task, or like I would like keep the cloud trail enabled so, so we can monitor access and like quickly identify any unexpected activity. 
 7:50: So that's, a standard approach. 
 7:55: Can you repeat the last part quite loudly because I think so your whole answer was very feeble. 
 7:59: So if you could look at least the last part, yeah, yeah, sure, sure. 
 8:03: So like, to further improve the security, I would, like continue the, like principle of lease privilege and avoid the like, using the long term credentials. 
 8:15: Sometimes, you know, we are using the long term. 
 8:17: Credentials, for, for like not doing those things, continuously or, or for, sometimes like people make changes like for 6 months or 1 year, make those, mistakes I would say. 
 8:30: So use those, not using those long term credentials, and also like use the IM rules for the like easiest task and also like, I would say I have also keep the cloud trails enabled so we can monitor access and quickly like identify any unexpected activity and that's we can help we resolve this problem and solve this issue. 
 9:00: God. 
 9:01: So now let's say that you are working with DBT models, right, and they are like significantly taking longer time, right, that to, you had some recent changes, team changes, right, and new data sources also came in. 
 9:19: So how would you investigate and optimize this DBT pipeline to improve the overall performance. 
 9:27: of the process. 
 9:29: OK, OK. 
 9:31: Got it, fine. 
 9:31: Then I would, in this case, I would say like if I have to work, for sure, like first I would review the DBT run logs and identify like which models are taking the most time. 
 9:43: And then I would like to check whether the slowdown is happening during like source injection or maybe like model execution or while like writing the data into the snowflake. 
 9:54: So, with that, I would like to look at the, you know, data, new data sources. 
 9:59: Like sometimes the volume of the incoming data increases significantly and then the full data quality changes. 
 10:06: So which can, you know, impact the downstream models and And we can verify like whether the new forces are introducing larger data sets or the additional transformations are doing that. 
 10:17: So after that, we can review the recent modified DVT models and then I will check if anyone like introduced the expensive joints or like unnecessary joints or Necessary CTs and, you know, sometimes like repeated transformations are there or like full table scans are there. 
 10:35: So if a model is building that, the entire table every day, I would like to see whether it can be, you know, converted into an incremental model so that, so only new changes are required are, you know, Like process instead of, you know, entire data sets. 
 10:52: So that's that would the approach of mine and that's how I can like tell you the snowflake query performance and make sure like continuously monitor the pipeline to make the short like optimization is effective and impacting, I, I mean without impacting the data quality. 
 11:15: Sure. 
 11:16: So now let's say that you have discovered, no, very critical DBT model which is developed by another team and you identified that their results are inconsistent, right? 
 11:28: After the warehouse update, like there's been a warehouse upgrade, upgradation happened and you are seeing inconsistent results. 
 11:35: So now systematically, how would I, how would you identify the route first, right? 
 11:41: And Make sure that no, this future model is reliable. 
 11:48: OK, OK. 
 11:49: So, for making the future model reliable, first of all, I would check that, if we are doing, I mean, like if I notice that, like artificial DVT model is giving inconsistent result after, you know, warehouse update or I like, since, since the issue is started from the data warehouse, so, our, our data warehouse agreed, so I would firstly like verify whether the, input data going into the model has changed, and like I would compare the data before and after the warehouse agreed. 
 12:21: And by checking row counts or like schema changes. 
 12:24: Data types, mal values like that. 
 12:26: So if the GBT model is like, receiving, different or incomplete data, then it's very likely to, you know, that the data output is very will also be inconsistent. 
 12:38: So I would review the DBT model and the skill transformation that prepare the data for the GBT model, and I would check whether any joints filters like, like. 
 12:47: Like started behaving like differently after the upgrade. 
 12:51: So after that I would compare the outputs using the same input data in both, like old and upgraded warehouse environments. 
 12:58: If the results match, then the warehouse isn't the issue. 
 13:01: If they differ, if they investigated the, execution plans, query performance or any warehouse specific behavior that, you know, change after that week. 
 13:12: So yeah, once I identify the root cause, then I will fix the performance, perform like end to end regression testing, then using historical data sets to confirm that the output are consistent and accurate. 
 13:25: Yeah. 
 13:27: But So now let's say that you have not inherited an airflow environment where dads run occasionally, right, but get stuck in a running state for hours like you have the dog, workflows, right, which is definitely, creating problem for your downstream processes, right? 
 13:48: So as the airflow lead, how would you investigate the root cause, right? 
 13:54: And how would you prevent the reoccurrence? 
 13:57: And definitely, how would you enable monitoring systems for future if future prevention. 
 14:05: OK, OK. 
 14:06: So I would first open the airflow UI and like identify whether the task is remaining in the running state. 
 14:13: Then I would like, like my first step would be, you know, understand whether, where they are getting they they are getting stuck, rather than restarting them immediately. 
 14:24: And then after that, then I will check the task logs to, you know, like see whether it's, it's actually executing waiting or like for a report and like. 
 14:37: And like it's, it's actually executing reading or like blocked like because of external dependency and like next I would I would verify the health of the airflow components, you know, such as the schedulers or and like workers or like make sure that they are there are enough resources available and I would also like check whether the issue started after a recent code change or like after, you know, onboarding a new data source. 
 15:04: So that's how like if. 
 15:05: , that that is reading data from systems like S3 or APIs or like data sets, then I will verify those systems and, responding normally and also like, I have investigated that air, airport pipeline and like, also like, Analyze task logs and fixed issues related to ETL processing then redone the failed jobs and like monitored pipelines to ensure like downstream data processing continued successfully. 
 15:36: So that's will be. 
 15:41: Got it. 
 15:43: So now let's say you know, your team, particularly building the airflow that and definitely you are experiencing. 
 15:51: Like no unpredictable failures, right, due to, database outages happening during peak hours or some other X Y Z issue is causing that. 
 16:01: So, as the airflow architect, right, how would you redesign your DAs, right, and your airflow setup, right, to minimize the data loss. 
 16:12: OK, got it. 
 16:13: So, for, for that, first thing I would like, that, that work, that, that work I have done, previously, for a few times. 
 16:20: So like, it's, it's been a time like first I would identify whether tasks are like dependent on the database or for those tasks I would like configure appropriate like retry policies without like delay between the retries and so if the outage is like temporary, the task can recover automatically without manual intervention. 
 16:39: And if, like I would like also like add proper exception handling if the P in the Python code or whatever database or school and whatever code we are working in and if the, data connection fails, then the task should, you know, log the error clearly and exit the exit gracefully and then let a full flow like handle that dry instead of, you know, leaving the workflow, in an inconsistent code and Like, after that, whenever possible, I would, I like where, like, if there is possibility then I would break the large workflows into a smaller, independent task, that way, like, in one database related task fails, if like it fails, then we only like. 
 17:24: Even that and especially like task instead of restarting the entire pipeline. 
 17:28: So yeah, that's, will be the, I mean, foremost approach I would take and like we already like uses the retries and logins and like production monitoring to, you know, improve the, pipeline reliability. 
 17:41: So when like failure occurs we analyze the logs and resolve the issue and even only like affective task instead of, you know, entirely flow when it's possible. 
 17:54: I got it. 
 17:57: So now, can you share your screen? 
 18:11: So the chair. 
 18:21: Is it true? 
 18:23: Yeah, I think so. 
 18:26: I've shared you the Question and the editor, can you edit the code for it? 
 18:36: Are you able to sing? 
 18:41: So now this is a question. 
 18:43: We will have 15 minutes. 
 18:46: All right, to complete this. 
 18:48: OK. 
 19:05: Yeah, so I have to like that. 
 19:16: So I can do it anywhere like a notepad or something or I have to like here only. 
 19:23: Yeah, yeah, here only language you can decide between Python and here. 
 19:29: OK. 
 19:54: OK. 
 22:40: OK OK good. 
 27:08: So. 
 28:03: So yeah, I have just completed. 
 28:06: Should I explain that or is that I have to call this number to do that. 
 28:14: Is Jen big? 
 28:15: Yeah, yeah, it's. 
 28:19: Of course, I think so, for the time being. 
 28:28: Let's start with this, no. 
 28:34: I'm sharing with one both of you. 
 28:40: You know, So that means. 
 28:46: are you able to see the updated version? 
 28:48: Yeah. 
 28:50: Like, let me. 
 28:53: Yeah. 
 28:55: I can see that. 
 28:57: Yeah, can you start working on this one? 
 29:00: OK. 
 29:16: OK. 
 33:25: So yeah, yeah, that's that's what I done and like and that I have calculated the like to rule sales for each customer whether like I be using like even some and upside down and after that I use that with like. 
 33:41: Partition by region and like ordered by tolec in the in the. 
 33:48: Like highest sales get ranked one. 
 33:51: So like that and also like I use the dance rank because if it's if like two customers have the same total sales then they receive the same rank and this, this can be insured like insured like ties are handled correctly and after that like finally I will, like return only like road where like rank is less than equals 3 and You know, which it gives the, you know, top 3 customers in each region, and, I think, yeah, this is the efficient it is, first, aggregate the data and then like reducing the numbers of rules before like applying the window function, yeah, so I think it's optimized function and the. 
 34:39: Hey, hi, are you there? 
 34:42: Yeah, got it. 
 34:44: You can, stop sharing the screen. 
 34:58: So now, can you explain me one of your projects in your past experience with what were the challenges, right? 
 35:04: What was the situation and how did you mitigate? 
 35:08: OK, so yeah, well, like, as I have worked on some of the So, my, my team is like, our team is responsible for like building data pipelines that collects the data from multiple sources. 
 35:23: So like for like, one of the challenges we face is like, airflow pipelines we're feeling like, Intimate intermittently, like because one of the external flows are like was occasionally slow or temporarily unavailable. 
 35:36: So as a result, like downstream DVT models and, you know, reporting jobs were delayed. 
 35:41: So, to investigate the issue, I just check the air flow like task logs and to, you know, identify the exactly where the pipeline was failing and then. 
 35:51: Like I confirmed that, you know, failure will like, happening during, you know, data extraction from the personal source and not during the transformational loading stages. 
 36:03: So yeah, to address that issue, like, I updated the pipelines by like, adding the proper exception handling and retrial also. 
 36:10: But like retry delay run like detailing like detailed logging and instead of like failing the entire workflow immediately the pipeline could then automatically retry when that source system becomes, you know, became available again. 
 36:24: So yeah, that's all like it seems that because it's a, it's a general problem but the the scale is quite big for this and that's the big issue and we because we have to like introspect so much here and there and that's how like it takes time and in a week or two, like we are able to solve this. 
 36:44: at that time, like we are, we are like on the previous version so that's how it was. 
 36:52: Got it, got it. 
 36:54: Yeah, I think so. 
 36:56: I have these questions with me, so I think so about HR will be reaching out to you and you know she can direct you for the further next steps. 
 37:05: OK, OK. 
 37:05: So, yeah, may I know like, when can I get back or if you have any idea. 
 37:13: Sorry, OK, for, for this test, I have to contact the child only, or you can like give me the idea like when can I hear back from the child? 
 37:23: Yeah, probably today, likely or tomorrow, HR will be reaching out to you, and she'll be guiding you the next steps from here, like, like she would be the right person in terms of exactly telling you what is, you know, Next step because I'm just part of the recruitment side so I have like overall information but the specific HR would be the right POC but that overall I got all the pointers that I was looking for. 
 37:58: So yeah, you know, HR would be updating you. 
 38:02: Yeah, yeah, thanks a lot, yeah, have a nice day and, do share any feedback you have for the interview or something, then she can take it forward from there as well. 
 38:12: Sure, sure, thanks a lot, and yeah, I will talk to, so thanks a lot then. 
 38:17: Bye-bye. 
 38:18: Have a nice day. 
 38:20: Oh yeah. 
