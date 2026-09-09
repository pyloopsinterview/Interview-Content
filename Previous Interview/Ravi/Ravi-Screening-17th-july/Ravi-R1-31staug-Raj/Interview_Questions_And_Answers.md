0:00: Just give me like two minutes, OK? 
 0:11: I think you're on mute. 
 0:20: just give me one minute, Ravi. 
 0:21: I'm, I'm just wrapping up a call. 
 0:22: Just one minute. 
 0:30: Good afternoon. 
 0:33: Hi, good evening. 
 0:34: How are you? 
 0:34: Oh, I'm good. 
 0:35: How are you? 
 0:37: I'm fine, but I cannot see. 
 0:38: OK. 
 0:40: You, it's pretty dark. 
 0:42: I cannot see your face clearly. 
 0:45: Do you think the lighting can be improved? 
 0:53: in his 2nd year. 
 1:00: No it's good. 
 1:04: I mean, is there a way that you can turn on the other side where there's a direct light? 
 1:14: I see. 
 1:20: Is it burden normal? 
 1:23: I mean, I can't even see your eyes at all. 
 1:25: Like it's very, very dark. 
 1:29: Where do you have the bulb, you can maybe turn on that side. 
 1:38: This is OK, this is, this is OK. 
 1:42: All right, so, Ravi, where are you based at? 
 1:47: And what is your work authorization? 
 1:51: OK. 
 1:53: I will need to record this. 
 1:54: Are you OK with that? 
 1:55: I'm OK with that. 
 1:58: I can appreciate that. 
 2:09: OK, Ravi, with your prior consent, I'm recording this call, just reconfirming. 
 2:15: Yeah, sure. 
 2:16: And do you have the JD? 
 2:21: OK. 
 2:22: OK, so we'll put that on the chat box just for your reference. 
 2:26: You said you're in New York. 
 2:29: no, I'm in, not in New York. 
 2:32: Northern New York, so you're in EST time zone, right? 
 2:36: OK, so this rule will be working in UK timing. 
 2:40: So let's say about 9 a.m. UK time that we, taught for. 
 2:50: 4 a.m. Eastern, would that be fine? 
 2:54: Yeah, yeah, it's fine for me. 
 2:57: And I think the client has a slot on September 2nd. 
 3:03: At 2 p.m. UK time. 
 3:10: OK. 
 3:10: That'd be, that'd be, I guess, 2 p.m., 8:00 a.m. central, so be 9:00 a.m. Eastern. 
 3:23: Mhm. 
 3:23: At Berkeley. 
 3:25: OK. 
 3:28: All right, so if you want to take a minute to go through the JD that I put in the chat box, just let me know if you need a minute, yeah. 
 3:59: Mhm Oh yeah, I go through it and it's all like related to my previous work. 
 4:21: -huh. 
 4:22: OK. 
 4:26: Right. 
 4:33: So, so how much experience do you have, in data, in total? 
 4:39: total I have in data almost around 8 to 9 years, but, like total I have 12 years of overall experience in like the data engineering and like, my experience includes building the ETL and ELD pipelines, data warehousing, also the cloud data engineering. 
 4:57: Mhm. 
 4:58: you have 4 years in daytime, you said no. 
 5:03: 12 total and in data particularly 8, OK. 
 5:12: And how about, how about snowflakes? 
 5:21: And SQL ATL also you said 8 years. 
 5:31: NAWS 9. 
 5:37: Python. 
 5:38: 12 years. 
 5:39: It's my primary language, so. 
 5:44: OK. 
 5:46: So can you explain the snowflake architecture that you have implemented and how did you design databases, schema, warehouse, or RBAC and security? 
 5:56: Sure, like, currently talking to our like the snowflake architecture, like, basically in my current project we use the Snowflake as a central cloud data warehouse, like, and I have like work on the architecture from like injections to the transformations and like conumption and. 
 6:14: see, like, at a high level data comes from like the source like the Oracle, SL Server guideware, APIs and like external files, and we, typically land the raw data in AWSSC and then like use the, like the snow pipe or like the scheduled injection process to like bring it into the snowflake and in the snowflake like I generally organize. 
 6:37: The data, like database into the layers such as like a raw or staging or transform also the curated or the like reporting layers. 
 6:46: So this keeps the source data separate from like the business, transform data also, like for the schema design depending on the use case like we use fact and dimension tables for like analytical workloads and. 
 7:00: apply proper keys, relationships, and the naming standards and also consider things like the data volume, query patterns, and implemented processing while like, designing the tables. 
 7:19: And can you describe an in an ETL ELT pipeline? 
 7:22: Are you built using Python by Spark, SQL and AWS? 
 7:26: sure. 
 7:27: Like, we first, like, in pipeline, we first like identify the source systems like which can be like, Oracle, SQL, or Guideware, rest API or any files, so. 
 7:39: Like the data is extracted either through the batch processors or, or like APIs and like for the cloud-based pipelines, as I told you earlier, like we normally, land the data first in AWSS3 and from S3 like we load the data into like the raw or the staging area in Snowflake, depending on the requirements and we use the snow, snow pipe like for, a continuous for the filebamissions or like the scheduled processes is for like. 
 8:07: , batch loads and, once the data is in the raw layer we perform transformations using the Snowflake SQL, Python, or the PS path. 
 8:17: So mainly these includes cleansing data type, conversions, like the duplications, applications, business rules like and also handling the incremental data and like for incremental processing, I worked with the snowflake streams and the tasks, so. 
 8:34: Like the transform data is then loaded into the curated and the reporting layer and typically into fact and the dimension tables or like other businesses specific structures and talking to our like orchestrations we use the airflow to manage the end to end workflow. 
 8:52: Including like dependencies, retry schedulings and monitoring, and, we also build the data quality checks into the pipeline, for example, like, record counts, checks, duplicate checks and like social target reconciliations. 
 9:12: So you only have the ceiling light. 
 9:14: You don't have any light on the walls or any lamp, yeah. 
 9:22: OK. 
 9:29: Oh, is it good? 
 9:33: I don't see you Mhm. 
 9:46: Yeah, this is better. 
 9:48: I think you, increase the brightness, I guess. 
 9:50: Yeah. 
 9:51: Is it maximum? 
 9:53: yeah. 
 9:54: OK, this is better than before. 
 9:59: OK, so can you, can, let's talk about the snow pipe stream and task. 
 10:04: so if you can explain how have you your snowflake, snow pipe stream, snow pipe and snowflake stream and task for real-time or incremental data processing. 
 10:16: like for the incremental data processing, sure, like in, in my recent project, like I've used a small pipe, streams and the task like together to. 
 10:26: generally support the, near real time and the incremental processing. 
 10:29: Like, for example, like, when new files arrive in S3, snow file like automatically detects those files and like loads the data into like the Snowflake raw or the staging table. 
 10:42: So normally this removes, the need for like the traditional batch processing or like to, continuously check like for the new, new files and, once the data is loaded like I use. 
 10:57: a snowflake stream on the staging table and like the stream keeps track of changes like, such as, newly inserted or like updated reports without like having to process the, like the entire table again. 
 11:11: And then I use this snowflake task like to run the transformation logic based on those changes and like the task basically needs the same, applies the required business rules, perform cleansing and deduplication and loads the data like. 
 11:30: Into the targeted and the curated tables and task can like also be changed when there are like the multiple dependencies. 
 11:37: So like the overall flow is basically the S3 then go to the like snow pipe raw table, stream task and then curated or the target table. 
 11:52: OK, and, can you describe a complex of 5 spark, spark transformation you have implemented and how did you optimize the performance for large data sets? 
 12:07: I remember like one of the most complex pass for transformation is like I implemented was for healthcare claim pipeline like the data was like coming from multiple source systems like with the different formats and The first step was like reading the large data sets from S3 into the Spark data frames, and we then performed the data cleansing, standardize the data types, handle the null values, and remove the duplicate records using the business keys. 
 12:39: And like the complex part was. 
 12:41: Like combining the data from multiple sources and I like use joints between the claims, member, provider, and the policy tables and, and also it's followed by the window functions like the room number, like to identify the latest records and remove the duplicate versions and, you know, like we also applied the conditions, business rules using like when, when the, otherwise to classify the claims into the different categories. 
 13:10: And also after the transformation, like we Aggregated the data to calculate the business mattresses and validate the record sounds before like like loading it into the snowflake and then like the pipeline process the millions of records. 
 13:26: So like I optimize it by using the power singing, broadcast joints for like the smaller lookup tables and avoiding the unnecessary shuffles. 
 13:35: These reduce like the overall processing time and significantly while maintaining the data accuracy. 
 13:43: And And can you explain your hands-on experience with S3, glue, EMR, lambda, IAM, Redshift, and what services did you use together in a production data pipeline? 
 13:58: OK, like start with S3 S3 has been one of the primary services like I use like, we use it, as like a data lake and like landing zone for the raw files like, we can say coming from the different source systems and, like I have worked with different file formats like, CSVJsons, and like pocket along with the, parts and organized data like that, business data and sources and, Glue. 
 14:25: Then I use Glue jobs and like the data catalog for like, ETL, processing and metadata management and like, for like larger Spark workloads and I also work with, EMR, like partition to Spark, the base distribution processing and, lambda lambda, like for the lightweight even driven processing, for example, like, or like triggering a downstream process when I like file lines in S3 or like, performing the small variations and the notification task and I am, I am like I work with rules and policies to provide the secure least privileged access between like service such as F3 Blue lambda like snowflake related workloads and Apart from this, I also work for with, Redshift. 
 15:13: Like I work on like, loading the transforming analytical data, writing the skill queries, supporting performance, optimizing although like, Snowflake is my life is stronger and more like recent data where I experience are like comfortable working with the red, red shift as well. 
 15:33: Yeah. 
 15:35: And can you describe a migration that you have worked on from Tata Data Hadoop, Hive Redshift, Oracle, SQL Server, or another legacy platform to Snowflakes, AWS? 
 15:47: Oh yes, like I remember like I worked like on multiple data migration projects like involving sources like the Oracle SQL server, Teradata, Hadoop, Hive, and like the red box like with Snowflake being one of the major target platforms and. 
 16:04: like, for example, like I can share is a migration where we move data from Oracle and like Hadoop Hive into the Snowflake. 
 16:12: So we first like analyze the source like schemas, st dependencies, the data types, volumes, and existing eti logics, and then, we like created the source to target mappings and identify any data type or or even like the business, like business rule differences. 
 16:30: And like for for the migrations we extracted the data and the landed in in 3 then like use the AWS Glue and Pass pack like for the larger transformations and cleansing before like loading it into the snowflake and like for incremental loads like we use watermark or like a chain-based logic so that we did not have to reload the complete data set every time and, like, yeah, after loading, I was heavily involved in validations and reconciliations, and, we compared source and the target record counts and checked the, like the, business, business to, totals, the validated import fields and the null values, and also the verified like the parent-child relationships. 
 17:19: and last, like, we also had to handle things like the datatype mismatches, large volume tables, and dependency sequences between like parent and the child. 
 17:32: Yeah. 
 17:35: And, given a large transactional data set, how would you design a dimensional model with fact and dimensional tables? 
 17:44: like, generally for a large, transactional data set, I would first understand the business process and the like the green of the transactions because that's the most important part of like the any, any dimensional modeling. 
 17:58: Like if we are like modeling insurance transactions, I might like define the green of like the pack table, like as one row per policy transactions, like a claim transactions and. 
 18:11: depending on the business requirements, then I like would create a central fact table, containing the, miserable business maresses such as the, transactions amount, premium, claim amount, quantity, and like the relevant points and around the like fact table, I would create, dimensions such as customer policies, product, provider date, location. 
 18:34: So these dimensions contain the descriptive attributes like used for filtering and reporting. 
 18:42: OK. 
 18:43: And have you implemented data validation, reconciliation, completenessness, completeness, and data quality check in a production pipeline? 
 18:52: yes, most recently I like to do that in my current project like data validation and reconciliation have been a regular part of like my production pipelines. 
 19:04: Like for every major pipeline, we typically perform the checks at the different stages like. 
 19:11: first we validate the completeness such as like the source versus target record count and whether all expected files or the partition partitions have like been processed and then like we perform the data quality checks like we can say a null check or on mandatory duplicates detections, data type validation, business rules and like for consolations. 
 19:33: We compare source and the target accounts and like important business level matters such as the transaction amount or the totals. 
 19:43: OK. 
 19:47: And can you describe the production workflow you built using airflow AWS glues type functions and how have you handled dependencies, or retries, a failure, alerting it to you or reruns? 
 20:08: I use the layer and AWS for the actual processing. 
 20:11: Like the sea, like the workflow started with the airflow trigger the pipeline based on schedule, and we first performed some source availability and file checks and once the required data was available in S3, airflow triggered the appropriate AWS glue job and, the glue job use fires pack to read the data from S3, perform, cleansing, transformations, and duplications and, same as like the business processing and then. 
 20:42: load the, process data into the, target layer such as the snowflake or like the red shift and. 
 20:49: After the glue job, completed, like air flow check the job status and then like trigger the next dependent task, and we had task dependencies, retriess, failure handling, and like the alerting configured. 
 21:03: So if like a glue job failed, downstream task would not execute until like the issue was resolved. 
 21:15: OK, and, how have you, how you have implemented GitPlus, Jenkin or GitHub actions plus Docker Cuban Native for deploying the data pipelines. 
 21:27: Yeah, like I worked with like the, Gitbase CICD for like managing and deploying the data engineering code. 
 21:35: Like we use it for like the source control. 
 21:37: Like we are our developers work on feature branch and raise the full request and after the code review and the approval, but like changes are merged into the main branch and same like for CSCD I worked with Jenkins and the guitar actions. 
 21:51: Like the pipeline typically perform the steps like the core checkouts, validations. 
 21:56: unit testing, lending where the applicable, and then the packages, and deploy deploys the required Python fi pack, scripts and, airflow decks and, configuration files like, to the respective environment and Docker like used for canonizations to, package the application and their dependency so that the same environment can be like, used across our development testing and instruction and in last. 
 22:25: 2 minutes, like have like exposure to deploying and managing the, containerized workloads, including the we can say, configuring ports, deployment service, and like the environment specific configuration. 
 22:42: I think I'm done from my end. 
 22:44: Ravi, do you have any questions for me? 
 22:46: like, first one is like, apart from this one, is there any other round for this room? 
 22:55: I'm sorry, what? 
 22:56: Any what? 
 22:57: apart from this, is there any other? 
 23:00: Yes, yes, yes, yes, this was just a screening round. 
 23:02: We're gonna go, submit the profile of the client, and after that they will schedule their own, their own rounds. 
 23:08: Sure, and I would also like to understand, what are the like the main priorities would be for this role in the first few months and what kind of the projects or the data challenges like I would be like working on. 
 23:21: So the, project related questions, I would rather suggest you do park for the later stages when you will appear in the next round of interviews. 
 23:28: You can ask them that. 
 23:31: And, I think Mark has already discussed the rate part with you. 
 23:35: I think 65 and W2, that could be a little on the higher side. 
 23:39: So do you think we can come down to 60 and W2 instead. 
 23:44: Is that non-negotiable? 
 23:46: We might get a pushback. 
 23:47: That's why I'm asking. 
 23:49: negotiated. 
 23:51: You can do 70 but not. 
 23:54: If I could do, I would have done 75. 
 24:00: No, the only reason I'm asking is that there could be a pushback. 
 24:04: That's why it's not. 
 24:08: OK, we'll, we'll keep you, posted on that, Ravi, if it, if at all, if it's required, I'll, I'll call you back, but, yeah. 
 24:17: Do you, so it's no questions anymore. 
 24:21: OK. 
 24:22: Thank you for your time and you have a good rest of your day. 
 24:26: Thanks, bye. 
