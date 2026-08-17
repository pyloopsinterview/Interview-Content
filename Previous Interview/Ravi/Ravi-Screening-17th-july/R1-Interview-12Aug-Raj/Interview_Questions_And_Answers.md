0:00: Yeah, I can hear you. 
 0:01: I'm I audible to you? 
 0:03: Yeah, your voice is not like. 
 0:07: it's coming as if you're talking like from far behind, but yeah, it's good. 
 0:13: It is a little better. 
 0:15: OK. 
 0:19: now, Yeah. 
 0:22: Mhm. 
 0:26: So, Ravi, we have, Rovidas who will be joining this, interview, like who will be taking this interview. 
 0:36: Well, let me just quickly check with him. 
 0:38: Mhm. 
 0:41: Yeah. 
 0:45: OK. 
 0:47: so do you mind if I go back and check with him and just give him a quick call? 
 0:52: OK. 
 0:53: Thanks. 
 1:04: Circle Kleba to you rate 140 to 150. 
 1:12: So where are you based out of Ravi? 
 1:14: I'm in Maryland. 
 1:16: Maryland. 
 1:17: OK. 
 1:26: OK, we have it with us. 
 1:27: Hi. 
 1:29: hello. 
 1:32: Yeah, thank you for joining. 
 1:33: I will just drop now. 
 1:35: Let me just make sure that the video is recording will start. 
 1:41: Let's get you over here. 
 1:49: OK, we are good to go, so I'll just drop it. 
 1:54: Hey, hi Ravi. 
 1:55: How are you? 
 1:55: Oh, I'm good. 
 1:56: How are you? 
 1:58: I'm doing good too. 
 1:59: So, if you don't mind, if you can quickly give me like a walkthrough of your profile, and I don't mean like, you know, go into very much detail, but like, like things you think you're proud of, and then we'll go from there, OK? 
 2:11: Sure, sure. 
 2:12: So like, As you know, my name is Ravi Kumar. 
 2:14: Like, I have 12 years of experience in data engineering, Python development, AIML, and the cloud technologies, and like I have like worked, like across the insurance, healthcare, and the, retail building enterprise data platforms, large scale ETL and ELD pipelines, and I like AI ready data solutions and currently like I'm working as a senior AI data engineer like with Mutual of Omaha and like I'm working like on an enterprise insurance data platform that brings the like together data from from source like the guidewa Policy Center and the claim center or like less skill servers, less APIs S3 and the like external partner. 
 2:59: Feeds and my core technologies are like Python, Fire Spark, SQL, Snowflakes, data breaks, AWS, and also like I have built pipelines for like injections, data cleansing, standardizations, duplications, incremental processing, and, like we use airflow like for, orchestration, scheduling, monitoring, and like the snowflake for like other trusted area. 
 3:23: So that's pretty much all me. 
 3:27: OK, cool. 
 3:28: So let's talk about Snowflake then, I guess. 
 3:31: maybe just give me like, you know, a brief, about what was the use case, right? 
 3:37: And, where did you use snowflake and or were you, you know, involved in the decision, to choose Snowflake, right? 
 3:46: And, basically what impact did it have, right? 
 3:52: More more legal systems. 
 3:53: Sure, like, talking toward in my current project of like Mutual of Omaha, like we use the Snowflake primarily as a like a trusted enterprise data layer like after the injections and the transformation processes and like the use case like was to bring that together insurance data like as I told you earlier like the multiple sources like the guideway policy centers and the claim centers or oracle SQL servers API and the industry. 
 4:20: And basically the data was like coming in the different formats and schema, so like we needed a scalable platform like where we could standardize and model like that the data for like analytics reporting and like also use the AI use cases and, here, like, generally my role was mainly around the building the Python and the pipelines like that performed the, like, cleansing, business rules, validations, and incremental processing. 
 4:49: And once like the data was transformed, like we loaded the trusted data sets into Snowflake and build structured models around like entities, like policy, member, claim coverage and the billing. 
 5:03: And after that like we choose Snowflake because it give us like the scalability, strong SQQL capabilities, separations of like compute and storage and the good integrations like with how the cloud-based data ecosystems and like it also made it easier for like the different consumers and our data science and the AI applications. 
 5:29: OK, so I guess you briefly touched upon it, right, but let's say, what was the cloud platform which you were using, under the woods for Snowflake? 
 5:39: Mhm, generally for like cloud we use AWS, like we use AWS services along with the Snowflake and Dablakes as like part of like the overall data platform. 
 5:50: OK, so let's say, you are designing a data solution, right, and you have two choices basically. 
 5:58: So you have your data music ecosystem, right, where you can have data lake in whatever databases, and you know, you have to do right and all that is there, right, versus, there is a choice of using Snowflake, right? 
 6:12: So what are the factors you would consider or what, what would make you choose, you know, Snowflake or the existing ecosystem. 
 6:20: Yeah, like, absolutely, basically, I would not choose the snowflake just because it's like a popular technology like, I would like first look at the workload data volume. 
 6:33: Performance requirements and like how the data is going to be consumed, for example, like in our current environment like we had data coming from like the multiple operational systems and we need a centralized analytical layer like that could handle the large volumes like without putting the additional load on those four systems so that that's why like the snowflake like made sense for us. 
 6:57: So the main factors like I would consider are like the workload isolation. 
 7:02: performance integrations and the operations over overhead like so snowflakes like separations of compute and storage like useful because we can like scale compute independently based on workload and we can like also have the different workloads like a data science reporting and the AI related processing. 
 7:23: So, without everything competing for like the same computer resources and, another factor is like SQL and the data engineering like productivity, like, basically our team like already work heavily with the SQL Python and the Spark, so like, Snowflakes, like, it fits naturally in this ecosystem. 
 7:43: So it also, like integrates well with the cloud storage like S3 and the tools such as like the Airflow and the data. 
 7:53: OK, do you have exposure to, say, pipe and smoke pipe steaming or pipe like whatever exposure you have maybe we can talk about that. 
 8:03: Mhm, yeah, like, basically I have like exposure in a snow pipe, like particularly for like the real-time or the continuous data injections in the snowflake, and, like, in our data platform, like the typical pattern was to like land, like incoming files in Amazon S3 and the snow pipe like could. 
 8:22: continuously detect new files and load them like into the snowflake tables like without waiting for the large batch processing. 
 8:31: OK, I see a lot of Python mentioned everywhere 2016, 2018, 2018 to 2021. 
 8:41: Maybe just talk about like, you know, what are the typical issues, you would address using Python and any, any peculiar issues you came across, right, which was not like, you know, straightforward thing and you have to come up with. 
 8:58: yes, like, like I have used Python, throughout my other data engineering projects like mainly for the data injections, transformations, validation, and the AP. 
 9:09: And like a typical example like would be an like injection pipeline where data comes from an API or databases or like the X-3 files. 
 9:19: So generally I use Python to handle the connection, schema validation and the data, like duplications, error handling, and like, and then pass the data like into this patch pack or the snowflake depending on the workload. 
 9:35: And I remember like one issues like I've encountered that was like a little more challenging was inconsistent source data. 
 9:46: Like for example, like the same business field like could come like with different formats like from different source systems so dates in different formats, unexpected notes, duplicate records, or like, we can say like even a column changing from like numeric to string so. 
 10:03: Instead of like allowing the pipeline to fail completely, we built the python-based validation and the exception handling like. 
 10:12: Around those cases, so we would quarantine or log log the bad records, alert the team, and then continue processing the valid data like where like appropriate and, after that, like, in one of my projects like issue was like the performance with the large data sets like early on using the standard Python or Pandas like for like very like. 
 10:37: We can say very large data sets will like become more intensive so we address that by moving the heavy pro processing to fire path using partitioning and the distributed processing like by keeping Python for like orchestrations and the business logic. 
 10:57: OK. 
 10:58: And where were you hosting the Python? 
 11:00: What was your execution moment? 
 11:02: Mhm. 
 11:02: generally, like, I've used data bricks like primarily rein in the data bricks using the like the spark cluster for the distributed, processing, and, for orchestrations airflow like manage the pattern is DAX and the trigger the different, processing jobs. 
 11:20: OK you're tying it back now, so, if you are given a choice between data breaks and snowflake, what things would you consider and, you know, what factors would push you towards snowflake or toward data breaks. 
 11:35: Like, basically, I first looked at the workload, same here, like and the type of the processing because, data breaks and snowflakes like overlap but they are optimized somewhat like differently. 
 11:46: For example, like, if the requirements is primarily SL analytics, BI reporting structured, and we can say you can't see any structured data like the high concurrency analytical workload, like I generally lean towards the snowflake like because. 
 12:02: It gives like a like a strong manage like warehouse experience like the we can say strong manager like like the storage and the strong governments and Relatively low operations overhead and on the other hand, like if the requirement involves the large scale data engineering, complex transformations, Spark or like workloads, machine learning, or we can say like the unstructured data, then I will go to go with the data breaks because the Spark ecosystem is like primarily useful when we need the distributed Python PySpark processing or like the ML workflow. 
 12:43: OK, so I think, I see you have been, an AIML data engineer, yeah, yeah, right, so I would like to understand what it means. 
 12:55: I may follow up I guess, yeah, like, basically like I would describe an AML data engineer as Someone who sits between the traditional data engineering and the AIML application. 
 13:08: So basically in my current role, like my responsibility is like not just to move data from like one system to another, like, like I make sure the data is reliable, clean, well structured, contextual, and like available in the way that the AI and ML systems can like actually use. 
 13:27: for example, like, in Mutual of Omaha, like we have policy, member claims provider and coverage data like, coming from the, like the different, different systems. 
 13:37: So like I worked the, on the Python 55 pipelines that ingest, validate, and standardize the deduplicate and incrementally process the data and then like publish trusted data, data set into the snowflake. 
 13:53: And like the AIML parts come in like when we prepare that trusted data for like things like the machine learning models, rag applications, so when you say data like what does it mean? 
 14:06: What do you do to make sure that it is can you please come again. 
 14:10: No, so you, you say that you prepare the data for AIML, right? 
 14:13: So what I'm trying to understand is like what goes in that preparation, like what are the things you do, right, to make sure that the data is ready for AIML, models or engine, agents. 
 14:24: Like the things like first is the data quality, like, I evaluate the schema, handle the missing or the invalid, values. 
 14:34: remove the duplicates and apply the business rule. 
 14:36: Like, for example, like with business, with like the claims data, like, like I'd make sure the claim amount, policy IDs, member IDs, dates, and like the relationships are like valid. 
 14:48: And after that, the standardizations and the integration like since like our data is like comes from guide databases, APIs and the S3 the same business entity can look different across systems so we like to standardize those formats and create a consistent representations and, after that, the creating the right business context, like, we don't give the, like give the AI individual tables like we establish relationships like such as a member and policies, then we go to the claim provider and the coverage. 
 15:21: So this makes like the makes the information like much more meaningful like for the AI applications and also in last like for an LLM or the rag use cases we then look at the things like chunking the relevant documents or records. 
 15:37: generating the embeddings, storing those like embeddings in vector search systems and I think the metadata so we can revive the like right information like based on the user's questions. 
 15:51: OK. 
 15:54: so talk about your exposure to data breaks. 
 15:57: you mentioned you primarily did that on like primarily did Pythonon data breaks. 
 16:02: So what was the use case and, what kind of pipelines were you building? 
 16:07: like my exposure, like we primarily use data breaks as a, we can say data processing and the transformation layer. 
 16:15: like, especially when the data volume was like large enough and the standard Python or the pandas was not practical, then the typical like, can you quantify it, sorry, what size which is large enough for data, size like. 
 16:36: talking to our like size, like, when I say the large scale, like I'm talking like roughly 100 millions or like a few like million records like depending on the source like the daily incremental processing is like a, typically in the tends to the hundreds of the like millions of records like while the, we can say historical data sets can go into the like the billions and, from the storage perspective, like we are dealing with the multiple terabytes of the data in the S3 and the Snowflake, so that's like where the data becomes like useful because Processing that volume with the standard Python or the Panda like a single machine would not be practical. 
 17:20: OK, have you worked on a use case where you had this, streaming data coming in and you have to process that, in, in one of our projects, like, like I have experience basically like, like we use Kafka as like a streaming layer, like the data was like consumed by the by a Python like based on the. 
 17:43: processing layer. 
 17:44: So, like here, like we performed the validation schema checks, transformations, and the enrichment and then persisted the process data into the downstream, data platform and, there are some like, few, I remember the few challenges like, like phase like handling the duplicate events, late arriving data, failure, and the maintaining the processing checkpoint so. 
 18:09: We use checkpoints so that if the failed job failed and we could like resume from the appropriate point like rather than the reprocessing everything and we also like monitor consumer lag and like the processing latencies and and we designed the pipeline to be like quite important so that the we're trying and even like would not create duplicate like the business records. 
 18:35: OK, what was the source for you, like, you know, where were you getting this, you know, streaming events from, talking to her like the source. 
 18:45: Like, generally the streaming events were like primarily coming from upstream application services and APIs and like in that use case the application generated business events, things like the transactions and the reports being like created or updated and those events like are published into the GAA topics. 
 19:06: OK. 
 19:09: let's talk about governance now. 
 19:12: So, since you have a lot of experience on smoke, like, I guess we can start there. 
 19:17: So can you talk about like different aspects of governance and how smoke, you know, smoke like ecosystem, how are those taken care of. 
 19:26: Generally, we can say, I looked at the governments across like the maybe several areas rather than just access control. 
 19:35: basically, first, like, first is like saying that access control like we use RBAC rule with access control, so the users and applications get permissions to like the rules rather than the granting the privileges individually and I follow the principle of like least privilege and the separate rule based on like Responsibilities like, such as like data engineering analytics and redoing consumption. 
 20:01: And second is, I guess, data classifications and the sensitive data like for things like PLLL or the sensitive insurance information we identify and classify the data and then apply appropriate controls, snowflake support things like. 
 20:20: tagging and the masking policy, so. 
 20:23: The sensitive volumes can be like masked depending on who like who is accessing them, and after that the row level security like the different users should be different subsets on the same data like we can use like row access policies like to control. 
 20:43: which rules are like visible based on the user's rule or the like, other attributes and, last one is like auditing and monitoring. 
 20:55: OK. 
 20:58: cool. 
 20:59: Let me see what else we got in the mirror. 
 21:05: Any exposure to BI platforms? 
 21:08: like I, I have like the Power BI and also the tablet and OK, what do you do with all the, like, like, particularly our understanding the dashboards consuming dashboards, using the dash query. 
 21:22: These are the things I like, policy volumes, creatings, KPIs, and like the other business like, mattresses and like my online, yes, OK, so, can you give me specifics as to like what was the business case, right, so. 
 21:38: I understand like, you know, generally like these tools are used for these purposes, but like what was your use case right? 
 21:43: Let's say when I'm asking about, Power BI, like what dashboard did you get, right? 
 21:48: What were the KPIs of the generally. 
 21:52: in Mutual of Omaha, like the business wanted a consolidated view of like policy volumes, claim volumes, premium trends, and the related KPIs across the different volumes of like the business and the region. 
 22:05: So the challenge was that the like underlying data was coming from the multiple systems, like, primarily guide along with the databases and the external feeds so that the number was not always directly comparable. 
 22:20: And my role was like to build the support the data layer like behind those dashboards we use like the Python Pilepark for the injections and the transformations, applied the business rules and the like the data quality checks and then. 
 22:36: Created the curated data sets in the snowflake, for example, like. 
 22:41: For a policy volume KPI like we had to make sure like we are, counting the current policies, handling the duplicates, supplying the appropriate effective dates, and joining the policy information like with the relevant customer and the like the product dimensions. 
 23:01: OK. 
 23:03: I think those are the questions that I have for you to be. 
 23:06: Mhm. 
 23:07: Do you have any questions for me? 
 23:09: like, I have some questions like. 
 23:12: Regarding, like, like, first I'd like to understand, what, what are the primary data and the AI platform initiates like other team over the next 6 to 12 months and like what you would expect this person to own initially. 
 23:29: So this person would be playing a guitar architect right so meaning like I think primary architectural decisions and you know leading plan conversation and basically advising the client about like what would be the right tools for their particular space right and Suggesting, defining architecture, making sure that you know that design is implemented properly using data engineers, and then basically building the data points. 
 24:00: That's the summary, yeah, it sounds good. 
 24:04: OK, yeah, anything else, like, apart from this one, is there any other technical wrong? 
 24:11: I'm not sure that I think HIV be able to tell you, so. 
 24:16: OK, cool. 
 24:18: Thanks, man. 
 24:18: Nice talking to you. 
 24:19: I'll see you, man. 
 24:20: I'll see you. 
 24:20: Bye-bye. 
 24:21: Have a good day. 
