0:00: For right now, is it good? 
 0:06: Yeah, it's, it's, it's, it's terrible. 
 0:09: OK, I'm right now in the basement so maybe might be like. 
 0:18: Yeah. 
 0:22: And after the recording also just stay tuned. 
 0:24: I can detect a few more details from your flight, OK. 
 0:27: I'm sorry. 
 0:32: So Anil, just tell about you guys you know where you're from and tell about, tell us about your roles and responsibilities and what you're doing right now. 
 0:40: OK, so let me start with And I will cover all the things. 
 0:43: So hi, my name is Anil Anil Kumades hi. 
 0:46: And I have around like 1111 year experience and right now I'm in you know in Jersey, Jersey City in New York, New Jersey, and mainly I'm in a full site engineer and working on the solution architect as over the year I have worked enterprise application cloud-based big, back end system, large scale distributed application, although I work across like full stack, a big, big part of my career. 
 1:11: has been, you know, focused on the Python backend using fast API class and Django. 
 1:16: I spent a lot of time, you know, building less APIs, developing microsurfaces, troubleshooting, I can say production issues, improving system performance as well. 
 1:25: And currently I'm working on the healthcare platform. 
 1:27: We are, you know, in the 11 health, and basically our application is, you know, I can say is handle large volume of healthcare data. 
 1:35: And support millions of users and my day to day work, you know, including like developing microservices, maintaining existing applications, investigating any production issues, incident, and debugging APIs, failures as well, as well as handling my teams to like, like, you know, help, help them to, you know, troubleshoot their issues and yeah, that's, pretty much about my, my project. 
 2:03: OK, so basically list and, you know, there are, you know, two types of I can say Python major component which is, you know, we are using day to day work majorly, you know, list and topple I can say is mutable and on the other side is immutable, and I can say, you know, yeah, major differences in the, in the list and is, is the immutable and unmutable side. 
 2:27: So which one do you think is your memory is a guest on the memory. 
 2:36: Yeah, so I can say, you know, majorly I, I am thinking, doubles, you know, is, is taking, you know, much memory on, on a, I'm, I'm seeing on a daily basis, so yeah. 
 2:51: OK, Python decorators. 
 2:52: So Python generators, you know, majorly I can say, is, more on the, on the, I can say, modify existing behavioral function method which is like changing the actual code. 
 3:03: I think it's like the things like wrapping additional function around the existing function. 
 3:08: For example, if I want to add a, logging authentic. 
 3:11: ation performance tracking, section handling, multiple APIs instead of, you know, writing same code repeatedly. 
 3:17: So I can, you know, create a decorator to help to apply it whenever it's needed. 
 3:22: So it's kind of, we are reusing our code and we not, not want, not have to, you know, rewriting our code like again. 
 3:30: So that's the decoration. 
 3:36: Can you explain the. 
 3:37: Global individual, OK, GL. 
 3:38: So basically, you know, GI I can say is more on the mech mechanism that is in the C Python that is allowed only the threads to execute and Python bytecode at a time within a single process because of the GIL even if we create, you know, multiple threads, then don't, you know, truly run on the Python code. 
 4:00: Pary or multiple CP ports for the C2 intensive task, the threads, you know, take task, like in turn acquiring the log execution time. 
 4:09: And for example if you are, if you are doing having, calculation, heavy calculation data processing or image processing, so you know, it's basically trade usually want you know improve the performance because GIL become the bottleneck. 
 4:22: So higher, like, basically I, higher bound operations like API calls, database queries, these are, you know, major factor on the GIL side. 
 4:30: So yeah, that's my understanding. 
 4:33: Yeah, and, but I actually can you explain the main difference between Flask and Django, and, and like how do you decide whether to use Flask and Django for your microsoft? 
 4:44: OK, so over there I mean I feel that you know both I use like both the Flask and Django as a popular Python frameworks, but, they, you know, follow different kind of philosophies. 
 4:54: Fla flask, I think in the, in the other side is, you know, lightweight micro micro framework. 
 4:59: It has given, you know, developed a lot of. 
 5:00: Flexibility and let them choose a library architecture they want. 
 5:05: It's a great for API microservice application and where, you know, they want more control over the component being used. 
 5:13: And on the, on the other hand side, Django is, is a more full featured framework that has come from the many billions. 
 5:20: And capabilities such as like ORM authentication, as well as admin panel, session management, security features, so it basically follows the batteries, includes includes an approach which is, you know, helps team to develop application faster than standardized pattern. 
 5:36: So yeah, basically these are the two major difference. 
 5:44: OK, so dependency injection is when, whenever we are working on the, I can say, building a feature that basically allows us to provide required dependency to the function instead of creating manuals inside our function. 
 5:57: So in a simple term, if multiple APIs need something like database connection, authentication log. 
 6:05: or configuration settings on a on a service service object we can define it at once dependency and fast DP automatically inject whenever it is needed. 
 6:15: So basically this make code cleaner, more usable, easier to test, and easier to maintain as well. 
 6:21: So yeah, it's basically more helpful for whenever we are dealing with the code format. 
 6:27: So for example, scenario you are getting a lot of internal. 
 6:34: So what is your approach of doing if you're getting a lot of internal? 
 6:37: OK, so whenever I'm, you know, in this kind of situation, mainly I will, I will start, you know, seeing the large numbers of internal like 500 errors, right? 
 6:46: So my first step is not just, assume the course. 
 6:49: I will try to gather the facts. 
 6:51: Narrow down the scope of the issues. 
 6:54: First, I would check the monitoring dashboard and logs to understand when it's already started and how many users are affected due to that and whether this issue was isolated to the specific API or affecting multiple services. 
 7:09: Then I would, you know, review the application logs and status most of 500 errors. 
 7:15: You know, leaves, clues such as like exceptions, timeout error, database connection failures, null reference issues. 
 7:23: If the application is built using Macroservice, I would trace the request to across the new service to identify where this failure is occurring. 
 7:31: sometimes if API itself is not healthy, but downstream service, our third party API injecting a failing. 
 7:38: So next I would review. 
 7:39: Verify our database health. 
 7:41: I would check balance, activity, slow query, legs, and connection pool a lot stands as well. 
 7:47: So yeah, these are, you know, a couple of steps I will check. 
 7:49: And once I know, in the recent, deployment I have got this kind of situation, I would compare the changes and review the deployment logs and determine whether it's log rollback is necessary or not. 
 8:01: So that's my approach of, you know, handling this kind of situation. 
 8:05: And you said that you, you, I mean if you want to do so what are the different kind of tools you use for monitoring? 
 8:14: OK, so majorly if we are using AWS, so there's CloudWatch, which is, you know, give us, more, I can say extended feature of, you know, giving a log monitor and for the application log site, I. 
 8:27: You know, commonly, use, like, samplnk and, ELK stack Elastic Search and log stack and Kibana. 
 8:36: So these, you know, basically help us to search logs to identify exception and place request since many of the our services run on the AWS. 
 8:44: So I, I always use Cloudwatch extensively for monitoring logs. 
 8:49: So one of the main, services that you use, OK, so, if I'm talking about in a particular area of the services, majorly I have worked on, I can see, 1313 plus, you know, services in, you know, over the year. 
 9:05: I recently, I have recently, you know, in micro current project I have used, I can say, AWS lambda, EC2 ECS targets, and, or as well ATSized workload for the API management, we use API gateways to expose rest APIs and integrate them into the lambda backend service. 
 9:23: And for the storage side we use the S3 to document the storage file processing. 
 9:28: And for the database side I have used RDS, for with the Post and MySQL and Dynamo DB as well. 
 9:34: And for the messages side, so I use SQS. 
 9:43: Yeah, basically Azure is not, another, you know, cloud, cloud platform, just like Tidal was. 
 9:50: So yeah, I have your back on the Azure as well. 
 9:53: OK, and I just want to ask about the CICD. 
 9:57: You know, I got a pipeline first, but he got into AS in. 
 10:01: That's why I asked about the services. 
 10:02: So can you explain your CIC workflow later. 
 10:05: Yeah, yeah, sure. 
 10:06: So, basically, you know, as per my understanding, I have worked, I, I, I not just, in the CSED, setup side. 
 10:13: I, I also, you know, I handle the CSCD pipelines in the my major of the projects. 
 10:18: I follow them not, typically start with whenever developer push their code changes on the future branch in the GitHub. 
 10:24: I pull request was, you know, created, then where I will bend through the code. 
 10:28: Review and approval process before, you know, being merged in the deployment deployment branch. 
 10:33: Once the code was merged, the CI pipeline was automatically triggered during, during the CIE stage. 
 10:38: We perform code quality checks, using tools like SNAQ or linters, and we do unit testing and integration testing as well. 
 10:47: We use security independent civil liberty scan as well. 
 10:50: After the successful. 
 10:51: Validation. 
 10:51: The CIAD pipeline, deploy the application through the multiple environments such as like deployment, QA staging, pre-production, production. 
 10:59: These are a couple of, staging around environment we have used for the infrastructure deployment that we use telecom and in which as a core principle to provision, you know, manage, resources, cloud resources consistency across the different kind of environment. 
 11:14: So yeah, these are my experience, so far. 
 11:19: So thank you so much for answering these questions. 
 11:22: I'm talking we're recording right now, just stay tuned. 
 11:27: OK, so first what I'm gonna do is that I'm gonna send you the right address and give it to you. 
 11:33: Sorry, can you come go just. 
 11:35: I'm gonna send you the right to represent the email, OK. 
 11:40: Would you just, just one second, one second. 
 11:56: OK, I'm done about it. 
 12:02: I know one of the characters getting joined, so I'm just texting him, Please connect and join. 
 12:07: Yeah, so. 
 12:09: Wait, wait, I, so, oh my gosh, I didn't take your email. 
 12:13: I just read this. 
 12:15: I'm sorry. 
 12:17: Copy. 
 12:18: So I'm gonna give you also just for one day just for one day, just for one day, yeah, exactly that I can do that I can do. 
 12:29: What's the, what's the location you said? 
 12:32: OK, OK, OK, I'll try that on you right. 
 12:40: Yeah, OK, OK, yeah, I can do that. 
 12:43: OK, and your full name, or is there any elaboration? 
 12:49: No, no, it's not in Kumar Desari. 
 12:52: Oh, I I scared. 
 12:57: I know that's I need to put it like because this arcade works with the line so they always check with your ID yeah. 
 13:04: 618, OK. 
 13:08: OK, I have shared with the like to the present. 
 13:10: Can you, acknowledge it right now so we'll go. 
 13:15: let me check my, my different system right now in my using my current system. 
 13:24: we need to get more details from you. 
 13:27: OK, so what kind of. 
 13:31: Is there any specific details you want like you mention OK OK, so last four digits of my son like 2532. 
 13:46: 2532 and the date 19th July. 
 13:49: Thank you ma'am. 
 13:51: And I am sending you another email too because we we, you know, a copy of your GC copy and a copy, OK. 
 13:59: OK, I will attach those copies in my email. 
 14:02: I will do. 
 14:02: How, how, how soon you can reply me back? 
 14:08: I'm gonna present you very quick. 
 14:08: It will take, you know, 5 to 10 minutes. 
 14:11: I will do, you know, 5 to 10 minutes, right, sure, I, yeah, sure, sure, and I don't want they specifically require somebody in the healthcare space, and you are in the healthcare space too, yeah, right, right. 
 14:24: So, and, and one more thing since you being a GC, can you explain a little when did you come to how you got it. 
 14:30: yeah, because sometimes when I send a resume to the client, like just being a remote, they ask you, this guy is like, can you, can, can you like I can, OK, yeah, so basically, so basically in 2013 I came, you know, USA, by GC and obtained, you know, green card through the marriage. 
 14:49: So yeah, that's, you know, how I, 2013 you came to US in which in, in GC, DC, you know, m migration visa basically I can say. 
 15:01: OK, I'm talking, how can you how do you get GC like now being. 
 15:08: the marriage. 
 15:08: OK then. 
 15:11: Oh my. 
 15:14: No, basically my, my like wife is US citizen, so that's how, you know, I got, that's what, yeah, you're my spouse. 
 15:22: Yeah, OK, do you want? 
 15:23: Do you wanna marry in India? 
 15:25: Like, no, if you want, then you can do this. 
 15:27: Yeah, correct. 
 15:28: Basically I married in, not, not in India. 
 15:33: no, but the thing is, like, you know, they'll ask me, like, you know, what visa you went to? 
 15:37: Is it possible to go directly in GC? 
 15:39: Like, you know, how would you get your GC while being in India? 
 15:42: That's why, basically, basically I came you, I can say I came in you in the migration visa. 
 15:47: Then after that I got my GC. 
 15:50: So what is migration visa? 
 15:52: It's a migration visa, you know, status is DC DCCR 6. 
 15:58: OK, so you will be able to provide me the GC copy and deal copy, right? 
 16:01: Yeah, sure, so that I can come, yeah, so, so please help me with those like and then I'll drop your submission with right. 
 16:10: Oh, thank you so much. 
 16:12: Thank you. 
 16:13: And, and, and I, I mean like what is the main reason for you to change and why you're looking for a change? 
 16:17: OK, so basically my content is going to be amazing and mostly, you know, next, next, next Friday, so that's why. 
 16:24: OK. 
 16:25: Next Friday is your last working day, so you're working on a contract, with this client. 
 16:33: A cell, so who is your employer in between? 
 16:35: His direct employer basically. 
 16:38: It's 11 cents, which my client is 11 cents. 
 16:41: I mean, if you're a full-time employee, yeah, really I'm doing remote job, but my contract is going to extended, so that's why I, oh, I mean, you probably I can tell the client that you are, you are working as a full-time of the element sales, but your job is getting winded up. 
 16:56: No, no, basically my contract, I'm this contract based, but my contract is going like extended somehow like in the you're doing a contract directly with elemental, yeah, yeah, contact. 
 17:08: Oh, OK, OK, OK, not a good time. 
 17:10: OK, I'll, I'll put the reason like, you know, project winding up that is the best thing, otherwise they'll keep on digging that would be good. 
 17:17: No, no, I said the project is winding up, so it might get laid off, so. 
 17:22: That's why you're looking for a new job and it will, it will work. 
 17:27: OK, OK then, thank you, thank you so much, I'll wait for the two of your email replies, yeah, sure, thank you. 
