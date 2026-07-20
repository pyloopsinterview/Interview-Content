0:00: Good morning. 
 0:00: Nice to meet you. 
 0:01: Yeah. 
 0:04: good. 
 0:04: Well, maybe I'll give you a bit of the structure of how I like to do these, so maybe first quick intro. 
 0:11: I'll dive into maybe one project that you're particularly proud of, ask a few questions, and then leave the last five minutes for you to ask. 
 0:19: Sure, thanks so much. 
 0:22: I'll start with an intro. 
 0:23: My name is Mark. 
 0:24: I've been a researcher in AI for about 10 years. 
 0:27: I've been at fair for about 7 years. 
 0:30: the team's goal is to come up with new ways of training AI that don't exist today, And I work on computer use ents specifically, so teaching AI systems to use computers like humans. 
 0:43: Do you want to give me a little bit of an intro of yourself? 
 0:45: Sure, sure. 
 0:47: So hi, myself is Moli Mohan, and I'm 3 years of experience in Python development like full stack web applications, engineering, and like cloud ned software platform development and with extensive experience building like a scale. 
 1:01: web applications using Python backends and throughout my career I have designed and delivered like enterprise grade applications using Python, fast J AI like Flask, React, all those Docker communities using doc, post SQL cloud, GCP AWS sometimes I like back and forth on different projects and like, I enjoy like building high performance applications like designing reusable architectures and Developing data-driven systems that are, you know, both scalable and like user-friendly, like, most recently, I have worked with, Borcos Mercy Hill where I was a part of a team developing like secure drug-based, healthcare, like. 
 1:46: Applications used by like clinicals and operational teams. 
 1:50: One of my key projects like involve building a patient workflow like management platform, like using the, yeah, so, yeah, maybe before we get into that, just, yeah, just keep that, keep us on time because you're only 15 minutes, sure, maybe I'll, I'll ask you to pick one project, so it could be the project you were about to describe or it could be something else and then in 2 or 3 sentences, could you just give me a high level description of the project goal. 
 2:16: And what it looks like overall. 
 2:18: So like the platform streamlined patient scheduling, referrals, care coordinations, and like document management through an. 
 2:27: Intuitive data interface like while integrating with multiple internal healthcare systems through best APIs. 
 2:33: So yeah, back inside I designed a scalable Python services, developed rest APIs, optimized postre database performance like that and that's the whole overview of our like high level. 
 2:46: Overview of that and particularly like I have the chance to apply my web development like expertise to AI research also. 
 2:54: So yeah, so a few of the things I will do that so that's OK, great. 
 2:59: Maybe let's stick with this patient scheduling project specifically first. 
 3:03: so tell me about the who the, who your stakeholders or users were, and then who else was on the team developing this patient scheduling, platform. 
 3:14: Yeah, so the primary users were like clinicians, physicians, or my care coordinators, scheduling staff like that, so operational teams, and then the, premises. 
 3:25: So like each group had a different role, but like, they are all like worked on the same patient workflow. 
 3:32: like, for example, when a patient was referred for treatment, the scheduling team would, create up and manage like appointments. 
 3:40: Care coordinators were like would track the patient's progress and coordinate with different departments and also like clinical and physicians would, you know, give you the patient information and treatment details, and the operational team would handle document management and monitor the overall work. 
 3:58: OK, got it. 
 4:01: all right, great. 
 4:02: And then on the, on the team for the developers, was it just you or were there other developers? 
 4:07: There are, there were other developers. 
 4:09: OK. 
 4:09: And can you tell me a little bit about what they, how many, and then their areas of expert, you know, you have someone who's working on design, front end? 
 4:16: Were you back end, tell me a little bit about the responsibility and who else was on, There, there were like 667 members out there. 
 4:28: So there are some, one is the product owner, one is the business analyst, there are 2 backing guys, and there was one fronting guy, and other one is some something like a QA team from the QA team. 
 4:41: So that's how it's working. 
 4:43: OK, got it. 
 4:44: Makes sense. 
 4:45: Cool. 
 4:46: and then tell me a little bit about like exactly what you were in charge of and then. 
 4:51: the goal of the area that you were in charge of, and then some of the design or implementation choices that you made for that. 
 4:57: OK, OK, so yeah, of course, like as I told you about my project, so I'm mostly in charge of the packing side, like, responsible for the fast repair microservices, designing rest repairs, integrating with internal healthcare systems like writing business logics and, designing database changes and posters and, supporting the application and production. 
 5:18: So my goal was to build like Backing services that were like reliable and easy to maintain and responsive enough to, you know, support thousands of users without noticeable. 
 5:30: Got it. 
 5:31: OK, great. 
 5:32: and then tell me about the choices that you made and how you designed this back end and fresh press communication. 
 5:38: I heard Postress was, one of the choices. 
 5:41: So tell me a bit about maybe two or three of the big important design choices you made and why you made them. 
 5:46: OK, OK. 
 5:46: So, if we talk about the design choices, then like, first design, like what's using to, you know, microservices architecture using foster API like instead of like putting all the functionality into a single system, so. 
 5:58: Since the different modules are there because patient scheduling, referrals, care coordinations, like document management has their own different business logics, so separating, separating them like into services made the application like a bit easier to maintain, you know. 
 6:14: like, allow different parts of the system to evolve, like independently, one of the choices are like, rest APIs as a communication layer between front end and back end like this because we designed the APIs to be simple, like consistent, and, you know, resource based, so react front end could consume them easily, and like also like, whose grace up you're talking about, so like who's best database design and for your optimization, so you know. 
 6:43: The application grew, you know, because we have to think, now for the next 5 years or next some years, so some, screens needed to, you know, retrieve a large amount of data like patient and referee data. 
 6:56: So, you know, we carefully like design that. 
 6:58: Databases schema optimize SQL queries by like giving joints and using appropriate indexes on frequently search columns. 
 7:06: So yeah, like that. 
 7:07: OK, makes sense. 
 7:09: Great. 
 7:09: so you know that that sounds very reasonable. 
 7:12: Then tell me a little bit about how The feedback group worked with other stakeholders, so you know, you probably designed an initial version. 
 7:21: There was probably some feedback, some things that worked well, some things that didn't work well. 
 7:24: Tell me about what some of the feedback was and then how you worked with the stakeholders to incorporate that feedback. 
 7:30: Yeah, like, the property owner and the business analyst explained the business requirement first and the expected workflow, you know. 
 7:38: So as a backend developer, we discussed on the API design, database changes, and any technical considerations before, like starting development. 
 7:48: If something wasn't clear, we clarified it early to, you know, about the rework later and once the, once, once I just completed a feature, I first tested the APIs locally, then worked with the front end developer to, you know, make sure that integration worked as expected and front end team like, needed additional. 
 8:09: Fields and the like response or suggested changes to you know make the simpler so we discussed those changes and updated the API accordingly and after that like feature went to you know every teams for functional and integrate integration testing you know so if you have found any issues then we just have to find the root cause and solve the problem. 
 8:31: OK, sounds good. 
 8:33: Perfect. 
 8:33: and then. 
 8:35: What maybe the last question before I hand it off to you for questions is, what would you do differently? 
 8:41: What are some of the learnings from this project that you were, if you were to tackle similar projects in the future, you would keep an eye out, maybe two or three things that you would change or do differently in the future. 
 8:50: OK, so for that, like, definitely I would, I think like that, that, it was spending more time on a requirement clarification first at the very beginning because in a few cases the business workflow, you know, changed after development. 
 9:05: which had already like started because some edge cases weren't, you know, discussed early enough, so we have to handle those changes successfully. 
 9:14: But if, we had identified those, scenarios, like during the design phase, it would have reduced the reroute and saved the development time. 
 9:24: So that's what I think that's the most important thing one should do, if you, if they. 
 9:31: They are thinking long term that that's how some someone should think like getting feedback from the end users earlier so we should, you know, we usually like receive the feedback during sprint reviews, but if clinicals or clinicians, I would say, or scheduling staff had interacted with an early prototype even like sooner, so we should, we could like, we could have refined some workflows earlier in the development cycle. 
 9:59: So, and also like one of the changes like the third I like. 
 10:06: Adding more automated testing first of all, like, especially for API integrations or, we have, we, we have like good testing, but, but I think investing more in automated integration and regression tests like earlier like. 
 10:21: We would have like made releases even smoother and reduced the time spent on the manual verification as the application continued to go. 
 10:29: So yeah, so overall like this, yeah, I, I just like, this project like taught me to build a successful application isn't that just about writing good code you have to follow some of the, feedbacks and back and forth, communication so that you don't stuck somewhere or you don't have to rework. 
 10:48: Sounds good. 
 10:49: Perfect. 
 10:50: I, I wanna leave you time for questions. 
 10:52: I'll just start by saying, you know, a little bit about the role and then, answer any questions you may have. 
 10:58: So the high-level goal of the team that you'll be working on, you know, and I'm a part of it is to work with researchers to build out a really robust simulation engine for training AI systems to use computers like humans by looking at the screen and so on, so that will involve both. 
 11:18: You know, full stack web development style application building as well as kind of back end data processing and. 
 11:29: You know, kind of large scale data management, observability, these kinds of skills, and we primarily work in Python, so, you know, good Python skills are definitely, important. 
 11:42: Sure, those skills and, it's, it's, the team. 
 11:45: So yeah, thanks a lot for the explanation. 
 11:47: Then may I know like what are the next steps from here. 
 11:53: next steps would be 2 more rounds of interviews with, a few other members of the team that test both like technical ability and some of the skills we talked about around communication and design choices. 
 12:07: sure, yeah, OK, yeah, yeah. 
 12:11: Thank you. 
 12:12: Sure. 
 12:12: Any other questions? 
 12:13: No, OK, sounds good. 
 12:16: OK, well, I wish you the best. 
 12:17: Take care, Marli. 
 12:18: Thanks. 
 12:19: Have a nice day. 
 12:19: All right, bye, you too. 
