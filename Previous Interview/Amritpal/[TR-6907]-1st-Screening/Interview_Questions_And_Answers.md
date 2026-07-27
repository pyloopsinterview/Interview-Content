0:00: Hi Shrikhan. 
 0:02: Hi Shabom. 
 0:02: How are you? 
 0:06: Hi, I'm good. 
 0:07: How are you? 
 0:08: Fine. 
 0:08: How are you guys? 
 0:09: are you there? 
 0:12: Thank you so much for joining the call again and sorry for the inconvenience. 
 0:18: I can't you there. 
 0:36: He can continue if he is not needed. 
 0:40: He is the one who will. 
 0:42: Interviewing. 
 0:44: I'm that I'm just the host, yeah, he's here now. 
 0:47: So I'm gonna meet Mr. 
 0:48: Shrikant. 
 0:49: He's the one who will talk to you and screen your profile. 
 0:53: So he's a technical screener. 
 0:55: So yeah, Shrikha, please go ahead. 
 0:58: Yeah thanks. 
 0:59: Hi Shikan. 
 1:00: Hey, I'm with. 
 1:01: How are you? 
 1:03: How are you doing? 
 1:06: your voice is a little bit low, yeah, am I audible now, right now. 
 1:12: yes, a lot better. 
 1:15: OK, so let's start with your introduction. 
 1:17: Can you briefly explain about the technologies that you have worked on and your work experience? 
 1:22: Sure, sure, thanks a lot. 
 1:23: So hi, Shek can't. 
 1:25: I'm myself I'm just passing, and I have, 13 years of experience almost on in software development with like majority of my career focused on like. 
 1:34: Python back in development like cloud, with like cloud native application architecture and fullt development on AWS like throughout my career I have designed like delivered scalable enterprise applications like. 
 1:51: Using Python fast API, best APIs, Docker, AWS, microservices on based on microservices, and like also worked with the DevOps teams like DevOps automation part and also like. 
 2:06: While like, leading development teams, like and working like, directly with business stakeholders to, you know, deliver the cloud-based solutions, so I have extensive experience like designing and deploying like cloud infrastructure using like you know with, cloud formation and one of my like Relevant projects was, was with, currently I'm with the Wisconsin Department of Health Services. 
 2:31: So, like, here I'm, I'm just working on, like, I have served as a lead partner for start developer on a like a statewide healthcare data modernization initiative and our team like developed our cloud native platform to, you know, automate the, A citizen eligibility verification, you know, so like pro provider data processing is there and like family relationship matching across like, multiple healthcare systems like that, and I have led the, design and development of the fast API based microservices, like exposing like, secure S APIs directed with, OIDC authentication also like, enabling the, seamless integration with the, like internal healthcare applications, you know, and external state systems also, and, and like I have designed the EWS infrastructure using like cloud formation deploying applications on, PCRs with like do containers while like leveraging RDS posters for the transactional data and like S3 for the, you know, secure document, storage so like that. 
 3:40: That I have like work on and yeah also like recently I have worked with like landing to build like AI powered capabilities like integrating large LLMs for you know intelligent document processing and like contactual search so yeah that's my experience and the work I have done. 
 3:59: OK. 
 4:00: So do you have experience in guiding a team or leading a team? 
 4:05: So how many years of experience? 
 4:07: It's been 5 to 6 years, from the last company to this, like, I'm, I'm doing that. 
 4:14: OK. 
 4:15: Got it. 
 4:17: So how do you provide security for your AP accounts? 
 4:20: OK, so we can apply a few of the implementations first. 
 4:24: If I talk about the security point of view, then like they are authenticated, like through our identity provider which, which issue them access to and like. 
 4:35: an ID token also like, every API request, includes the access token and the authorization, header, bear a token and, API, middle where, you know, like, validates the token before like processing the request and checking it's, like, signature or like expiration or like issuer or like the audience like if the token is like invalid or expired then that request is is rejected or with the you know 401 unauthorized responseible like that also like old based access control level implemented so yeah also like we can we we also can enable logging and monitoring to clog watch apply input validation. 
 5:21: OK, so what do you mean by role-based authentication? 
 5:24: So rule-based authentication, I understand like, for each and every person, it's, which, available that's present in the, our system like, if I talk about the rules like admin, manager, employees, so like that, we can provide the that after, user is authenticated, the system checks what, what that user is allowed to do based on their rules like that that's what we can say we'll be. 
 5:50: OK, got it. 
 5:52: So do you have experience in building the pipelines or doctor images? 
 5:56: Of course, of course I have that. 
 5:59: OK, so can you explain, maybe the steps? 
 6:01: How do you do that? 
 6:03: Maybe CHC pipeline. 
 6:04: How do you do that? 
 6:05: OK, OK. 
 6:06: So if I talk about the next steps, so like, first of all, like, a developer creates a future branch, first of all, like implements the changes that raise the request and GitHub. 
 6:18: then before merging those another developer or tech, leads, going to review that code, then we can like merge that code and after the full request is approved, the, like, merge is going to be, it is going to merge in the main branch and it did have actions automatically triggves those, CI pipeline and after that, that first stages like I would say full quality and validation like that if all check pass like pipeline vents and documents using the applications doco file. 
 6:47: And like like the image the images like includes the application code and Python dependencies and runtime contribution and next the dock images like tagged with the you know builds version or comment ID and push to our contain history such as ECR EW so like that and finally after like deployment that we monitor the application like using log watch and Whether logs or CPU memory utilization we can check an application matrix like that so that's how the process can work. 
 7:24: OK. 
 7:26: Got it. 
 7:26: So what are the Python libraries that you have used, maybe for A or non-A work? 
 7:33: OK. 
 7:34: if I talk about the Python libraries, like, morning I work is, we are using from, I mean, from so much time, but, like for back end and web web development, I primarily use the Fasterpay for STPI parentic for the request validation and data models also like, SQL for SQLLK result. 
 7:54: For the ORM and like unicorn for the like ASGI server and like also like if I have to like data process then we can use the pandas and Numpi very well that to work very handy and also like plotly is for the visualization like that and if I talk about anything you're looking for these are the major libraries that. 
 8:23: OK. 
 8:25: Got it. 
 8:27: So do you have experience in improving any performance related, I mean, in APIs? 
 8:34: Yeah, yeah, of course, like, performance, if I have to like, improve the performance, like, the first thing I would, definitely check the bottleneck using like identify, try to identify the bottlenecks using, logs on the cloud box and like then I found the IPI was making like, repetitive database queries and like some queries that were just not, you know, optimized sometimes so we happen to. 
 8:59: Performance like by added appropriate database indexes like or maybe sometimes reduces the unnecessary joins or like that and loading to you know like you we can use the SQL I mean like load eager like SQL can easily eager to you know loading to avoid the and plus one query problems. 
 9:23: These are the major things I would say like I have done or there are so many things we can do from the court to the department so many things, on the performance. 
 9:34: OK, so what are decorators in Python? 
 9:37: OK, so decorators in Python are just, like, you can say like piece of code or like, Python, like it's a way of to modify or like, Exchange the behavior of a function. 
 9:51: So like you know or or like method without changing it's it's so that is the let's say very I underlying thing if we talk about the that is. 
 10:03: -huh. 
 10:05: OK, got it. 
 10:08: Shiva, are you there? 
 10:12: Yes, ID, OK. 
 10:20: Yeah, OK, OK, Amrit, thank you so much for joining the call. 
 10:23: You cleared this screening room. 
 10:25: I'll let you know the, I'll submit your profile and let you know the further updates. 
 10:30: OK. 
 10:30: May I know if you, like, when can I get the, I mean, back from you, Your voice is breaking. 
 10:37: Yeah, I just want to ask, like, when for the next round, when can hear when I can hear from the back today I'll submit a profile and hopefully this week we will get an update. 
 10:49: So once I'll get an update, I'll let you know the same. 
 10:53: There will be a 2 to 3 round of interview process. 
 10:56: First would be with Capco and the other two would be with client. 
 11:03: OK, OK, got it. 
 11:03: OK, that's, that's, that's OK, OK, yeah, thank you. 
 11:07: Thanks, thanks for joining the call. 
 11:08: Thank you. 
 11:08: Bye. 
 11:09: Thanks. 
 11:09: Bye bye. 
 11:12: Maybe they'll. 
