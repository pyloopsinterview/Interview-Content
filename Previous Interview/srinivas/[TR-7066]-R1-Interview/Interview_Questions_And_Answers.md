0:00: This little bit up. 
 0:04: Little, take it a little back, sorry. 
 0:09: OK, fine, yeah, be, be like. 
 0:16: Then I took. 
 0:17: To. 
 0:24: I'm saying. 
 0:25: Now, now I'll take your photo. 
 0:33: OK. 
 1:06: Oh, this photo was a long time back, huh. 
 1:11: Like 5 to 6 years back. 
 1:15: When fighting its back. 
 1:18: OK. 
 1:21: From when you, you have the green card, like, at, like I came in the US like in 2014 and like I got green card, got a green card then like through marriage. 
 1:34: I. 
 1:39: look, I think. 
 1:42: So, one second, You want to brace yourself for a minute? 
 1:53: Yeah, sure. 
 1:56: So, like, like talking about myself, so like, I am Savaote and like I have a little over, like over 10 years of experience, and 2 levels of experience, I would say, and like in data engineering and back end development, and my core-exportise is like mainly around like Python and PySpark and I also You use like SQL and data bricks and like deployed like applications to AWS and like currently talking about my my like most current experience I'm working with like TNET Healthcare where like I mainly focused on building and supporting data pipelines for like large healthcare data sets and like I work with like Pike Spark and Data bricks to bring data from like different sources and transform it and validate it and then create reliable data sets for like downstream analytics and applications. 
 2:45: And on the cloud side, like I work with services like S3 and like Glue and you know, like I also use Data League, Spark, SQL and like database workflows and unit unit catalog and apart from that, like, you know, apart from development, I am involved in production support and like performance tuning. 
 3:03: So like I spend, you know, a good amount of time troubleshooting and spark, spark jobs, optimizing queries and like making the pipelines more efficient. 
 3:11: So yeah, like, all I'd say like my friend is taking a complex data problem, breaking it down practically. 
 3:18: I like building something that is reliable and scalable, so yeah, that was all about me. 
 3:25: OK. 
 3:26: Food. 
 3:30: you do. 
 3:33: OK. 
 3:36: So tell me one thing. 
 3:38: You know what is an SCD2? 
 3:40: Sorry. 
 3:41: Acidity, acidity, yeah. 
 3:44: What is it? 
 3:46: OK, so, like, like if I talk about like SCD2, like, I mean, I. 
 3:54: Like, let me put it into words like. 
 3:57: I mean, Like you mentioned, like FCT, right, right? 
 4:05: A CD to. 
 4:06: Sorry, I like your voice is really broken. 
 4:10: S as in Sam, C as in Charlie, D as in David, CD 2 SCD2, right? 
 4:16: Hm, OK. 
 4:18: OK, so, like, like, like I'm talking about like SCD2. 
 4:22: And I, I, I, you know. 
 4:27: I thought I couldn't remember this like like it is this type, SCD2 type, it means like, you know, slowly like changing dimension type 2. 
 4:38: as much as I can remember, yeah, thank you. 
 4:41: Like we use it like when we need, I would say like to maintain the complete history of changes and like, yeah, instead of like overwriting an existing record. 
 4:51: So yeah, this was it. 
 4:56: No. 
 5:00: OK, explain, you, you know, what are the cluster types which are available in data works, yeah. 
 5:08: What else can you name a few give me a use case. 
 5:12: So, like, like talking about the cluster types and data breaks, like, you know, I mean, I would generally like classify the compute options into like all purpose clusters and like job cluster and like skill warehouses, like with the exact terminology and depending on like database sorry. 
 5:30: You have only one screen open, right? 
 5:32: Yeah, yeah, and like with the exact terminology and like depending on the database frozen and like workspace setup and like all purpose clusters are like mainly used for I would say like interactive development and like for example. 
 5:45: Like data engineers can use them, like with the notebooks to develop pipe Spark code or test transformations, or deal with pipelines and like analyze data, and yeah, I mean they can be shared with multiple users, although, you know, access and permissions need to be managed properly. 
 6:03: And like job clusters are like designed for production workloads and like they are created when a job starts and like, you know, can be terminated after the job finishes and I prefer this approach for duty ETL pipelines like you know, because it provides better isolation and like cost control. 
 6:19: So yeah. 
 6:21: What are sequel letters? 
 6:22: Have you played sequel letters? 
 6:25: like, yeah, yeah, I mean, I have worked with it. 
 6:29: What is it So, like SQL layout, like it is, you know, it it is optimized for like SQL queries and like reporting dashboards and like, I would say like BI workloads. 
 6:44: Eric, yeah, I mean, yeah. 
 6:47: That's what Sorry, so, so yousel battles for Python, yeah. 
 6:54: OK, so, so you can, you use for dashboards, creation of dashboards you use. 
 7:02: Yeah, like, I am used for troubleshooting aware of query and like usually, like, you know, to, look at like execution. 
 7:13: See, I'll give you a scenario. 
 7:15: You have an, a data set which is $2 billion.02 billion dollars, in volume which is available in a legacy dataset. 
 7:25: Same way you say it's an oracle or in sequel. 
 7:28: OK. 
 7:30: How do you, bring that to the lyrics. 
 7:34: OK, so, like, like bringing that into data breaks, like in this situation, like, you know, like, I wouldn't try to move the entire like 2 billion records in a single room. 
 7:45: Or rather, like I would approach it incrementally, I would say. 
 7:48: And first, like I would understand the source oracle or like a skill server tables and like identify the primary or like incremental column, usually, you know, something like a time stamp or like increasing ID and like I would determine the data volume and partitioning strategy and like secondly, like, yeah, I mean I would set up the connectivity from the legacy of database to the cloud environment. 
 8:10: And depending on the, you know, architecture, I could use like AWS Blue or like, you know, another ingestion mechanism to extract the data in parallel. 
 8:18: And for the initial load, like data, like I'll break the data into a manageable partitions like data ranges or ID ranges, so like multiple workers can process it, you know, concurrently. 
 8:30: And like 3, I would land the raw data in like S3. 
 8:35: And you know, then use data breaks with Spike Spark to transform and like validate it like right into the data leak. 
 8:42: yeah, I would also use partitioning appropriately and like so we don't scan the entire data set for every query like that will be my approach for like bringing the data over. 
 8:53: How do you read from S3 bucket and write into delta tables? 
 9:00: OK, so, like, writing it into the dental tables and, like from, after reading from the S3 bucket, like if the data is like already available in S3 bucket, then like I would use like data bits with 5 path to read the data and like write into a data table. 
 9:14: For example, I would first read the files from I'd say like S3 path using the appropriate format like CSVA you can say. 
 9:23: And then I would apply the required transformations and things like, you know, data type. 
 9:27: I'm not asking about the transformation transformation. 
 9:29: No, I'm not going at all. 
 9:30: I'm not going into the logical all, OK. 
 9:32: So you have a, the CSV file as we said in next. 
 9:35: OK. 
 9:36: How do you write to delta table? 
 9:37: OK. 
 9:37: You have to just move that to delta table. 
 9:39: Yeah, explain me the code base of it, OK. 
 9:42: I don't. 
 9:42: This is a hands-on position, OK, yeah, I know that this is, this is possible by a price spark or something. 
 9:47: What you would look your actual price spark would do. 
 9:49: That's what is my question. 
 9:52: OK, OK. 
 9:53: So, yeah, now I got it like. 
 9:55: The actual thing that like my Spike Spark would do, like, you know, if the requirement is simply as a CSV in S3 like CSV simply CSV in S3 to like data table, like without any transformation and like the actual Spark Pike Spark code is like pretty straightforward. 
 10:10: And, like, suppose like my CSV file is available at a like a certain, like path. 
 10:16: Like first I read it into a data frame and like the next step would be like, you know, I explicitly provide the schema for the production and especially large data sets. 
 10:27: I normally don't use infra schema because the Spark would need additional work to determine the data types, so yeah. 
 10:36: No, specifically in PySpark, right, to read the things and data, right? 
 10:40: In PySpark, there is a mechanism. 
 10:43: Do you know what is the mechanism? 
 10:45: There is a keyword to it. 
 10:47: Scripting and Python scripting Py sparse scripting. 
 10:50: OK, so, like, to be very specific, the mechanism, like, you mean like database mechanism for like again like intimately in in Pikes P. 
 11:03: OK, so like. 
 11:05: Yeah, I mean, I don't remember this at the moment, like mechanism, the specific mechanism for that. 
 11:12: So yeah, I don't remember this. 
 11:20: No Have you not heard about Moto 3? 
 11:25: Sorry, what is of 3? 
 11:28: Yeah, I have heard about it. 
 11:31: What does it do? 
 11:35: Like both, it's 4 to 3 is like mostly like AWS SDK for Python and like I have used it when I, you know, when I need a programmatic interaction with like AW services, from Python. 
 11:47: And for example, you know, working with S3 objects, listing files and like checking whether an object exists or not and like reading metadata and like or moving, I'll say like copying files between like S3 locations. 
 12:00: So yeah, like, you know, like one distinction that I would make is that like, you know, for large scale distributed data processing, I generally use Spark to read the actual data set from S3 and like. 
 12:12: If I use like Go to 3 for it, it is for like more for S3 level operations and like file object management, so yeah. 
 12:31: Yeah, also, OK, fine, yeah, last, you wanted to say anything, so, yeah, yeah, so yeah, could you able to share with, like, screen, screen, not only application, yeah, and then, maybe if you ask for writing a book, yeah, it's good, yeah, so like. 
 12:53: Is this visible to you? 
 12:55: Screen is visible. 
 12:56: it's loading. 
 12:58: yep, yep, yep, it's visible, yeah. 
 13:01: So, yeah, Bhaskar. 
 13:04: Yes, yes. 
 13:04: So, another thing, right, the photo ID, taken along with the background that that is the scenario, right? 
 13:11: We need realistic. 
 13:13: Another one thing is, do you have any other photo ID along with your glasses? 
 13:20: No, so, like, these glasses, like I have built it like, recently, so I don't have like, photo ID with glasses, yeah. 
 13:28: OK, that's fine. 
 13:29: You want to do, can do, yeah. 
 13:33: Is, Medicaid could be able to ask to write some program I wanted to write some programs. 
 13:40: Would you be able to write programs? 
 13:41: OK. 
 13:43: Simple program. 
 13:44: OK, two programs that we could. 
 13:47: One, I'll give you a Python. 
 13:48: The next one I'll give you a price part. 
 13:50: OK, Python program. 
 13:52: What I'm going to give you is, OK. 
 13:55: Write me a logic to generate a Fibonacci series. 
 13:59: OK, yeah, perfect. 
 13:59: That works. 
 14:01: Should I write it notepad or like, yeah, however it works, OK. 
 14:53: And Yeah Like here, like created of like favor of this function. 
 16:24: They had a function like called theology and like and represent how many theology numbers I want to generate. 
 17:31: Yeah. 
 17:32: So like. 
 17:34: Yeah, it's completed. 
 17:37: And extent, yeah, so like again, like I, as I said, like I, like defined the Fonaci functioning. 
 17:47: and, and like and represents how many numbers I want to generate and like I am creating an empty list called result, and I will use this list to store a few machine numbers like as it gets generated and like I have, yeah, declared two variables A and B that has been in the sliced like 0 and 1. 
 18:03: I like, the next line like, I have used like looping. 
 18:07: I'm running loop the loop like loop and times and like I'm using unders like because I don't actually need the loop index. 
 18:13: And like after that, like I am using like result. 
 18:17: app and A like in each iteration I open the current value of like A to my result list. 
 18:23: So, yeah. 
 18:27: so this is the main electron Nazi logic. 
 18:31: OK. 
 18:33: OK, do me one thing. 
 18:34: OK, this is a 5 part, OK. 
 18:36: You have two tables, T A, T B. 
 18:39: OK, I need a price part code. 
 18:40: OK. 
 18:41: You have to consume each table has around, 1515 attributes. 
 18:45: It's 1515 columns, table. 
 18:47: OK. 
 18:47: So you have to consume both the tables. 
 18:49: OK. 
 18:50: Then you have to read both the tables and, take only the joint records from match records from both the tables. 
 18:58: Basically. 
 19:01: The part is correct. 
 19:03: OK, OK, yeah. 
 19:46: First, like, I imported Sparkation from PySpark because like it's the entry point like I need to work with Spark data frames and tables, so that's why they imported it. 
 19:59: And like in the second line, like I am creating a part session. 
 20:04: You get a great network. 
 22:11: Yup. 
 22:13: Thank you. 
 22:14: I'm just putting you one more program in the chat, OK? 
 22:18: Just try this. 
 22:20: I'm giving you. 
 22:23: I'll also give you examples how it has to be there, treat the patient. 
 22:29: All going to the rings. 
 22:34: strange. 
 22:44: Yeah, I'll give you an example of how it works. 
 22:58: Let me copy that. 
 30:04: Yeah, so like this will be the code. 
 30:07: And that you think that Yeah, like here, like I'm using it slide, sliding window to. 
 30:14: Sorry. 
 30:25: Yeah, so like here I'm using a sliding window approach and like first countert like that that the stores how many times each character is required. 
 30:34: And like afterwards, like I move the right pointer through like F and like decrease the right required count. 
 30:41: And like, yeah, when all the characters from T are present, like I moved the left pointer from. 
 30:48: You know, forward, like to make the window as small as possible. 
 30:52: And yeah, like after I keep track the smallest valid window using start and length. 
 30:59: yeah, like finally I returned that substring. 
 31:01: Yeah OK, thank you for this. 
 31:07: OK, let me go to some questions. 
 31:09: OK, see, you have a 5 spark job your schedule in database that is running very slow. 
 31:18: How would you investigate? 
 31:20: How would you go about it? 
 31:21: Yeah, OK. 
 31:22: Like, so if my price per job is running slow, like I would investigate like it systematically, I, I would say, yeah, rather than like immediately increasing the cluster size and like at first I would check the database Spark UI to like identify like where the time is being spent, whether it is a particular stage or a task or a skill query. 
 31:42: Yeah, I would look for data skew, large shuffles and long running tasks mostly. 
 31:48: yeah, then I review the spark execution plan and we're using like explain method and like check whether we are doing unnecessary scans or like white transformations or I would say like in in inefficient joints. 
 32:03: And yeah, I would also check partitioning and file sizes, like, you know, because like too many small files, like a poorly partitioned data can significantly slow down a job with data tables I would look at like optimization and data layout as well. 
 32:19: Yeah, and last, last but not the least, like then I would review spark configuration, executive memory, and CV utilization mostly at the collection, and yeah, I would also compare the current execution with previous acceler run to like mostly determine like whether the slowdown is caused by an increased data or like volume. 
 32:40: OK. 
 32:42: OK, coming back to the next question, right, everybody says, right, the cost is going to be optimized. 
 32:50: Cost is going to be optimized. 
 32:52: You have, a process running an oracle, OK, which takes only, $100 for example. 

 
0:01: Like you mentioned G like a GI genetic guy and like. 
 0:05: Oh, sorry, what is the second one that you mentioned? 
 0:08: Agent, yeah, agent, that's correct. 
 0:10: So like for genetic AI agent frameworks like I have exposure mainly from like application education site and like I also worked with like land and concepts and like opening. 
 0:22: You know, like what, sorry? 
 0:25: What is lang chain? 
 0:27: Oh, so yeah, like lang chain basically if I. 
 0:30: Like lang chain is like a framework that is used to build applications around large language models like Chat GBT everything, and like it provides components for connecting an LLM with prompts, external to APIs and databases. 
 0:44: So yeah, this is like. 
 0:46: Where, where this embedding coming, comes into the picture at, at which stage embedding. 
 0:52: Yeah, so like, Like if parents come into picture when we like we need to do semantic search or like rack and like we take the text and such as documents and the database content and convert each piece of text to like a numerical vector like an embedding model so like yeah those vectors are stored in so like in this scenario like embeddings really come in the picture. 
 1:18: Why do you use that? 
 1:20: OK, so I Especially like the use case of like retired government generation so like we use the rack then the LLM needs to answer questions based on like our. 
 1:30: you can say like frequently changing data rather than. 
 1:34: Train knowledge, yeah, like we we trying to to deliver information from sources like our documents or databases. 
 1:42: OK, you have a model. 
 1:43: OK. 
 1:44: You have a prompt. 
 1:44: OK. 
 1:45: So in the prompt you give, my name is Shini Vascoti. 
 1:49: OK. 
 1:49: So tell me about myself. 
 1:51: It gives that Shini Vaskoti is from here, OK. 
 1:53: He got married here. 
 1:55: He has 12 years of experience. 
 1:56: He's great engineering, OK. 
 1:57: The same question you asked, OK. 
 1:59: It says that Shini Vaskoti is from India. 
 2:02: He lives in Hyderabad. 
 2:03: He is from, he is a doctor developer. 
 2:08: So two times when you ask the same question, it gives you a different answer. 
 2:11: How do you handle this? 
 2:13: OK, like asking the same questions and like it gives, like different answers multiple times. 
 2:19: So like in this scenario I would handle that like by making the application and like grounded in like trusted source, rather than relying on like, for example, if the correct information is that like has 2 years. 
 2:35: I would store his verified profile or resume as a source of truth. 
 2:41: And like in a rack system, I would retrieve that information and, you know, provide it as a context to the model. 
 2:48: And yeah, like I would also use a low temperature clear system. 
 2:52: So So yeah man, OK fine. 
 2:57: OK fine. 
 2:58: I think one minute the call will get cut. 
 2:59: Thank you for your time, sweetie. 
 3:01: Bhaskar will get back to you. 
 3:02: Thank you. 
 3:03: Appreciate it. 
 3:03: OK, yeah, OK, bye. 
 3:05: OK, bye. 
 3:06: Bye-bye. 
 3:06: Have a good day. 
