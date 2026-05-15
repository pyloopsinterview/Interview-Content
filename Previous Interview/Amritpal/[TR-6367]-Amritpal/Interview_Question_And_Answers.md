(Transcribed by UniScribe (https://www.uniscribe.co). Upgrade to remove this message.)

How are you? I'm good, I'm good sir. How about you? Fine. Can you please turn on the video? Yeah, yeah, it's on. Yeah, it's great to meet you officially. How's it going sir? How's it going at the event? Completely fine. How are you? I'm good, I'm good. So, I believe you have gone through the job description and everything and you have an idea about the client as well. Sure, sure. I have an idea, yeah.

Yeah, so it is with our client Huntington Bank. It is a financial client and usually they are repeated in Columbus, Ohio. Fortunately, you know, it is a remote position for you. There were like four openings for this particular position. Two we have scored and eight of you was on last Wednesday. So we got two delusions and two more delusions are left. So it is a remote position. So...

Just wanted to ask a couple of things sir. They have seen your metrics and everything. So just let me see. So can you please confirm your last 4 SSN it is 2054 right? No no no. 2055. Is that fine? It's 2055. Okay. Exactly. 2055. Okay. Okay. I have just sent a reminder you are available at Q2C for a video call as well. And you are available for a virtual interview right?

So tomorrow and day after tomorrow? Usually they do update on Wednesday though I'm hoping I can get you an interview slot by next Wednesday. So that's the thing. We'll keep you posted on the next pages. So I was going through your resume so there were like couple of things I wanted to rectify about. So can you walk me through your first 30 days when you joined the project at

I'm Mr. Manik Bhurjan. Where you dropped into the existing enterprise architecture exactly, what steps do you take to understand how the data flows, where you write your first line of code and all? Okay, okay, you ask a very critical question, I think. First line of code is, I don't remember exactly, but you can understand, like, let's mean it's 2022, but if I talk about, like, in there, like,

I mean pretty large enterprise environment is there so with multiple interconnected systems, microservices is there so during my first 30 days like my primary focus was to you know understand the architecture, business workflows or operational dependencies before making any

code level changes. So that is the case basically there for the first 30 days. You don't work from the day one or you know KT sessions. So I connected with the QA teams, DevOps teams, product owners and after that, yeah, so that is the case. So what about the systematic approaches you took and data tracing, how all of that stuff happened?

What? Data tracing? Yeah, how the data tracing happened, like what was the APA gate we worked with and what was the systematic approach we took to actually hand out the things.

Sure, got it. So like since it was a distributed multi-services architecture, so data tracing and systematic troubleshooting were very important because requests were flowing through multiple services, Kafka topics, APIs, downstream systems. So typically the approach we followed like was end-to-end

request tracing and starting from the API gateway layer all the way to the decking processing and downstream integration we were primarily using AWS API gateway in front of Python fast API services and some internal services were also routed through

English controller in Kubernetes environments. So for tracing and monitoring we use Datadog, AWS X-Ray, CloudWatch logs. So these are the things. So actually the thing is the hiring manager explicitly mentioned that they are needing someone who can work in a job-adjusted environment. So in previous role

Exactly, how did you use your Python API to communicate with the Java backend? What specific technical challenges did you face in the data between the two?

Okay, okay, so you're looking for a Java JSON environment. Yeah, so I have worked on Java JSON environment of course. It's a part of the, it's a very wide system as I say like it's a, so in my previous project also like even though my primary development work was on Python, but like environment itself was very mixed like enterprise heavy and like several existing Java based systems already in place. So like

Python fast API services interacted with the Java Wiccan applications mainly through REST APIs, Kafka Waze, E-Winz communication and shared database in some cases also there. Scheduled file processing workflows are there. If I give a few examples like the pricing or order validation workflows that we developed in Python had to exchange data with the legacy Java services responsible for the inventory management.

So compliance check also there. So they are, I mean, connecting and exchanging the data through the legacy Java services. So these are the main cases and if I have to like tell more, so like there was a like, like,

Like if I talk about the flow, then like a request came through the AWS API gateway, then routed to Python fast API services. And depending on the business flow, we either like invoke Java based rest endpoints directly or like published Kafka events that were consumed by Java downstream, like

services and one of the major challenges was also like maintaining the consistent like data contracts between Python and Java systems because both ecosystems handle serialization, validation and data typing differently. So these are the cases.

like to solve that we standardize the json payload like contracts using the open API specification and schema validation also so we also implemented a strict request and response validation at the API layer so these are the I mean major things that we have done to you know communicate to java and python together

Okay, let me tell you about the most painful fail batch job or second work you like in AFL or GUN which was your cross-polling, right? You had to cover two pre-cently. How did you isolate the group boss? How did you fix it?

So if I talk about like that, so there are so many troubleshooting going on like the workflow was like responsible for the processing large batches of order and pricing records coming from the multiple upstream systems. So the orchestration was also handled through Airflow and like internally the workflow triggered several Python services, Kafka events, database updates,

So one day, like the business team reported that a significant number of orders were stuck in a pending state and downstream person went processing for the part of the batch. So the first thing I did like was isolate like where exactly the workflow was failing instead of assuming the entire pipeline was broken

So I just, I mean, see that and after that, I started from the airflow DAG execution logs and identified that one of the downstream tasks was like taking unusually long and eventually like timing is going out. So then I

the workflow step by step using AFO task logs, Datadog monitoring dashboards, and CloudWatch logs, Kafka consumer lag matrix. So, initially it looked like it's an infrastructure issue because ECS task were scaling correctly and CPU and memory uses were also stable.

So, then I started validating the actual data being processed and noticed that a specific subset of the required had, you know, malformed and pricing attributes coming from the upstream legacy systems. So, the tricky part was to, that the retries were like failing completely, that were partially processing. So, to isolate the root cause, I traced one failed transaction end-to-end using correlation IDs and

and the API logs and to fix it we implement additional schema validation defensive handling in the Python consumer services to invalid records like redirected to dead letter queue. So these are the, I mean, the problem and solutions we have implemented. Okay, so how much backend Python you are doing and how much production issues you are looking for? So Mr. Fay, what would you like to know? Okay, okay. If I talk about the backend...

Python so I would say like percentage wise it's 70 to 80 percent I would say like a percent of them has been it's one fourth back in Python development and remaining 20 to 30 percent you can say has been on the production support so troubleshooting operational support activities like on the on the like back inside on the Python

designing them, developing REST APIs using Fasten and FastAPI, implementing business logic, database interactions, performance optimization. So, these are the things and on the production side also, if I say like API failures, workflow issues. So, production settings are quite tricky or stressful, but

field, schedule, jobs, file processing problems. So, a typical production issue usually involves analyzing logs through Datadog, CloudWatch. I'm very comfortable working in environments like development, production, and machine learning. I see. So, how have you been fixing batch files and batch files and all?

okay if I talk about the batch files as I say that like troubleshooting like fixing batch process and should use jobs in a moment like batch jobs were mainly used for the like

reconciliation pricing synchronization and compliance validation so some workflows were orchestrated through airflow while others were scheduled through drone based jobs and even triggered pipelines so first like i would identify like where the failure occurred like whether it was during file injection data transformation or API communication is called i mean

problem is there with API communication or Kafka or database whatever the problem is I first analyze them then I would analyze logs and from Airflow then then like

common issue we face from Malfound input like input files or unexpected data coming from upstream system. So missing fields and correct delimiters. So these are the things so in those cases I use SQL queries, log tracing to validate the affected records. So these are the, I mean, Just wanted to know, I know it is approximately 6 to 7 hours of drive from your location to Columbus for I/O.

So just wanted to know one thing, in that route is remote, so that one is there a possibility can you do a face to face sound if they decided to call you and they want to decide to decide to go in that direction? It's not possible for me quite like I can't surely say that from now on yeah that is a case. I see and now what about if they decided to get you for that, are you willing to go

But due to a full time employment after 9-12 months of contract, so are you willing to go into date direction or what's the thing? Sorry, like you are asking after the 9-12 months I can be on full time right? That's what he is asking. Can you be a full time employee for until then? Sure, sure, no problem. It's absolutely fine for me. Okay, okay. Just a quick hi to you. I will be arranging you with my business partner. He will be there. He has a position with you. It depends on his mood.

So it depends, it will be either having a virtual conversation on the telephone or he will go very heavily on technical side. He will go very very deep technical, he will be asking questions and all. So he needs more of the hands-on experience which you have. So I am just giving you a heads up, so you can go through it and you know you can

You can articulate your thoughts accordingly so you will have a better idea, better chance to present your country to him and the client. And for the interviews, I would say like, on next Wednesday there is a possibility there will be like, I can get you an interview shot. It will be for like 20-25 minutes, that's it. But the technical pre-screening call, that is very important. We have to get you through the technical call.

And the interview is like, it's okay, that in order, crazy, but the technical thing is, please stay in court with my wisdom, that is the one. So, we have already closed two positions, two more openings are there, I'm hoping I can get you in, so there's that. Later on the line, they will be, they wanted to group big on this project, so there will be like four more openings for this particular same position. Hmm.

So, if you have somewhere in mind, any of your friends, that would be great. If you can refer it to me and I can see if they can be a good match, and I can get them in, that would be great. If not, then I will arrange your body.

I understand Sachin, I mean your inputs but I just want to request you from the very beginning of the starting of anything like please don't waste my time if any like asking for the last time like for the on-site face-to-face round because as I am very comfortable

saying that it's a remote thing and we have talked earlier also so these are the things because 5-6 hours distance is there to travel and it's not possible going to be possible for me so that is the reason so that's why I will say that I just wanted to have a clarity because both of the interviews were virtual so I just wanted to have a clarity because if they decided to go in that direction although it is a

remote position or remote position you know there will not be any face to face talks right and you are already like 6 and a half hours away from Columbus Ohio you are in Laurel right so definitely it will not you know there will not be any face to face interviews for you I just wanted to give you an answer that's it so wish you luck I will

That's why we should check first with the manager and anyone you want. Yeah, definitely. I got your back. I got your back. So do you have a deal copy right now? Right now? I have to check. Yeah, I can just send you right now. Yeah. Can you give me? Can you please show me that would be great. Yeah, yeah, yeah. Please show me that would be great. Yeah. I just need your photo ID. That's it. Just give me a minute. I'm just...

But if I get a baby, can I bend it?

(Transcribed by UniScribe (https://www.uniscribe.co). Upgrade to remove this message.)
