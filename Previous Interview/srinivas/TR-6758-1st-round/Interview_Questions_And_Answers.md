0:02: Ha. 
 0:03: Hello. 
 0:10: Hello. 
 0:11: Am I audible? 
 0:19: Hello. 
 0:21: Yeah, sorry, I'm late 2 minutes. 
 0:23: No, no problem, no problem. 
 0:25: OK, so you have the dog job description. 
 0:28: It is Python. 
 0:30: It's good, I means snowflake, spark, and, what is that, some database higher snowflakes, snow snowflake database. 
 0:40: OK, so I will mainly ask you a question about the Python quill. 
 0:45: And the spot, OK, sure, so that on that, on that day it didn't happen. 
 0:50: So you just introduce and tell what you're experien in this field. 
 0:55: Sure, sure, sure. 
 0:56: So like I would say like, yeah, like I have like exposure to like, I would say around with Python and I have extensively. 
 1:05: for building, building the back end services, rest APIs, batch processing, and also data pipelines, and also I work with the school on a daily basis providing the context queries, optimizing performance, I'm working relation and databases regarding Spark. 
 1:21: I have, like used FiSpark for processing large data sets, also performing the data transformations, filtering, joints. 
 1:30: Aggregations and optimizing the distributed data processing workloads and here we use it whenever we need to process very high volumes of healthcare claims and clinical data efficiently and for Snowflake like I have experience working with it as a cloud data warehouse where I have written the S2 queries, created the tables and used. 
 1:51: loaded the data and, use it for analytics and reporting. 
 1:55: And also I have like also integrated Python applications with Snowflake to read and write data as part of ATL and data processing workflow, so yeah. 
 2:05: OK, so, what is the difference between the panda data films and spark data frames? 
 2:11: What's the basic difference? 
 2:12: Sure, sure. 
 2:13: If I talk about the basic difference between the pandas, like actually, the pandas and sparks are basically not the databases. 
 2:20: They are both data processing frameworks, but they are like designed for different scales. 
 2:26: So pandas is mainly used for working with data that fits into the memory of a single machine and. 
 2:33: It's like great for data data analysis, cleaning, transformations, as well as the acceleration analysis. 
 2:39: And what about the data frame? 
 2:41: What's the difference between the data frame and frame? 
 2:44: Sure, sure, I'm, I'm, I'm like, like, like, like, like on it like, so basically the, if I talk about like the, pipe part on the other hand I get built for I would say. 
 2:56: Data and it processes data in a distributed manner across multiple machines in a cluster and this allows us to like 100, like hundreds of gigabytes or even terabytes of data efficiently using the parallel processing and it's commonly used for large scale ATL pipelines and big data workloads. 
 3:15: So panda is 5 database has some limitations that you can do in panda, but you cannot do in 55. 
 3:23: Can you tell me that what is that? 
 3:25: Sure, sure. 
 3:26: So yeah, like that definitely has some of the limitations. 
 3:29: Basically, if I talk about like one key limitation is that the pass pack is optimized for distributed processing, not for interactive data analysis like pandas. 
 3:38: And like both like basically both like Mandas and Pywa are used for data processing. 
 3:43: Panda provides many features that are like either little or less convenient in P. 
 3:48: for example, Like find pandas allow you to work like interactively with data that's that's loaded up entirely into memory. 
 3:56: So operations like the Spark, you can do the interactively. 
 3:59: So 5 spark, but not 5 sparks. 
 4:01: Spark has some online interference that you guys can kill our language. 
 4:08: You can do the interacting things in the Spark also, but OK, I know, I go to the point. 
 4:14: So you can write it quietly to select the. 
 4:19: Find the data frame, can you do it for the spark also spark data frame also. 
 4:24: So yeah, like, if I talk about you can I just select here because I just see the complex select query in 5 spark, data frame loading. 
 4:34: Yes, like we can, like, like in PySpark we can run the SQL queries, against the Spark data frame by first creating a temporary view, and, the difference is that the Pandas itself doesn't need any support the SQL queries. 
 4:47: If we want to use the SQL with the PandaS data frame, like we usually, need an additional library like, like Panda SQL or, or load the data into the SQLI. 
 4:57: So yeah. 
 5:00: No, no, no, my question is, so pandas, you are, you are loading the loading the data that time you can write a ser complex query. 
 5:11: Why you can write this thing you write a complex query and that can be load to the panda or I. 
 5:17: OK, so why it is possible and why it is not. 
 5:21: OK, OK, OK, I got, I got your point. 
 5:23: OK. 
 5:24: So, like, basically, if I talk about like that is possible like within the, but, but mechanism is slightly different. 
 5:31: In Pandas, when we load data using the, like PD. 
 5:36: SQL, this, the SQL queries executed directly by the Source databases we can write a very complex query with joint aggregations and in Spark we generally don't like execute the arbitrary SQL while reading the data in the same way. 
 5:51: So basically Spark. 
 5:56: Could you please come again? 
 5:59: So that that 5 part data frame permit that you can write a query in the 5 spar or data frame argument and load that is it possible? 
 6:10: OK, OK, so yeah, like, it is like, I would say like, like it's, it's possible like whenever we're reading the data through, JDBC don't mind, I'm, I'm in the office, OK, so yeah, so don't, no problem, yeah, definitely it's possible like when, when reading the data through JDVC instead of loading on entire table we can pass as will query. 
 6:32: Yeah, it's definitely possible. 
 6:35: OK, and, so in this as well, why do you will, prefer join and why do you prefer nested query? 
 6:45: Can you give me an example of some scenario? 
 6:47: Why do you prefer the nested query and why do you prefer the join and just be the. 
 6:55: Give me a, give you a feedback. 
 6:56: 5 spot data frame you cannot write complex query. 
 6:59: You just select the all columns the total table you have to load and then you 5 spot, you have to process the data. 
 7:08: But one day you can selectively do the query. 
 7:10: OK, so, so this is the thing I just want to give you feedback. 
 7:14: And the thing, the second thing is that, OK, why, when do you like to join and when would you like to do listed query. 
 7:20: OK, basically, it depends on the use cases. 
 7:23: In general, I prefer joints whenever I need to combine related data from multiple tables because they are usually easier to read and in most databases, the query optimizer executes joints more efficiently. 
 7:36: For example, you. 
 7:44: OK, OK, got it. 
 7:45: So basically an object query or subquery is useful when the result of one query is needed as the input for another query. 
 7:51: For example, if I want to find patients whose claim amount is greater than the average claim amount, I would first calculate the average in a subquery and then compare each patient's claim amount against that value. 
 8:03: So yeah. 
 8:05: So but when you prefer, so same thing you can do by the joint, same thing you can do with this, nested query. 
 8:12: OK. 
 8:13: Now, when you will use the nested query and when you use the joint, so that give me that that scenario. 
 8:19: OK. 
 8:20: In short, I would say if I talk about joint like when combined, I use the joints when combining data. 
 8:27: From multiple tables and I use the nested query when I need an intermediate result such as filtering based on an aggregate or ranking or a or a derived data set. 
 8:38: I think, I hope, yeah. 
 8:40: So, can you give me the scenario why is not possible? 
 8:43: OK, you want the scenario. 
 8:45: OK, OK, OK. 
 8:46: So if I talk about the scenario, let me give you one scenario here, like, like, like, like, like, basically give you, like, like, like, let me, let me give you an example from my, my project. 
 8:58: Suppose like I have like two tables, patients and claims, and, if the, like, if like if the business ask me to show the patient name, claim ID claim amount, and claim status, I would use a joint because I need columns from both tables based on the patient ID. 
 9:16: Now, suppose like, like the business asked me to find patients whose claim amount is higher than the average claim amount across all the patients. 
 9:25: In that case, I would use the nested query because I first need to calculate the average claim amount and then use that result to filter the record. 
 9:33: So yeah. 
 9:37: Now if your ramp size is small in in your database, then you what initiative query or OK, OK, OK, OK, got it. 
 9:49: OK, yeah, sure, in particular in the scenario, I think like, it also like it basically depends on the like, like in the size of the data for like for a small database, I don't have a strong preference because the performance difference is usually negligible. 
 10:05: So here I would choose the approach that is simpler and more reliable, which is, often a subquery or for a large database I generally prefer joints because they are usually better. 
 10:14: Optimized by the database engine and tend to perform the better. 
 10:19: Why, why, why you choose a large database to small database you don't choose well? 
 10:23: OK, OK. 
 10:25: So like for, for like the, like the databases, I think like, if like both join and sub query can also be problem like solve the problem. 
 10:35: My preference depends on the data size and performance. 
 10:37: Because, for the small tables, either the joint or softwa is fine because my, my constitution, the machine or the install its RAM is limited. 
 10:50: OK, now what do you prefer, join or softwary? 
 10:55: OK, OK. 
 10:56: If the, like the, if the, if the RAM is like, like is, basically I think I. 
 11:05: What I, what I, what I think like, if the machine has like limited RAM, OK, so all the database a memory constraint, so what I, so what I think is like, it, it basically like I would generally prefer like I would say, subquery especially if the filters and data early and why, why you are not, why you not, join here, OK, why I I use joins here when the RAM size is, OK. 
 11:32: OK. 
 11:33: I think, I would say if the RAM size is slow, why I'm not joining using because if the memory is limited, a joint can like become expensive here because especially when join, when joining, like joining two very large tables, the database may need to build hash tables or, or sort large amounts of data which increases the memory usage and can, can spill, spill to this discourse slowing down the query. 
 12:00: So yeah. 
 12:01: So what is the OLAP database? 
 12:04: OK, OCP database and the OSA database. 
 12:06: What is the difference? 
 12:07: OK, OK. 
 12:08: So the major difference between the, OLDP and OLAP is like the, the OLAP database like basically. 
 12:16: has, like, let me first go through it through the OLTBs that is the online trans processing. 
 12:21: It is basically a database that are like designed for day to day transition operations. 
 12:25: They handle a large and large number of small transactions such as insert, update, delete, and simple, simple select, select, select topic. 
 12:35: And for like a lab like that is the online analytical processing that is the databases that are particularly designed for I would say reporting and analytics and they poss large volumes of which kind of query, which kind of query is OK, OK, I think like. 
 12:58: if I like, if, if I'm like in an online databases, we generally prefer the, I would say a complex analytical queries rather than foundational queries. 
 13:07: These queries typically involve the aggregations, group by, or the actually it is is preferable. 
 13:15: So now my question the database or while Cyne is fast, their instruction is not fast. 
 13:22: And that is why instruction division is fast. 
 13:25: Their select is not fast. 
 13:27: OK, can you explain it luid manner in the usage of data structure why insertion is fast, but select is not fast. 
 13:35: so because in the back end of the in the database there are some data structures. 
 13:40: So can you explain in the data structure for format one select is fast and another another instruction is fast. 
 13:48: Yeah, that's because the well depend lab databases are optimized for different purposes. 
 13:52: I was on the Python like missed and and missed, whichever it's just done it fast and while select it fast. 
 14:06: OK, 3 and the hashback. 
 14:08: OK, got it, got it, because it's on the back end of the database. 
 14:13: OK, got it, got it. 
 14:14: So, like, I, I would say, like the, the reason is like how the data is organized internally because here the data is stored row by row when, when I insert or update or update a record. 
 14:27: The database simply appends or like modifies, I would say modifies, like modifies like one row so insert update and delete are very fast. 
 14:37: However, if we We run a large query that that needs only a few columns, more from millions of rows. 
 14:46: The data which still has to be every row and in the app like the data is stored column by column, so all the values of a column are stored together. 
 14:56: So when we execute. 
 15:06: He's faster and Juarez. 
 15:09: Fix is faster. 
 15:12: OK, I didn't basically like the instruction is generally faster because the database is simply provides new data to storage or I got it. 
 15:30: Got it, got it. 
 15:34: OK, so insertion is for for Python link list insertion is fast because if, if I already have a reference to the node, I only need to change a couple of pointers and searching or searching is slow because a linked list does not support a random access. 
 15:50: I have to like travel. 
 15:54: I go to have like now they're about to have a dictionary and the fee compared the same comp we do with the dictionary and, OK, got it, got it. 
 16:06: You can store the data, you know, the database back back in some data was stored in binary tree. 
 16:11: Some data was stored in few healthfare, so that's a very dictionary. 
 16:15: So basically, so why, why is such a possible, OK. 
 16:21: so basically if I talk about like a Python condition is implemented using a hash table while a tree stores data in a hierarchical, sorted structure. 
 16:32: So like, so that's like, like it, it, if the databases uses a hash table, additionally insertion and lookups are generally very fast on, on average. 
 16:42: That's because the databases compute, computes a hash of the key and, and like. 
 16:50: And I find the dictionary. 
 16:56: What is the, what is the time complexity, what is the time complexity of touching a key in a dictionary? 
 17:03: I'm sorry, but I'm not able to like get your diary, so you know the time complexity of the problem the problem has some time complexity in in order of order of, OK, so in dictionary. 
 17:22: a memory, so I end the memory, you have to type that in the key. 
 17:26: I keep that key key if it's present or not. 
 17:29: It is a key to the picture or not or the type of of the problem. 
 17:33: So basically in dictionary, the average time complexity for for inserting searching is like omega one. 
 17:41: Good, good. 
 17:43: OK. 
 17:44: OK. 
 17:45: OK. 
 17:46: OK. 
 17:46: So how long, how long the interview is going on? 
 17:50: I don't know, like, like, like, like, like, what are you asking about? 
 17:55: No, what is that? 
 17:56: So, OK, OK, OK, now we are, we pass spot, OK, so now you have a data there. 
 18:08: You, you have a data you have processed by the spark or spark whatever and data has strong relationship to each other. 
 18:18: How will processing work? 
 18:20: OK, OK, for processing the data in the. 
 18:25: And the like the in the pipe part what I, what I think like it like if the data has like a strong relationships between the entities the yeah yeah yeah so the first step is to really identify the common keys that create the data sets such as patient ID, claim ID, or provider ID. 
 18:44: Then I would load the data into spark data frames and perform the required joints using those keys. 
 18:49: And for smaller data data sets, I would use a broadcast joint to avoid unnecessary data shuffling. 
 18:56: For larger data sets, I would definitely use, I would use the partition the data approciately and use the spark distributed joints such as short mud joint or hash joint. 
 19:06: And after joining the late data data sets, I would apply the required inform transformation. 
 19:12: Do you graph. 
 19:20: OK, I think you are like, asking about the, like the, like I'm not like able to understand like what's your database, you know, in Spark it is there or not. 
 19:37: OK, OK, oh yeah, yeah, yeah, like, like basic, OK, I got it now like you are asking. 
 19:42: About the graph frames like in Python we generally use the graph frames where we create one data frame for for for verts and another another 4s and then we can then perform the operation like finding connected components, shortest paths or page or traversing relationships so in the scenario I have given that. 
 20:05: You have a larger data with a strong relationship. 
 20:08: These glass is applicable there. 
 20:11: OK, I think like, in your particular scenario, I think, it, it, I would say I would not definitely say yes because, because it depends on the type of relationship. 
 20:23: If the data has normal business relationships such as customers and orders for patients. 
 20:28: I would not use a graph and here the data, the real database with SQL joints is the better choice because these are structured one to many or many to one relationship there. 
 20:41: Thanks. 
 20:42: OK, so, OK, there's coding question. 
 20:46: So just use that, OK, I have to give you a coding question, now, OK, sure. 
 20:52: So write the generator and the decorator in the, Python in the, in, in, in the code. 
 20:58: Sure, sure, it's, so write it decorator generator for the pacy number. 
 21:03: So a generator generate the series of fina number people's number, you know. 
 21:10: People bonus number FN is called FN minus 1 plus FN minus 2. 
 21:15: So write a generator would generate a sequence of the fibonus number. 
 21:21: OK, OK. 
 21:29: Do you know Gator? 
 21:30: Yes. 
 21:32: Oh Yeah Oh, you did not share the scene now sharing, sharing. 
 22:04: Is it visible to you? 
 22:06: Yeah, yeah, yeah, OK, OK. 
 22:17: Can I write this in my notepad or do I use any no no no no it tells me the editor is a code editor in the in the ok got it. 
 22:46: Let me, I made it. 
 22:49: I'm, OK, OK, I may need to open an online compiler here. 
 22:53: Mhm, OK. 
 22:56: OK He is the P3. 
 23:39: OK, so let me, let me ask you one thing. 
 23:43: I need to write a, Fibonacci code using the, using generator, and you apply the gene you apply the generator we generate the series of numbers. 
 23:56: So in the end if you give the pipe, then top 5 the number will come. 
 24:02: OK, OK. 
 25:06: It's good. 
 25:07: So can you, OK, just open your, you are shutting your skin now. 
 25:11: Open your pajama and see if it's running or not. 
 25:15: Oh, pajama or whatever that you, yeah, can I use an online compiler. 
 25:21: Yeah, yeah, sure, sure, OK, OK, got it. 
 25:22: Give me a second. 
 25:25: It is to the good question. 
 25:26: OK, yeah. 
 25:44: Opening now. 
 25:45: Open now. 
 25:46: Let me copy with you and done. 
 25:52: And then, yeah, like, let me, like, let me, let me check what, what's the issue here. 
 26:05: This, yeah, yeah, edit the, co editor of the platform, OK, then copy paste to there because otherwise your things will be not recorded, OK, so your, the quality code will be there. 
 26:36: Give me a second. 
 26:37: My system is like, working a bit slow. 
 26:48: I think it's identification, identification error. 
 26:52: Oh, I think. 
 26:55: It's common. 
 26:56: It's a very common error. 
 26:58: the part of you right now with the left in the left, the loop you right there. 
 27:02: That is the problem. 
 27:04: No, that is our, I, I have. 
 27:14: Is it ready? 
 27:16: let me check. 
 27:20: OK, we are done. 
 27:21: It is half an hour, OK 30 minutes, but you feel your accent is good, OK. 
 27:26: And the only other, only the feedback is that the part I part part you have got, you do not want much because there are graph part and the dimensional data means that the graph is, used, but because graph is used the one the strong is there because there is no and with the age will be that and. 
 27:49: Data frame part, you can write a spill query complex in the loading dataoryice part. 
 27:56: So otherwise you're all things are good and you write the code and then last you have, you have on the pill for the last. 
 28:05: OK, OK, OK, OK, on this query about you have a, employee table or employee ID employee ID and manager ID is that. 
 28:20: And, Another thing is why employee name and employee ID. 
 28:28: OK. 
 28:29: Now you have to give the employee name and manager name. 
 28:36: One is manager every like every employee ID and manager ID is there. 
 28:39: It's very simple, yeah, yeah. 
 28:43: But, Let me, let me do. 
 28:47: Yeah. 
 28:50: I got your, I got your question. 
 28:54: Let me try the query here. 
 28:59: In the in the coordinated yeah. 
 29:17: Just writing. 
 29:32: Mhm OK So you are there is 11 you write him and another is you write him in the fight. 
 30:36: So that is a silly mistake, I think. 
 30:39: So it's a not employee name, yeah, yeah. 
 30:43: So basically, Hm, I think you are making a mistake here, like, but, but like, let me check here. 
 30:52: So in the 2nd line, in the 2nd line, you said, you know, I aim not to it. 
 30:56: There's no aim to me. 
 30:59: Yeah. 
 31:03: So basically since the manager is also an employee, I use the employee table twice a year. 
 31:07: So the first joint gets the employee's name and the second joint is a self-reference to another analysis. 
 31:14: This is like this is for the manager table. 
 31:16: It's very simple for you who make it complicated. 
 31:19: OK, OK. 
 31:23: I have like currently I have this in my mind so I writing the yeah yeah yeah yeah that's. 
 31:42: That is for the manager to driving. 
 31:53: I. 
 32:03: So what I'm basically what I'm trying to do here is the employee manager table stores the relationship between the employees and managers. 
 32:11: So here first I joined the employee table using employee ID to get the employee's name. 
 32:17: Then I joined the same employee table again using the, manager ID to get the manager's name. 
 32:25: So, that's my approach I'm doing here. 
 32:29: OK, now I do not push it that the MTV has a met in my name. 
 32:37: like, I'm so sorry. 
 32:39: Like, could you please like come again? 
 32:42: Yeah, OK, yeah, so basically, yeah, let me, let me give you my answer. 
 32:49: Basically, the employee manager table does not contain the employee name. 
 32:53: It contains only, only the employee ID and manager ID which represents the relationship between the employees and manager. 
 32:58: That's why I'm using your EM. 
 33:02: OK. 
 33:04: OK, done. 
 33:06: OK. 
 33:10: OK, yeah, I have, I have written the code here as well for queer. 
 33:16: OK, OK, OK, so we can finish here. 
 33:18: So we'll, I, I know that back in the video. 
 33:28: You, you did, you're doing it good. 
 33:30: OK, thank you. 
 33:32: Like Themes 
