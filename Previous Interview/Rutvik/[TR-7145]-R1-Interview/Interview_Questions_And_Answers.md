0:01: Hello. 
 0:01: How are you? 
 0:02: Oh, I'm good. 
 0:03: Good afternoon. 
 0:04: How are you? 
 0:05: I am well, thank you. 
 0:07: Thank you for joining a little bit early. 
 0:08: I didn't get a chance to. 
 0:09: I know we were, how was the weekend we were at a It was, you know what, it was good, fast. 
 0:15: It always go so fast, and we were at a, we were at a company event Wednesday, Thursday, Friday. 
 0:19: I don't know if Bob spoke like that, so it kind of was like rolling right into busy, right? 
 0:26: Is the end. 
 0:32: Hello. 
 0:33: Oh, we can see. 
 0:33: OK, perfect. 
 0:35: I always join at the beginning, just to make sure I, I had a glitchy interview earlier today. 
 0:40: Sometimes teams, likes to play one on us. 
 0:43: So I always make sure that I step into the middle. 
 0:45: But, Ruthbai, this is Ian, who is actually leading the effort on the Data landing zone, interview. 
 0:51: So, I did provide a little bit of background for Ruotbai, but obviously there's gonna be plenty that you can, dive into a little more. 
 0:58: Is there anybody else joining the interview this afternoon, Ian? 
 1:01: Yeah, there's somebody else turning. 
 1:04: There's nobody else joining. 
 1:05: OK, OK. 
 1:07: And Rufik, do you have a hard stop? 
 1:09: I always ask that question. 
 1:12: Do you have a hard stop at 3? 
 1:15: No, no. 
 1:16: Group, no, OK, so I did carve out an hour. 
 1:19: I don't know if it's gonna take that time. 
 1:21: I know when we originally talked to, we're thinking it might be 45 minutes to an hour. 
 1:25: So I always carve out. 
 1:26: I always figure, worst case scenario, we can give you a little bit of time back that nobody knows you have. 
 1:30: So, I'll turn it over to you, I, and I'm gonna go ahead and drop. 
 1:34: I'll circle back with you as well. 
 1:35: And then Rupe, if you just wanna, circle back with Bob and I when you're done, that would be great. 
 1:41: Yeah. 
 1:42: OK. 
 1:43: Sounds good. 
 1:43: Thanks, guys. 
 1:44: Bye-bye. 
 1:48: How's it going? 
 1:49: it's good. 
 1:50: How are you? 
 1:52: pretty good, pretty good, yeah, I work, with the data landing zone operations team, as the product owner, and we are pretty much, we pretty much handle all the ingestion into the lakehouse, so everything into raw landing with, into the bronze layer and then also the administration of the platform itself. 
 2:15: So to me that's definitely the easier part, the administration. 
 2:19: so we handle administration for all the other product teams that do, create silver and gold tables. 
 2:24: We don't create any silver and gold tables. 
 2:26: We don't do any reporting whatsoever, so it's just the data ingestion, handling the platform and also the administering the airflow platform. 
 2:37: And we're also responsible for the the repo for all the teams that write pipelines or create pipelines. 
 2:45: OK. 
 2:47: So, did you want to tell me a little about yourself, or, yeah, sure, see, like, basically with this side this side, like I have around, like, 12 years of experience like as a Python AI and I'm a platform engineer, like primary focus on like the Python software engineering, data engineering, and, like cloud platforms and the workloads and, like, like, I work for like the vision, where like my work is focused heavily on like Python. 
 3:15: And data breaks, S2, airflow, Azure, and the terracom and like a big part of like my role basically is building the reusable components and metadata-driven, like data pipelines like rather than creating one of pipelines for the individual sources. 
 3:33: For example, like, like I have worked on a framework like where metadata define the source target, schema load type and the, we can say, processing rules. 
 3:44: Like, while reusable Python components handle the injections, validations, transformations, and orchestrations, and also like we use airflow for the workflow management and data breaks and the pipe spar like for the distributed processing and apart from that I'm also involved in the troubleshooting, performance optimization, CICD like infrastructures automations and working with the different engineering teams. 
 4:11: So that's pretty much about me. 
 4:14: Nice, yeah, that's a lot of what we do as well. 
 4:18: it's all metadata driven. 
 4:20: everything is broken down into components like, so almost all the product teams are writing Spark in, in notebooks and things except for my team. 
 4:29: So my team is largely doing ingestion and we're, we're not really manipulating the data much. 
 4:33: Pretty much all our stuff's Python, whereas most people, within the company are probably Spark or Spark SQL. 
 4:40: So we're a sequel of Python almost entirely Python. 
 4:44: is your experience more, functional or object oriented? 
 4:48: see, like, I work on both, like, basically, like, in my current role, like I use Python to build the reusable classes, client utilities, and like I work like, as I told you, both function and object programming. 
 5:03: but like for the kind of reusable injection framework like I've been, like I lean more towards the object oriented design, for example, we create reusable classes and components for things like source connections, injection strategies, validations, file processing, and error handling. 
 5:20: Then like the metadata or like the configuration determines which components or strategies get like. 
 5:27: Executed and also like I do use functional components where they make sense like especially for the data transformation and keeping smaller functions clean and detestable. 
 5:39: Yeah, we're, we're pretty much the same boat like, it's almost all object oriented. 
 5:44: There's some functional whereas the teams that are doing the silver and gold notebooks, they're like almost they're all functional. 
 5:49: There's nothing, they're not a single class that works for those types of things, but yeah, we're largely, class-based, reusable components and things like that. 
 6:00: so, I'm guessing it's like the, the code that was back at GitHub where you worked before, or how was, how do you guys have like a shared repos and how did that work with the, pipelines? 
 6:11: yeah, like, basically, absolutely we use GitHub like as, the current rapport or like for our code and all of our like the pipeline injection framework or the airflow DC configuration files and infrastructure are like maintained into in GitHub. 
 6:25: And like we followed the standard branching strategies like typically the feature branch like with the full request into the main or the dev branch and before like merging we have the code reviews and the automated CI checks for things like the unit test lining formatting and something like security or the quality scans. 
 6:47: Nice, yeah, I'm really enjoying the DS codes, extensions or that type of stuff. 
 6:53: It's life's pretty easy, so yeah, like you said, we, we use GitHub as the like people repo for all the code. 
 7:00: it's largely object oriented, but really on the team it's what the person wants to do is no one's required to do one or the other. 
 7:07: It's just we, we tend to do object oriented for the a lot of our code for, are usable, components and things like that. 
 7:15: I'm trying to think of what else, so I do have a list of questions, but I feel like they would be far too easy, You know, so, so you say you worked with a distributed compute as well, but you've been in situations where, like things are running unnecessarily slow and you had to figure out why and like what were the causes of distributed compute not working like you expected. 
 7:37: Oh yeah, like, like the same situation like I got like I, I have had a situation like where the our data breaks or the passpar workload was are taking much longer than expected and. 
 7:49: The first thing I do is look at the spark execution plan and also the actual job behavior or like just rather than immediately increasing the cluster size. 
 7:58: Like for example, like I have seen the performance issues caused by the large shuffles or like the unnecessary data movement or the poor partitioning or the we can say the transformations that were not being handled efficiently. 
 8:11: So like I will look the. 
 8:13: At the Spark UI to identify like the way the time is being spent and check the stages and the task distributions and then like review the code and the data volumes and depending on like what I find like I might reduce unnecessary columns early, filter the data sooner, also adjust partitioning, avoid the unnecessary stuff also just change the way two joints are being handled. 
 8:39: Apart from that, I, I will also look at the cluster configurations and the workload side because sometimes the problem is compute configuration rather than just code itself. 
 8:49: So for me, the goal is like not just to make the job faster but like to understand why it is was like slow and fix underlying issues like while keeping the compute cost under control. 
 9:04: Yeah, that makes a lot of sense. 
 9:05: I've run into that a lot too, where, you know, sometimes it's just the data skewed, and you know there's not a lot we can do like it's especially for the company I work for, because the, the data is almost all one state. 
 9:16: So if state is something is, you know, like, it'll skew heavily on state, that's just something that happens, you know, But yeah, and, and I, I think a lot of the reasons that things slow down or run into is unnecessary shuffles. 
 9:30: There's a certain amount of shuffles that are going to happen no matter what based on what you're trying to accomplish, but yeah, that's something I found as well is that I'll look through and if I can see the shuffling happening, it doesn't need to, that's usually like the easiest to find for me. 
 9:43: But Oh yeah, so you said it's all. 
 9:48: Do you have much experience with the Azure? 
 9:49: I saw you had AWS. 
 9:51: I know bricks, data bricks, but, do you spent much time with Azure and bricks? 
 9:55: I, I, I, I do have like Azure as well and also my background is AWS Azure and GCP also like, but in the current work like I hands-on exposure to the Azure data platforms, like, for the type of environment like, you're describing our work. 
 10:12: With concepts around Azure data lake storage, gen 2, blob storage or the Azure-based data platforms and the, our data break, bricks running in Azures, and I like working with the storage and the, data processing side like along with the application and the infrastructure like pieces around it and, also I would not say like Azure is the only cloud I have worked with like, I, I was already told you like AW is also the part of my background. 
 10:40: But like, like I'm comfortable moving with the cloud environments because the concept, like the core concepts are like similar like the storage, compute, networking, and the access management and the infrastructure at school. 
 10:54: Yeah, absolutely, and I've done AWBS and Azure, and to me I feel like Azure is a little easier too. 
 11:01: It's definitely not hard to switch between them for data bricks and a lot of the, the storage, you know, like, you know, they all have their equivalent, you know, object storage and stuff like that, so it's definitely not difficult to switch between one and the other, so I know for this job we're not necessarily going deep into the spark side of things, it's helpful, but have you ever looked into like, like transaction logs and delta tables and, And is it like any benefit over just straight up folders or? 
 11:34: Oh yeah, like, I have like worked with the data tables and the transaction, log side of like the, data bricks lake house, like, especially, around like how Delta provides reliable table management on like, top of the cloud object storage and Also, like, I've used Delta concepts like for things like schema management, incremental processing, append versus override patterns, and also the maintaining reliable data pipelines and, let's see, when troubleshooting, I'm also comfortable looking at the delta transactions history, like to understand like what the operations have like happened on the table, especially like when we are investigating unexpected changes of the pipeline-like behavior. 
 12:21: Yeah, and also within the Delta log, you know, you get your cable versions and things like that and you know, have you ever used things like vacuum or optimize? 
 12:32: And you know look at the log after that or yeah, yeah, like, basically I work like with the both optimize and vacuum like mainly for the data platform and the maintenance perspective like with optimize like the main thing I look at this is like how the underlying files are laid out and if a data table has accumulated a lot of small files like that can create unnecessary overhead during the leads and Basically, optimize can compact those files and improve the query performance, especially for like we can say, frequently access tables and on the other side like with vacuum, like I'm more carefully because it's related to the cleaning, cleaning up the old data files that are like no longer required and I, I made sure like we understand the table's retention requirements and, anytime, the time travel or the re recovery expectations before like running it? 
 13:31: Yeah, no, absolutely, I just recently had to restore a table and I was really worried that the retention policy was going to be 7 days because it had been like 8 days and it turns out that it had been switched to 30, so I got lucky in that I was able to restore it and everything was fine, but yeah, they're across the company here they're about 30 days for almost all tables, so that's a pretty good window. 
 13:53: So if something goes wrong we can restore. 
 13:56: I would hate to have a 7 day. 
 13:58: That's pretty long too, but I mean. 
 14:02: Yeah, so I do want to go over a few other questions, So you already mentioned the small file, the small file problem that was one of the. 
 14:16: what's that, OK, basically, like, I, I like, basically the small file problem is, definitely something I have like deals with it. 
 14:25: Like it can happen when pipelines like write data frequently in small batches or like we can say when there are like too many partitions and each right creates a lot of small files like. 
 14:38: The issue is not necessarily the amount of data, it's the number of files this path has like to manage and read. 
 14:44: And like when I see that, I will look at the file size like partitioning right frequency, and the execution plans. 
 14:52: So to understand like what's causing it, dependency, like depending on workload, we can use like optimized to like the compact files like, but like I also prefer the addressing the root cause so we are like not. 
 15:06: Constantly fixing the same problem. 
 15:08: For example, we can say if the pipeline is over partitioning the data or like writing too frequent, like too frequently, we can just adjust the right strategy of the partition designs. 
 15:20: So that way we improve both like the query performance and the storage efficiency rather than treating optimized as the permanent workaround. 
 15:29: Yeah, absolutely. 
 15:31: I did have another question that came up. 
 15:32: You mentioned before something about incremental processing. 
 15:36: So, what kinds of, I guess pipeline processing are you familiar with that, has like a more efficient process as far as CDC and things like that? 
 15:47: for the, like, I worked with like a few incremental processing patterns, and generally the main goal is always to avoid the reprocessing the entire data set when only a like portion has changed. 
 15:59: For example, in my like recent project like in a metadata deization framework, like we can define the load behavior in the metadata and like whether like it's a full load, incremental load, or app or just override for for incremental processing. 
 16:14: We typically use some things like reliable time stamps, watermark, or the source site changes indicate indicator or like to identify like what's a new or the change since the like the previous successful runs and then like the pipeline reads like only that portion of the source data processes it like through data breaks or file spark and then like write it into the appropriate data table. 
 16:43: We also make sure the process is like restartable and the item potent so if the job fails and we rerun it, we don't accidentally duplicate the same reports and also I have found that the biggest improvement usually comes from combining the right incremental strategy like with. 
 17:05: good, partitioning and avoid unnecessary scans or the suckers and also like I work with several types of platforms. 
 17:12: we can say for, the incremental processing, I primarily use watermark or the high watermark patterns. 
 17:19: Like we might use the last updated time stamp or an independent we can say an increasing ID to identify the reports that changed since the previous successful runs and we stored that watermark in metadata and the next pipeline pick up select from that pointer rather than scanning the entire source again. 
 17:41: Yeah, and that's primarily at Health Partners how we do it. 
 17:44: It's, it's largely watermarked and sort of metadata tables. 
 17:48: So for the most part, and that's something you mentioned about item potent, that to me that's a big one. 
 17:53: Whenever I'm writing code for a pipeline, like I don't write code anymore for pipelines, but when I did, like it was like item potent is such an important thing that for some reason it fails or something goes wrong, you should just be able to like go again and everything would be just fine like. 
 18:07: It shouldn't need a special, like a special effort to get it reset or anything like that, especially, you know, I mean you could just code it up to easily, you know, be out of both, yeah, but yeah. 
 18:19: Totally agree with you. 
 18:21: Yeah, and I feel like there's also the, have you ever worked with the change data feed data works? 
 18:27: Oh yeah, like, basically in this, like, like I have some hands-on experience like with the data change or the data feed or we can say also the CDF like I have used it in scenarios. 
 18:39: We are we needed to identity identify the changes to our delta table rather than repeatedly scanning the entire data sets. 
 18:47: So the nice thing about the CDF is that it gives you the row level changes such as the inserts, updates, and the deletes along with the commit information. 
 18:59: So generally this can be useful for the incremental downstream processing because you. 
 19:05: Can like consume only what changed between specific versions or like points in time, for example, like instead of reading an entire like every time like table every time a downstream process can read the changes like since the last successfully processed versions and apply those changes to its target. 
 19:24: So that fits nicely with the watermark and ident important processing patterns like we are just discussing. 
 19:31: And I had like to still evaluate whether the CDF is the right approach like for for like a particular source and the workload, but conceptually I'm comfortable with how it fits into the delta-based incremental architecture. 
 19:49: Yeah, I'm not entirely sure why why more people don't use it. 
 19:52: I've written it a few times, but it's still not widely used, I don't think. 
 19:57: Like you get a like so the CDF you get the the inserts updates, the pre-imposed image, and the deletes, and to me that's perfect. 
 20:05: You have like everything you need to incrementally process things. 
 20:08: I agree, but it's, I think the part of it is that teams often already have an established watermark or the time stamp based incremental pattern. 
 20:19: So introducing CDF can feel like changing something that already works. 
 20:25: Yeah, yeah, and I think conceptually it's just a lot easier to just use a watermark. 
 20:31: And I don't know, but like I, I've written a few pipelines where I, you know, all the things that were updates got merged and all inserts got inserted, and a lot of the time it was just inserts, and it just, it was, I don't know, it was, it's, it was more complex, but it was much more efficient. 
 20:46: Totally agree, totally agree with you. 
 20:51: I had, so have you, have you had situations where you, you had to write your error handling in your pipelines and you decide, you know, sometimes, you know, it should crash because of what happened. 
 20:59: Other times you should retry. 
 21:01: Is there like a, is there a good indicator for you for like why something should retry? 
 21:08: Oh, absolutely, I think error handling is really important in the injection pipings because Not every error should be treated the same way. 
 21:16: Like, like if I get a temporary connection issue or timeout or some like other transient infrastructure problems, I agree like want the pipeline to retry automatically with the appropriate logins, and there is like no reason to fail the the entire workflow because like a service was like temporarily unavailable, but like. 
 21:38: If I get something more fundamentals like the unexpected schema changes or like we can say invalid configurations or corrupted input or we can say a data quality issue, so that would make the downstream data like unreliable or I'd rather fail. 
 21:56: The pipeline clearly so that's the surface problem that quickly continue and also if the reusable Python frameworks like I worked with, I typically separate the expected or recoverable like exceptions from non recoverable ones and Also, use the structured logging and make sure the airflow task gets the correct success or the failure status. 
 22:23: OK, that brings up something else and made me think of. 
 22:27: I mean, have you ever, so the DLZO team, they write a lot of the code for injection, but a lot of reusable code for other teams too, because most of the other teams are functional programmers. 
 22:39: So have you ever, had to develop libraries, for like a whole for company, and, and how did you manage, if so, like the versioning of any of the like shared code. 
 22:52: like, I have worked on shared usable Python components and libraries rather than like having everything build, build the same functionality, independently like. 
 23:02: in my current work, like we have built a common components around the things like the, data injections, configuration handling, validations, APR or the source connectivity, or also the exception handling and some like other utilities. 
 23:17: So the idea is that like an individual pipeline or a team can consume those components like instead of rewriting the same logic. 
 23:26: so for example, like with the metadata-driven injection framework. 
 23:30: the core Python library handles the common behavior while the individual pipeline mainly provides the metadata and the source specific configuration, so that keeps the business of the pipeline specific code relatively small and also like when building something like intended like for the multiple teams, I pay like particular attention to like clean interfaces, also the backward compatibility testing. 
 23:58: the documentation versioning. 
 24:00: So, also, want the library to be easy to consume like. 
 24:06: Without requiring every developer to understand the internal implementation, so yes, like the kind of, platform as a library approach is something that I really enjoy and like from what you are describing, it sounds very like aligned like with the how like like the Dezo teams operates. 
 24:25: Yeah, no, it definitely does, there's something else too, oh, you had mentioned like metadata driven, so we're metadata driven, but it's, it's unfortunately it's metadata is stored in SQL Server. 
 24:37: We sort of inherited that and the people that stood the platform up and we're transitioning over to YAL for everything, and that's largely to do with just, I don't know, separation of concerns with what people need to do, but also there's a lot of compute we pay for by having airflow constantly pinging our SQL Server. 
 24:55: And we could remove a lot of costs associated with that. 
 24:58: What kind of metadata infrastructure have you worked with? 
 25:02: like the kind of, the metadata, infrastructure like in my experience, like I worked with metadata stored in the relational databases as well as a configuration-based metadata, like depending on the use case like. 
 25:18: database driven metadata like I have worked with the SQL-based configurations where the things like the source details, the target locations, the schemas, load types, or the watermarks, and the processing rules are like stored centrally. 
 25:34: So the Python framework reads that the metadata and use it to determine how the injections should behave. 
 25:41: And apart from that, like I have also worked with like the more configurations are driven like approaches where like the metadata can like maintain the alongside the core and manage to the GitHub and the CICBs and also I like that approach when the metadata is relatively static because You get the version history, PR, reviews, validations, and the like the control, promotions between them and, from like an architecture perspective. 
 26:11: I had probably separate the two concepts operational state like the current watermark or the last successful runs and may still like make sense in our database and while like pipeline definitions and the configurations can like live nicely in Yamil or or or we can say it. 
 26:30: Yeah, no, it's good. 
 26:33: I've, I've done both as well or multiple kinds of infrastructure, so I'm looking forward to getting off of SQL Server, yeah, there was something else. 
 26:43: Oh yeah, so, I made me think of GitHub, but, with GitHub, so we promote to pretty much directly to Maine like it goes to staging, but just to. 
 26:55: Say that it can technically run like, you know, so after there's a full review, there's like a full review, multiple people check things out and then it goes into staging just to see if it can function in staging for like, you know, a minute like it's real fast and then if it can, it doesn't, if it doesn't crash in staging, it goes right to me, which is not how a lot of people do it, So what is your experience with promoting code, in your history? 
 27:21: like from my experience, like, generally it is a little different from having the separate long-lived development of QA and the production branches, but, if you have a strong, PR reviews, automated checks, and, staging validation, it can work well. 
 27:36: Like, in my experience, like I worked with the Gita-based CICD workflows. 
 27:40: We are the, changes go through a feature branch and the PR, then, automated testing and the validation run before the changes like merge and like for the infrastructure and the deployment related changes I've also worked with the terraform and the data of actions so we can try to keep those changes version control and reproduceroducible rather than making manual changes and. 
 28:05: one more thing, like for shared Python library libraries, I'm particularly careful about, regression testing because one change like can affect multiple pipelines. 
 28:16: I like having the staging validation, cache integration issues. 
 28:19: I like the PR review catches, design, maintainability, and the compatibility concerns. 
 28:25: So I'm comfortable at, adapting to, the different, bit of workflow. 
 28:31: The exact branching model is like less important to me than having the good controls around review, testing, and like the safe promotion. 
 28:42: Yeah, and, and like we have really good, you know, overviews and things like that, but you mentioned testing as well, so where I come from, prior to here you would have automated testing and then go into staging and then production, you know, there is no automated testing here. 
 29:00: There's none. 
 29:01: OK. 
 29:01: It just doesn't exist is. 
 29:04: Like code review only, absolutely like I worked with that model as well. 
 29:09: Like I think the code review and like the, automated testing of like the two are different purposes like code review. 
 29:18: Give us the human perspective on architectures like maintainability, security, and whether the implementation makes sense and automated test gives the repetitory validations every time like something changes like, yeah. 
 29:35: Yeah, I know that's good to know, So I, I did, I want to ask if you have any questions for me about the team or anything that we do. 
 29:45: yeah, like I have a couple of questions like, since you mentioned that the transitions from, SQL server metadata towards the YAL, like I had interested in understanding like how far along that the migration is and, whether the person is this role would be expected to help design that the new metadata approach. 
 30:07: they, they could help, but it's, the, it's been designed and it's been tested, and we're at a point now where we're getting ready to implement. 
 30:17: so it's pretty close, but everything right now is on SQL Server still, but yeah, it's, it's designed, and it's, it's really we're just trying to get a few other things in place before we, get that because right now we're, we're currently using synapse, Azure synapse. 
 30:35: And we're trying to move off of it. 
 30:37: there's a lot of problems we're having, we've always had with it. 
 30:39: And so once we move off of synapse, then we're going to, focus on the metadata layer moving completely off SQL Server. 
 30:47: Yeah, that makes sense. 
 30:48: So like it sounds like the architecture and design are like already in the pretty mature state and the next phase is just like, really implementation and migrations rather than the figuring out the whole approach from scratch. 
 31:02: Yeah Yep, and the, the, the teams like tech lead actually came up with it and tested it, got it all ready. 
 31:11: There's, you know, 5 people on the team, and there's, just everyone's at the same level engineer, and then there's 1 tech lead. 
 31:17: The tech lead's really, really good. 
 31:19: Like I have yet to stump him on anything. 
 31:22: I don't know. 
 31:22: He just must not sleep or something. 
 31:24: He seems to know it all, but, that's the size of the team, and those are the big changes that we're getting ready to do. 
 31:30: The person that left who we were trying to fill a spot for, they, everyone does everything, but that person also had an interest in GitHub actions, terraform. 
 31:39: We currently don't have anybody on the team that has experience with either of those things. 
 31:44: Person doesn't have to have that, but we currently don't have any. 
 31:47: We don't have a whole lot of GitHub actions right now, but we were just getting into it in 2026, so I don't know if you have much experience with GitHub actions or. 
 31:59: that's actually lines up very well with my, the background. 
 32:02: Like I worked with both the guit actions and the telecom, particularly around the CICB and the infrastructure automation. 
 32:10: Yes. 
 32:12: And like I said, we currently had stopped all development on that because the person who did that, left. 
 32:17: So we're using what we currently, what we had before as far as everything's still in place that we're using before it did have actions in terraform, but we haven't started any, new work. 
 32:27: and I guess I should trans transition to like to explain how the team does work. 
 32:32: So, the, the team basically there's 5 people and there's a series of stories and the person, the engineers, they just, they pick the story that interests them, that's what they work on. 
 32:46: and there's usually, I don't know, 10 to 15 stories that are out there, and then every 2.5 months they have to do on call, which means just taking care of, like, operation support like just one-offs like this broke that broke from people. 
 33:04: It's real usually fast, quick things, but that's a realistic thing, so. 
 33:10: You know, every, it's about 2.5 months somebody has to spend 2 weeks of, operation support and then they go back to just picking stories. 
 33:19: Like I said, people pick the stories, they can also create their own stories if they have good ideas for things, but, if they don't want to, they can just pick the existing. 
0:00: That gives people a lot of ownerships while still making sure the important platforms like works get covered. 
 0:08: Yeah, the only downfall is then you can get somebody that's focused on like GitHub actions or terraform and no one else is because that one person, if they keep picking up those stories, then you just have one person that's got experience. 
 0:20: But then at the same time that's just how it works. 
 0:22: It seems like everyone just seems to have the things they like and you know which stories people are going to pick up. 
 0:30: Oh yeah, like see. 
 0:32: basically, I actually like that, like it sounds like. 
 0:36: People naturally develop areas that are interested in, but they are like still enough flexibility that everyone can contribute across the platform. 
 0:44: For me, like I had probably gravitate towards the Python framework, metadata-driven ingestion, data actions and the stories because those are the areas where I can bring some experience right away and but I also be comfortable like picking up their stories with the teams need help. 
 1:05: Yeah, well, that's good to know. 
 1:09: that is all the questions I had too. 
 1:11: I know it's like really early still, but, I feel like we went through like a lot. 
 1:18: Yeah, and, I have also, one question, like, apart from this one, is there any other for the like the other other round, in the future? 
 1:29: well, what's that, is there other interviews? 
 1:33: Oh yeah, so at most there's one more, but that's it like, it's either stops here or one more, and so I, I give you a message too to expect which one it is. 
 1:44: I mean it's really, it's up to other people like typically there's also like an HR person in these things. 
 1:51: I usually sit around and don't actually talk, but so there might be another one with like an HR type person, like a non-technical. 
 2:01: OK, sure. 
 2:04: Cool. 
 2:05: That is all I had though. 
 2:07: if you have anything else. 
 2:08: yeah, no, man, thanks, and I really enjoyed the conversations and I like feel we covered a lot of areas that are, important to this role. 
 2:18: Yeah, definitely recovered your time. 
 2:19: I'm gonna go report to the tech lead now and yeah, thank you. 
 2:23: I know that it went pretty well. 
 2:24: All right, thank you. 
 2:26: Bye bye bye. 
