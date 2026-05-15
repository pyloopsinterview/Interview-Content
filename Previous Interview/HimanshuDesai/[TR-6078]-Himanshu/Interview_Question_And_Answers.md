00:00:05,600 --> 00:00:05,689 [speaker_0]
Hello.

00:00:05,689 --> 00:00:08,140 [speaker_1]
Hey. Hello. Hey, Rajesh. How are you?

00:00:09,340 --> 00:00:10,470 [speaker_0]
I'm good. How are you?

00:00:10,470 --> 00:00:11,760 [speaker_1]
How are you? Good. Good afternoon.

00:00:15,460 --> 00:00:20,940 [speaker_0]
Um, I'm sorry about this, uh, meeting movements. I have, uh, you know, been in a call and, um-

00:00:21,240 --> 00:00:22,210 [speaker_1]
It's fine. Yeah

00:00:22,210 --> 00:00:25,760 [speaker_0]
...I still-- I was-- the call was still extending, so I had to drop.

00:00:26,980 --> 00:00:28,500 [speaker_1]
Okay. Do you have to drop now?

00:00:30,020 --> 00:00:31,060 [speaker_0]
No, no, no, not this one.

00:00:31,080 --> 00:00:31,360 [speaker_1]
Oh.

00:00:31,420 --> 00:00:32,040 [speaker_0]
The, the other one.

00:00:32,980 --> 00:00:33,210 [speaker_1]
Oh, got it.

00:00:33,210 --> 00:00:34,280 [speaker_0]
I, I had to drop the other call.

00:00:34,640 --> 00:00:38,180 [speaker_1]
Yeah, that's fine. No problem. I understand.

00:00:38,300 --> 00:00:46,230 [speaker_0]
Okay. Okay, so let's get started. I know we have a very short of time, but we will...
Are you okay to extend ten more minutes if we-

00:00:46,600 --> 00:00:47,220 [speaker_1]
Yeah, it's fine.

00:00:47,260 --> 00:00:47,739 [speaker_0]
Be fine?

00:00:47,800 --> 00:00:48,160 [speaker_1]
It's fine.

00:00:48,340 --> 00:01:02,760 [speaker_0]
Okay. So this is, uh... Just let me give you a little bit introduction about this project
and about myself. So I'm a technical architect working in this, um, in a project. I joined recently,

00:01:03,100 --> 00:01:03,380 [speaker_1]
Mm-hmm.

00:01:04,160 --> 00:01:09,000 [speaker_0]
And, um, I'm part of, um... I, I'm with Optum for almost three years.

00:01:09,700 --> 00:01:09,730 [speaker_1]
Okay.

00:01:09,800 --> 00:01:13,980 [speaker_0]
And, uh, with, uh... Prior to it, I was with, uh, Anthem for almost twelve years.

00:01:14,970 --> 00:01:14,970 [speaker_1]
Okay.

00:01:14,980 --> 00:01:42,100 [speaker_0]
And my, you know, my-- most of my experience is in healthcare. Um, so that's about me. And, um,
th-this project is like, you know, for Optum UnitedHealth Group, and, uh, you know,

00:01:42,680 --> 00:01:42,900 [speaker_1]
Okay.

00:01:43,500 --> 00:01:49,280 [speaker_0]
Um, we support, uh, we support and maintain their data, uh, for Illinois account.

00:01:49,840 --> 00:01:50,200 [speaker_1]
Okay.

00:01:50,300 --> 00:01:52,220 [speaker_0]
For Medicaid and Medicare mostly.

00:01:53,100 --> 00:01:53,110 [speaker_1]
Okay.

00:01:53,140 --> 00:02:19,060 [speaker_0]
So it's a government data and, um, you know, right now this is, uh,
the data processing happening on the legacy systems like, uh, Informatica, Teradata, and, uh, and,

00:02:19,700 --> 00:02:19,989 [speaker_1]
Got it

00:02:19,989 --> 00:02:38,440 [speaker_0]
...um, Python scripting and all that. So, you know, our-- eventually our goal is, um,
our future goal is to move, um, like, um, everything into cloud and, uh, bring the Snowflake

00:02:38,920 --> 00:02:39,220 [speaker_1]
Right.

00:02:39,260 --> 00:02:42,160 [speaker_0]
So that's what we are looking here. Um, any questions?

00:02:43,040 --> 00:02:48,120 [speaker_1]
No. I'm, I'm trying to understand things and I'm comfortable for now. Yeah.

00:02:49,100 --> 00:03:04,140 [speaker_0]
Sure. Okay. Okay, so let's start, uh, um, from your side. So start with your introduction and, uh,
give me your technical background and what are you doing in the current project, and, uh, you know,

00:03:04,520 --> 00:04:14,380 [speaker_1]
Got it. So, hi. Hi, Rajesh. And, like, uh, myself Bharat,
and I'm a lead Python engineer with around eleven years of experience, uh, building data platforms,

00:04:14,800 --> 00:04:14,890 [speaker_0]
Okay

00:04:14,900 --> 00:05:28,320 [speaker_1]
...effort to redesign the, uh, pipeline using the Python and Databricks. And, uh,
I build like ingestion frameworks that extract, uh, data from multiple sources, uh,

00:05:28,420 --> 00:05:49,740 [speaker_0]
Okay. Um, sure. That, that sounds great. Um, can you tell me a little bit about how the--
how you process the data within your team? Like, um, what are the technologies that you guys

00:05:50,520 --> 00:08:47,864 [speaker_1]
Right. Right. Of course, like as I said, like it's, uh, end-to-end and heavy data. So I work like,
um, on my-- in my-- in our current project, like the overall data processing, uh, is like, uh,

00:08:48,424 --> 00:09:04,164 [speaker_0]
Okay. So [clears throat] w-what were... Like are you doing, um,
any kind of a data validations before, you know, you get the data into your raw layer?

00:09:05,544 --> 00:09:06,973 [speaker_1]
Okay. So data validation-

00:09:07,304 --> 00:09:14,764 [speaker_0]
Or were you doing, were you doing any kind of a data validations or any-anything like checks
and balances or anything like that?

00:09:16,104 --> 00:10:00,004 [speaker_1]
So like, yes, definitely. I would say like data validation
is actually one of the most important part of the ETL process. So, uh, like, uh, especially become--

00:10:00,084 --> 00:10:04,344 [speaker_0]
So how were you, how were you doing all these checks? Uh, where were you doing all these checks?

00:10:05,124 --> 00:10:05,834 [speaker_1]
Uh, like-

00:10:06,973 --> 00:10:07,984 [speaker_0]
Which, uh, the PySpark?

00:10:09,104 --> 00:10:23,454 [speaker_1]
Mostly in like code, yeah, code in the PySpark or, uh, if I talk one by one then, uh, like, uh,
first like the raw data comes, uh, uh, from the source like HR, uh, claims, uh, billing platform-

00:10:23,504 --> 00:10:28,284 [speaker_0]
So will you do all these validations before the data gets into raw layer or after raw layer?

00:10:29,024 --> 00:10:44,004 [speaker_1]
Uh, okay. Um, like, uh, that the, uh... No. After the, like, the data is raw coming to us,
like before the data gets into the raw layer, we mainly perform basic ingestion, uh,

00:10:44,064 --> 00:10:50,024 [speaker_0]
So you do, you do all these validations before the data gets into raw layer? Okay.

00:10:50,084 --> 00:10:50,504 [speaker_1]
Yeah. Like-

00:10:50,604 --> 00:10:50,844 [speaker_0]
So-

00:10:52,604 --> 00:10:52,674 [speaker_1]
The-

00:10:52,774 --> 00:10:53,044 [speaker_0]
I'm sorry.

00:10:53,364 --> 00:11:10,594 [speaker_1]
No. Like transformations and, and, you know,
reconciliation validations happens in the after the raw layer. Like some of the, uh, uh,

00:11:10,664 --> 00:11:29,624 [speaker_0]
Okay. Um, so what, what, um, what... W-how do you like, you know, do these validations? Do you--
did you write any framework, um, and execute? Because these validations

00:11:30,324 --> 00:11:31,124 [speaker_1]
Right. Right. Of course.

00:11:31,144 --> 00:11:34,904 [speaker_0]
So h-how do you, how do you manage all these validations?

00:11:35,784 --> 00:12:55,704 [speaker_1]
Uh, so exactly like, um, uh, the, the, um, uh... Actually one of the main challenge, uh, we,
we identified like early in the project like because almost every pipeline required like similar

00:12:55,784 --> 00:12:55,904 [speaker_0]
Okay

00:12:56,324 --> 00:12:58,524 [speaker_1]
... you do this, yeah, with the data.

00:12:59,864 --> 00:13:28,444 [speaker_0]
Okay. Um, so can you, can you explain me, uh, like, you know, give me the, um, like architecture,
like, you know. Suppose, um, you know, you have multiple sources coming from the, uh, for,

00:13:28,724 --> 00:13:29,224 [speaker_1]
Right.

00:13:29,324 --> 00:13:53,704 [speaker_0]
So how are you-- Like, can you give me an idea in your technical terms, how
are you going to validate the schema validations, the null checks, you know, all those, you know,

00:13:53,904 --> 00:13:54,184 [speaker_1]
Right.

00:13:54,284 --> 00:14:02,284 [speaker_0]
So, uh, how are you doing that, you know, with the different files using the same framework?
What is, what is your architecture?

00:14:02,484 --> 00:15:51,054 [speaker_1]
Yeah. So suppose like, uh, we have, uh, one healthcare interface where data
is coming from multiple sources systems like member files, claims files, uh, provider files,

00:15:51,124 --> 00:15:55,684 [speaker_0]
Where do you, where do you load that metadata to compare-- for comparison purposes?

00:15:56,884 --> 00:15:58,704 [speaker_1]
Sorry, where I load that metadata, right?

00:15:59,604 --> 00:15:59,944 [speaker_0]
Yeah.

00:15:59,984 --> 00:16:00,264 [speaker_1]
Of course.

00:16:00,344 --> 00:16:04,984 [speaker_0]
Yeah. So you should do-- The metadata should be somewhere to compare it, right? If it is correct
or not.

00:16:05,044 --> 00:16:34,444 [speaker_1]
Right. Right. So yeah, of course. Like, uh, so the metadata like usually stored in the control,
like control tables inside the SQL Server or sometimes in the configuration files like JSON

00:16:36,244 --> 00:16:42,194 [speaker_0]
Okay. Um, so w-w-- so have you used, uh, PySpark?

00:16:43,604 --> 00:16:44,354 [speaker_1]
Of course. Yeah.

00:16:44,404 --> 00:16:48,454 [speaker_0]
Okay. And, uh, did you use in the Databricks or where did you use, um, PySpark?

00:16:49,504 --> 00:17:21,244 [speaker_1]
Uh, majorly, um, in the Databricks also I have used and, uh, like mainly in the Databricks, uh,
environment on the Azure.

00:17:23,724 --> 00:17:40,554 [speaker_0]
Okay. Um, [clears throat] so how do you execute, uh, the Python code in Azure, uh, you know,
when you write it, uh, using, uh, Jupyter Notebooks in Databricks? How are you going to execute

00:17:41,264 --> 00:19:04,468 [speaker_1]
Okay. So first of all, like, um, the execution flow in our environment is like usually work, uh,
like first developer creates a and tests the PySpark notebook inside Azure Databricks,

00:19:04,648 --> 00:19:18,328 [speaker_0]
Yeah. Okay. So, so you said you used PySpark. So have you used PySpark for every, uh,
for everything, or did you use any other functionality in Python a-apart from PySpark framework?

00:19:18,648 --> 00:20:16,788 [speaker_1]
Okay. Okay. So basically, majorly, um, speaking about PySpark, because majorly the PySpark is used.
But like, uh, uh, if I talk about like we also use regular like Python, SQL

00:20:16,968 --> 00:20:51,068 [speaker_0]
Okay. And, uh, [clears throat] um, so have you like, you know, every, um... Sorry.
So even for the data-based processing, like, you know, the members data or like any, any other data,

00:20:51,988 --> 00:22:24,368 [speaker_1]
Of course. Like, as I say, like Python, I mean to say we can use Pandas there. So that is the,
I mean, but the like, um, I would say like, uh, we,

00:22:25,788 --> 00:23:01,228 [speaker_0]
Okay. Um, so like I'm-- that's a very good point between like, uh, Pandas versus the Spark,
but Spark also has some disadvantages like processing, um, large volumes of datasets. What have you,

00:23:02,428 --> 00:24:13,868 [speaker_1]
Of course. Like, um, in my experience up to now, like I have faced enough, uh, difficulties.
Like Spark is very powerful for the, for large scale distributed processing,

00:24:13,908 --> 00:24:30,477 [speaker_0]
So how do we, how do we identify the correct total number of executors, like, you know,
the memory space that require parallel processing, you know, the engines? You know, how do you,

00:24:31,760 --> 00:25:56,330 [speaker_1]
Of course, like, um, if I have to talk, uh, I mean, on that. So, uh, like when we, uh, uh, I mean,
talk about the parallel processing in Spark, so one of the, of course, key thing is,

00:25:57,360 --> 00:26:07,380 [speaker_0]
Okay. Um, sure. And, um, uh, do you know anything about Terraform scripts like Terraform in Azure?

00:26:08,620 --> 00:26:32,800 [speaker_1]
Yeah. Uh, I mean, I'm not very, uh, I mean, not more than the Python and PySpark, but yeah,
I know about those and I have... As I say, like I, I worked with the devops team

00:26:32,860 --> 00:26:34,480 [speaker_0]
Have you written any Terraform scripts?

00:26:35,400 --> 00:26:37,270 [speaker_1]
Yes. Few, I mean-

00:26:37,580 --> 00:26:37,610 [speaker_0]
What-

00:26:37,900 --> 00:26:38,600 [speaker_1]
I would say like few.

00:26:40,140 --> 00:26:44,100 [speaker_0]
Okay. Can you, can you explain me like now what, what have you done in Terraform?

00:26:45,800 --> 00:27:54,449 [speaker_1]
So like, uh, if I, [clears throat] uh, like my involvement with the Terraform is mainly around the,
uh, like, uh, supporting Azure-based data engineering environments

00:27:54,600 --> 00:28:07,340 [speaker_0]
Okay. Okay. Um, so how, how did you... Like do you have any experience in Teradata,
like the sequels?

00:28:08,240 --> 00:28:15,970 [speaker_1]
Of course, I know about the sequels, uh, but, uh, like, uh, Teradata, like, uh, if I-

00:28:16,060 --> 00:28:19,560 [speaker_0]
Do you know anything about the loader util? It's because these are-

00:28:19,920 --> 00:28:20,380 [speaker_1]
Sorry, sorry.

00:28:20,660 --> 00:28:38,720 [speaker_0]
These are mostly, um, you know, the, the legacy migrat-
legacy code migration into refactoring into Python. So do you know Teradata

00:28:39,040 --> 00:29:39,270 [speaker_1]
I know very much about them, Informatica. And like, uh, uh, I have... I mean, that, that
was the one of the case for us also on the project. And like one of the, I mean, um,

00:29:41,120 --> 00:30:00,440 [speaker_0]
Okay. Okay. Um, sure. Um, what else? Like, um, yeah, um, [clears throat] let's stick up on SQL,
okay?

00:30:00,840 --> 00:30:00,920 [speaker_1]
Yeah.

00:30:02,440 --> 00:30:14,160 [speaker_0]
Um, so can you write me a SQL? Like, you know, I have a table, uh, I have a table, recipient table.

00:30:14,880 --> 00:30:15,080 [speaker_1]
Mm-hmm.

00:30:15,400 --> 00:30:24,180 [speaker_0]
And, uh, the member date of birth, recipient, uh, member table and member date of birth
is in varchar, like string dat- string format-

00:30:24,360 --> 00:30:24,740 [speaker_1]
Mm-hmm

00:30:24,820 --> 00:31:26,800 [speaker_0]
... string data type. And, um, for some reason it is accepting every value like, you know,
any format, YY/MM/DD, DD/YY/MM, you know, any format like, you know, fifth MayUh,

00:31:27,080 --> 00:31:27,960 [speaker_1]
Yeah.

00:31:31,560 --> 00:33:55,600 [speaker_0]
Okay. So you're writing in, um, where like, um, in SQL Server, SQL Server SQL?

00:33:56,580 --> 00:34:01,579 [speaker_1]
Like it's a online, online compiler editor.

00:34:01,640 --> 00:34:08,900 [speaker_0]
No, no, no. It's not the editor, like the SQL syntax because try convert date, member date, DOB,
comma one one two.

00:34:09,980 --> 00:34:10,200 [speaker_1]
Okay.

00:34:10,240 --> 00:34:11,740 [speaker_0]
Is that SQL Server SQL?

00:34:12,040 --> 00:34:14,420 [speaker_1]
Yeah. So SQL Server editor.

00:34:16,260 --> 00:34:16,580 [speaker_0]
Okay.

00:34:26,480 --> 00:36:39,580 [speaker_1]
Like using some T-SQL functions like try convert and all, so that as well.

00:36:58,930 --> 00:37:02,270 [speaker_0]
So how-- so you remember that one one two, one O three T-sequels?

00:37:02,970 --> 00:37:21,910 [speaker_1]
Of course, yeah. As I say, like, it is the T-sequel I'm using the syntax. There
was a time T equals L, T-sequel syntax. Yeah, I remember that. Yeah.

00:37:28,630 --> 00:37:43,770 [speaker_0]
So convert-- you're, you're converting to varchar eight. Um, so already that is in varchar, right?
Why are you converting it? I... So it is con-- The conversion should be to date format, YYMMDD.

00:37:45,410 --> 00:38:31,090 [speaker_1]
Okay. So, basically, you, you are saying, like, I should change that or? Sorry.
[clears throat] Okay. So I mean, if I say about myself, like, since the, uh, column

00:38:32,470 --> 00:38:32,750 [speaker_0]
Okay.

00:38:32,790 --> 00:38:33,330 [speaker_1]
Yeah.

00:38:35,910 --> 00:38:39,450 [speaker_0]
Sure, that's fine. Um, okay. This is fine.

00:38:40,210 --> 00:38:40,220 [speaker_1]
Yeah.

00:38:40,250 --> 00:38:44,770 [speaker_0]
And, um, like, do you know anything about analytical functions in SQL?

00:38:46,210 --> 00:39:06,250 [speaker_1]
Yeah. I mean, a little bit. Uh, not all. [laughs] That's what I would, I would say. Yeah.
So you can ask. Uh, row number, rank, the lag, sum, average. So these

00:39:06,410 --> 00:39:06,690 [speaker_0]
Okay.

00:39:06,970 --> 00:39:07,040 [speaker_1]
Yeah.

00:39:13,750 --> 00:39:14,710 [speaker_0]
Um, all right.

00:39:15,110 --> 00:39:15,230 [speaker_1]
Yeah.

00:39:16,750 --> 00:39:21,870 [speaker_0]
Um, so I think that's all I have. Bharath, do you have any questions for me?

00:39:23,150 --> 00:39:44,950 [speaker_1]
Okay. Like, um, what kind of... I, I, I read the, of course, the, the JD,
but I just want to know that what kind of team and project as you say that Teradata

00:39:45,330 --> 00:40:17,290 [speaker_0]
Yeah, it's a data engineer role and, um, you'll be doing, um, like, uh,
most of data engineering work like, uh, code refactoring from Teradata into Python

00:40:17,810 --> 00:40:27,070 [speaker_1]
Okay. All right. Cool. Of course. May I know another question? Like, uh, what
is the next process going to be here for you?

00:40:29,410 --> 00:40:29,870 [speaker_0]
I'm sorry?

00:40:30,470 --> 00:40:35,760 [speaker_1]
Like, may I know, like, what is going to be the next process from here? What is the next-

00:40:36,070 --> 00:40:45,710 [speaker_0]
Yeah, we will... So, so every team, every member should go through multiple, um, multiple like,
you know, meetings, total three rounds.

00:40:45,970 --> 00:40:46,450 [speaker_1]
Okay.

00:40:46,490 --> 00:41:03,710 [speaker_0]
So this is, um, this is just an initial round that I'm, I'm tracking. So next round
is going to be full technical, um, and, uh, with the hands-on, um, with hands-on on Python, SQL,

00:41:04,110 --> 00:41:04,330 [speaker_1]
Mm-hmm.

00:41:05,270 --> 00:41:18,370 [speaker_0]
Okay? So and after that it's going to be an hour-long, um, tech-complete technical discussion and,
uh, third round will be like, you know, with, uh, other technical manager and, uh, PM.

00:41:19,010 --> 00:41:30,370 [speaker_1]
Okay. Basically, it is a zeroth round or first round I was, I'm asking, like from the three rounds.
So it is a zero level round that we are taking right now and after

00:41:30,570 --> 00:41:31,819 [speaker_0]
Probably yes. Yes.

00:41:31,830 --> 00:41:34,310 [speaker_1]
Sure. Sure. Thanks. Thanks a lot. Thanks a lot.

00:41:35,450 --> 00:41:36,569 [speaker_0]
Sure. Thank you, Bharath.

00:41:37,150 --> 00:41:37,610 [speaker_1]
Thank you. Thank you.
