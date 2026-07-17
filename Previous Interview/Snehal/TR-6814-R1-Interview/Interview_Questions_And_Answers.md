0:02: Yes, Nathan. 
 0:03: Hi Prashan, good morning. 
 0:05: How are you? 
 0:07: I'm doing good. 
 0:08: Just give me a minute. 
 0:09: Sure. 
 0:33: Hi John. 
 0:34: Hey, good morning. 
 0:35: Good morning, John. 
 0:36: Good morning. 
 0:36: How are you? 
 0:37: I'm doing good. 
 0:38: How are you? 
 0:39: I'm also fine, thanks for asking. 
 0:41: OK. 
 0:43: Hey Prashan there, I see you there. 
 0:44: OK, thanks for joining. 
 0:45: I think I have some issue with my monitor somehow, but that's fine. 
 0:49: I'll take it from here. 
 0:51: yeah, thanks for joining, Sneaker. 
 0:54: so, OK, it looks like something is going on. 
 0:56: Give me a second, yeah, OK, let me move here. 
 1:05: OK Sorry about that. 
 1:24: OK. 
 1:28: OK, very good. 
 1:29: No, yeah. 
 1:32: So, Snell, yeah, I know, just a brief introduction, then we can get into more of the technical deep dive. 
 1:39: so we, at ABV, you know, it's a pharmaceutical company, when I see that your background is also in the kind of the medical field. 
 1:47: so yeah, at ABV as a pharmaceutical company, we, you know, make pharmaceutical products and we are all over the world, around 180 countries. 
 1:55: We are part of the manufacturing, operations and the IT team which supports the BA and the AI space. 
 2:02: So I, I, I own the platform which is predominantly AWS, and then we have other few flavors also known AWS ones, the homegrown ones, but, what we're looking for is, from an application standpoint, the AIBI space. 
 2:18: platform engineer who can deliver, build, and deliver the automation part of deployment, application deployment, building frameworks, you know, CICD pipelines and automation of the CICD pipeline, things like that. 
 2:32: So that's, that's the current role we are looking for, and we have, I have Prashan here. 
 2:37: He's, an associate with me for. 
 2:39: Long time now and he's the he's the prime hands on person as well as architect for the platform and he will he will be able to kind of take a deep dive into the technical part of the things but before going there if you you know Prashant I would, I would rather you introduce yourself and sneaker you can then if you can give us a brief intro of what is going on. 
 3:02: Yeah, sure. 
 3:03: Hey, myself, Prashan, so I work for platform engineering over here, for John, and, yeah, we, currently we are working on, you know, building next-gen infrastructure. 
 3:19: Based sort of Kernais, all of that stuff, but, we are, we are building an orchestration layer based on CRDs, all of that using coprogramming and, Python that, that is the complete text stack we are using right now. 
 3:37: yeah, then there is a lot, a lot of stuff and Kuberneticide and a lot of stuff are. 
 3:43: , STO mesh, and, so there are a lot, many things, even on the CIC we are using, centralized, GitHub, based, template actions, all of those things. 
 3:59: So yeah, that is it. 
 4:01: So, from my side, OK, yeah, and thanks John and for giving your brief introduction. 
 4:07: So let me introduce myself. 
 4:09: So yeah, this is me and Paella and I have around 12 years of experience in soft engineing. 
 4:13: And I would say over the last several years, my primary focus has been on pattern development, the platform engineering, cloud native applications, as well as distributed systems. 
 4:23: And now I'm working with the Franciscan Health as a lead pattern developer and engineering lead. 
 4:29: So here my main responsibility is as leading the, leading like the development of, an enterprise clinical AI platform. 
 4:37: I would say that has the doctors and, healthcare, health like healthcare providers quickly search the patient information. 
 4:45: They can generate their clinical, summaries and support the, decision making using genetic design. 
 4:52: And one of the key solutions I worked on was building a rag or retrieval argumented generation platform using the Python, fast API, Lang chain, as well as the fact databases and also the, large language models. 
 5:09: Basically, like whenever, user, like, ask the questions to our platform for the most, relevant clinical information from the electronic health records, physician. 
 5:23: And notes as well as the medical guidelines and then our system can provide the context of the LLM to jump it up secure and accurate responses and along with the application development, I also work extensively on the cloud side. 
 5:37: So I have like I would say hands-on experience with the AW services like EKAZC2 Lambda, Gateway. 
 5:46: SEODB. 
 5:47: So here I also build and deploy the centronized microsurfaces on Ubermates and also also automate the deployments using the GitH actions and OCD with GitOps and make sure like the applications are highly available, scalable and also easy to monitor and I would say like security has like also been a major part of my work so especially because, we are working in the healthcare domain and the healthcare, data is the thing like that is very crucial or sensitive. 
 6:20: So I, I implemented the OPTA 2.2 and, RBAC for the security purposes. 
 6:26: And I also work with the Northwestern Mutual Genetic where I involved in developing scalable background systems. 
 6:33: So I would say like, what I enjoy is solving complex engine problems, building scalable platforms from the ground up. 
 6:40: So yeah, that's a pretty about, pretty much about myself, what I did so far in my career. 
 6:45: So yeah. 
 6:47: So currently, are you working for Happy or I see you're with Fran Franciscan Health, right? 
 6:56: Yeah. 
 6:57: Snehal, is there any way you are, I mean, I, I hear it very feeble. 
 7:00: I can hear, but it's clear, but it's very low volume. 
 7:03: I don't understand if you feel the same way. 
 7:05: Is there any way you can, I don't know if it's a mic issue or, I, yeah, I had to kind of really listen in to understand what's going on, but I could hear. 
 7:14: Let me, let me check with my mic what is the problem with my mic. 
 7:18: OK. 
 7:19: If you want to use the headset, that's perfectly fine. 
 7:21: Go ahead, you know, if that helps with the volume. 
 7:23: Is it, is it, is it fine now? 
 7:25: Hello? 
 7:25: Is it fine now? 
 7:26: Better, yeah. 
 7:27: OK, got it. 
 7:28: Yeah. 
 7:28: OK. 
 7:31: Yeah, so person, do you want to get into, I know we, we have half an hour. 
 7:34: That's very limited, you know, depending on how it goes, we may get into another round, but, yeah, let's, let's, you know, take a deep dive into what we are looking for here. 
 7:43: Yeah, I think, what, at least what were you told, at what we are looking for. 
 7:47: Yeah, go ahead, Prasan. 
 7:49: Yeah, Shil, can you share your screen? 
 7:51: Sure. 
 8:03: Is it visible to you guys? 
 8:06: It's coming up, yep, yeah. 
 8:09: So can you click this link, whatever I give you, OK. 
 8:27: Yeah, so you, so can you Let me know what, can you read through the program and I Then just let me know. 
 8:39: Can you go out? 
 8:41: Give me a second. 
 8:42: Let me go up. 
 8:43: Mhm. 
 8:46: can you read that first, few lines, like, no, why are you going down? 
 8:52: Go the beginning in the, the, the comments. 
 8:56: Yeah, yeah, sure. 
 8:57: So basically, like, it's only like the above records has the clinical conversations, transcris them, and I need to generate some medically accurate summaries from them. 
 9:11: And here is Coder pad with the code, the system is running, which went from POC to a centime dollar value. 
 9:23: Yeah, and it went from the POC to a $70 million venue engine almost overnight as a found product market fit. 
 9:33: We are unable to keep up with the scale and system is crashing down. 
 9:39: We need to fix it before we lose the trust of the medical community and can never get it back. 
 9:45: Code exercise identify the permanent and security issues. 
 9:49: With this code, we use a collaborative efforts that they are able to identify potential resolutions, pay special attention to synchronous processes and data storage. 
 10:00: We do not need to write the code, so we could all come to comments. 
 10:05: OK, OK, OK. 
 10:08: Yeah. 
 10:10: Yeah, OK. 
 10:14: So yeah, so what, yeah, yeah, yeah, you, you can do it. 
 10:23: Yeah, you can start, explaining me what is the, what did you understand about the question here. 
 10:29: OK, OK, got it. 
 10:31: So like, as for my understanding what is like happening here, like from my understanding like the, like this is not like. 
 10:39: I have coding exercise like where you are expecting me to write new code. 
 10:43: So instead you are asking me to like review the existing implementation like senior engineer during a code review. 
 10:50: So like your scenario it means that the like the application started as a proof of concept, but now it's being used in production at a much larger scale and Since like it has like grown like rapidly, so the current implementation is like no longer able to handle the increased traffic, which is why the system is crashing. 
 11:17: So here my major responsibility is like is to analyze the code and identifying the bottleless and I need to explain like why they are like causing problems and suggest improvements rather than rewriting the entire code. 
 11:33: So, and also I think the, this problem of statement also, specifically asked me to pay attention to the, what is that synchronous processing and data storage so while reviewing the code. 
 11:49: So yeah, so yeah, that's, that's my understanding from like your, your like comments and all. 
 11:55: I hope my understanding is correct here. 
 11:59: But Yeah, partially, yes, OK, we can go through, with the program, yeah, OK, OK. 
 12:12: No, tell me, like, from the start, like what are the issues? 
 12:15: What is the performance issues in this program? 
 12:18: OK, OK. 
 12:20: But, let me, let me go through the first. 
 13:50: Thing on the line number 24 that is written the open. 
 13:53: API. 
 13:54: Here the issues that the API case is like hardcoded in the source code. 
 14:00: So, like, like if the code is pushed to get up or or like lead anyone can like misuse it so we can like fix it in the environment where the variables or in the AWSC data manager. 
 14:16: This is like my first observation. 
 14:20: Then Then like You like we have it done here the in the line number 26 we have the process audio and I think like this, this request I think is for the uploading the file and transcribe it in and it calls the in in the request. 
 14:43: So here I'm also seeing like an issue like, like I think that we like every user has to like wait for transcription and summarization. 
 14:52: Under the heavy loaded and get blocked so it can cause leading to a timeouts and crashes. 
 15:00: That's my observation here for this line. 
 15:03: And also the File path that shows the user ID and audio. 
 15:12: We also have issues like I think. 
 15:18: So what is the solution for the user ID? 
 15:24: What, what are you thinking of? 
 15:26: Why is the issue with the user ID? 
 15:29: OK, I think with the user ID. 
 15:37: OK. 
 15:38: I think the issue is I noticed that the, it is being used to construct the file back, but like, I don't see like where it's being defined or validated. 
 15:49: And this visible code, the user ID like like hasn't been like accepted from the authenticator user or the request or any session context. 
 16:00: And why do you, why, why do you think it is not, a valid user, valid authenticated user? 
 16:06: OK, because, I'm, because like, I think like, if, if, if we are like assuming the user ID is like coming from an authenticated user context, then that, that's fine. 
 16:19: Like, so my concern would be like we are like saving the file on the local file file system under time. 
 16:26: So. 
 16:27: In a production environment, especially if this application is running on multiple, Kuberne ports or the local so at the local food is, is not ideal because ile would not be shared across the instances and they can be lost if a pod restarts. 
 16:52: So that's my you can use PVCV right like why you lost. 
 16:56: because, yeah, because, like, I think like it is like I would say it is like actually backed by like a persistent volume claim, so then we like data like I would say that wouldn't be lost on a pot side, so the, so that concern doesn't apply in this environment. 
 17:15: I think my assumption here is like it is like based on the code alone like where I like couldn't you like see the Google its storage configuration even with a PVC I would still think like about whether it's the best choice for storing large audio files at scale. 
 17:32: So that's, that's my assumption here. 
 17:35: OK. 
 17:41: OK, move forward. 
 17:42: OK. 
 17:50: What was the first thing you told like prior to this one, I have told that there is a hard. 
 17:58: No, what is the issue of the line number 29? 
 18:04: OK, line number 20. 
 18:06: Line is there is no audio file. 
 18:10: OK. 
 18:10: OK. 
 18:12: so the basically line number is usually the audio file. 
 18:15: So the problem is that if, if the request doesn't contain audio file field, then the request files will immediately raise a key error before it no audio file check is ever executed. 
 18:27: That means like the validation is too late here. 
 18:30: That was, that was directly the No, what is that function doing? 
 18:37: OK. 
 18:38: OK. 
 18:39: So, basically, here. 
 18:46: What is that function doing and what is that supposed to you, you are supposed to do there? 
 18:50: What is this? 
 18:50: OK, so as per my understanding, I think we have the functions to the uploaded audio file on the on the server's local file system so it can be processed later. 
 19:04: It's no, that is on line number 33. 
 19:07: OK, OK. 
 19:08: But what is happening from line number 26 to line number 30? 
 19:13: OK. 
 19:14: Hm, OK, from line number 26 to 30, I think, From line here from 2:30 the code is like expecting the uploaded file from the incoming STTP request and on line 28. 
 19:33: I think it accesses the uploaded file request using the request file and it stores it in the in the audio file variable. 
 19:44: Then online 20, I think 29, it checks like whether the audio file is actually present in the request and this is actually a validation step to ensure the client has uploaded a file before the application continues processing. 
 20:00: And if the file is missing then then on 9:30 the function immediately returns an STTP 400 bad request response with an error message including that no audio file was provided. 
 20:12: So yeah, that's my understanding here. 
 20:15: What, what. 
 20:17: Go up on the top. 
 20:21: What is the first issue in this program? 
 20:23: OK, what is the position this book now? 
 20:28: Yes, by seeing at the court, what are you thinking? 
 20:31: Is this court reliable? 
 20:34: Is this court has any security or any issues, performance issues, or this court doesn't have any issues at all? 
 20:44: OK. 
 20:53: I think overall I would say the core is functionally right, but I wouldn't consider it like a production ready yet because I do see a few areas where reliability, security, and performance can be improved. 
 21:07: So, particularly from a security perspective, I think the biggest concern is the hard-coded open AI key, open API key here. 
 21:16: So what, what do you do for that one? 
 21:18: So what I will do for the security perspective, the open API issues, OK, OK. 
 21:26: So what I can do is, hmm, I think, I would like, definitely, definitely never hard code the, open it take in the source code. 
 21:37: Instead I would store it in a, secure secret management solution and if the application is running on AWS. 
 21:45: I would use the AWS C grade AWC. 
 21:49: How, how would you use AWS manager directly over here? 
 21:54: OK, OK. 
 21:55: So basically I would say I would like to use like I would like in that case I would store the open API key in the CS manager instead. 
 22:05: Of like putting in the application during the I understood that. 
 22:09: I understood like what you are telling, but why, why is the secret manager required here? 
 22:16: OK, so basically, the major concern of like using the secrets key managing here is, it would like basically retrieve the. 
 22:29: secret using the SDK and I think the application is the SDK you use. 
 22:36: What is the? 
 22:39: Is DK you lose? 
 22:40: OK, OK. 
 22:41: So let me, let me tell you the, I think, as for my understanding here, the main reason is that the, open API keys is that you are sensitive credential data. 
 22:50: So if it's hard coded in the, source. 
 22:55: That is absolutely, that is absolutely fine. 
 22:58: OK, I got that you are repeating the same thing, right? 
 23:02: I got like what is, what is the issue with the secret there. 
 23:06: I, 100% agree on that, but why do you want to use the SDK here? 
 23:14: SDK and what SDK? 
 23:14: OK, OK, OK. 
 23:16: So basically, I'm here using the SDK here because, if the application is already injecting the secret as an environment video, then I don't need SDK at all, but I can simply, simply, simply using it, using the, like a Python's, get environment. 
 23:34: So I would like to hear. 
 23:36: I would only use but the get environment is also again exposed to right hm. 
 23:44: The environment is also exposed. 
 23:48: OK. 
 23:49: So, because if you do OS. 
 23:53: get TNV, right? 
 23:55: That is what you are trying to tell, right? 
 23:59: So ways of gettingenV is also exposing a key on your file. 
 24:06: Like you're like, well you're like your family, your point is very very valid here but like the environment variables can also be exposed if someone has access to the host or container. 
 24:18: And in an enterprise production environment, I would avoid, I think storing the long-lived cigarettes directly in the environment very well. 
 24:27: So for this, I think I would prefer using a dedicated cigarette management solution. 
 24:31: Or where the application you keep the secret securely OK, I got it. 
 24:37: Like you can move on, so what is the major other issue in this program in this program, OK, If I talk about the the program is not big, right? 
 24:50: Like it is hardly 10 line score. 
 24:52: OK, I think so what is the, other major issue in this? 
 24:58: I think the, the next major issue I see is that the, entire work is synchronous ear, and I think the API, received the audio file, see if you then extended for the transcription. 
 25:12: Then it which which line number, OK. 
 25:26: And you are telling, you are not telling line number also, and there is no 510 to 5, 15 lines of code. 
 25:38: OK, so basically in the line number 3537 we have the open API. 
 25:43: Can you? 
 25:46: Yeah, yeah, from top to bottom. 
 25:47: Sure, sure. 
 25:48: So basically our code is here tells about like the the records clinical convention that is the coding. 
 25:57: No, no, no, I, I, I'm asking you. 
 26:00: Sure, sure. 
 26:01: Here we have written the, import open API, then import import import into you written the import Jason from class import class request. 
 26:11: Then we have the app that shows the class name. 
 26:15: Then we have written the open API. 
 26:17: open API. 
 26:18: EIP. 
 26:19: He is written the. 
 26:20: , the data that is 1234 and all and here we have the app work route that processes the audio, that process the audio, audio methods that post then we define the, process audio, then we have the audio file that shows the required files is audio and we have written the condition here that if the, if no audio file, then it returns the 400. 
 26:46: Then we try apply the dryca here that that shows the file part on the tamp user ID. 
 26:55: Then we have the audio. 
 26:57: wave. 
 26:57: Then we have the pass the audio file. 
 27:00: save as the file path. 
 27:02: Then we have written the width that control that it has the open file file path as the RB as then we have to find the transcript here that shows the open AI. 
 27:14: audio.transcribe this for minus one. 
 27:17: Then we have the I mean, I think, I got pretty much like what I need, So yeah, I think we are, good for now, but really a small solution for you, so I'm not sure like what other interviews you're giving. 
 27:39: my suggestion would be like whenever you give the other interviews, make sure you don't read what exactly they're on the AI, OK, so I can see like what you are telling, but don't do that because Really that is not a good thing, I hope you understand that, OK, because these are very simple basic programming and it's not even complicated, hardly 10 lines of code, OK. 
 28:08: hope you don't repeat that, but, see, this role really demands a lot of programming, OK. 
 28:17: and, from day one onwards, like teams, at least, someone who is working for John, they need to really be very good into the programming, OK, and, we are going to build Kuberne CRDs for the orchestration framework, OK. 
 28:37: And we, we have, we have like very complex and tight deadlines on like what we need to deliver. 
 28:46: OK. 
 28:47: I hope you understood that but overall it, it was nice talking to you, but my sincere suggestion would be like to be honest like when you're trying to do something because that, that will help for your career, OK. 
 29:07: I got it. 
