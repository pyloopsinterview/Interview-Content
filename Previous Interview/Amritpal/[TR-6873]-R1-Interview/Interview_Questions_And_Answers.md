0:00: Pretty good. 
 0:01: Nice to meet you. 
 0:02: I see you. 
 0:05: Yeah, so we've, we've looked over your resume and, thought that you might be a good candidate for a position that we have available. 
 0:12: I do have a couple of, housekeeping things that, that we gotta do right up front. 
 0:17: first of all, do you have a photo ID and if so, could you hold it up to the camera? 
 0:21: Yeah, I have. 
 0:22: Like, just give me a second, OK. 
 0:25: Sure. 
 0:38: it's visible. 
 0:43: OK. 
 0:46: All right. 
 0:46: Excellent. 
 0:47: Excellent. 
 0:48: And Yeah, yep, and also for all of our interviews, the interviewee is not allowed to use any outside assistance, no Google, no chat GPT or anybody in the corner telling you what to do or anything like that. 
 1:05: As long as you're OK with all of that, we can move forward with. 
 1:09: OK, very good. 
 1:10: All right, so first of all, I'll introduce myself. 
 1:15: My name is Tim McCabe, and, I've been with Guidehouse since October of 2025. 
 1:22: I'm a full stack developer, and I've been working, doing development for about 25 years, and I live in the Cincinnati area. 
 1:30: OK, So tell me a little bit about yourself. 
 1:34: Not, not the stuff on your resume, but just, you know, who are you? 
 1:38: yes, like I'm impulsing. 
 1:40: I've learned 12 years of experience in a software development, like a strong focus on like Python and AWSP's application. 
 1:47: And throughout my career, like, I worked on like designing, developing the enterprise applications using Python, Django, past API, JavaScript, and I'm like involving like the complete software development life cycle like from, understanding business requirements and, designing the solutions, like to development, deployment and the production support also, currently like I'm working as a like a principal Python developer with the discussion department, like. 
 2:15: Generally we are like we are modernizing the legacy healthcare platform into like the cloud native microservices architecture on AWS and before that like I worked across industries like the banking, healthcare, life sciences, retail, and the financial services and apart from that I also have good experience on the US like React or Ambulance. 
 2:38: That's pretty much all. 
 2:41: Very cool. 
 2:42: have you ever worked with you at all, the UJS? 
 2:45: yeah, yeah, a little bit. 
 2:48: Little bit, OK, yeah, like, but most of your work has been reactor angular, yeah, but like, I, in a couple of projects including like I work enhancing the maintaining the views front end like, approx 3 years, like, included the building and updating the, UI components, inte integrating them with the backend rest APIs, handling form validation, managing the application and like some fixing UI related issues. 
 3:16: OK, very cool. 
 3:17: And, you've got some experience with Django, I saw on your resume, And have you ever worked with Django Rest framework? 
 3:26: yeah, obviously, like, talking to her like, Django rest framework. 
 3:30: So yeah, like I used to build the restful APIs for like, front-end application and for the communication between the microservices and also, like I worked on creating, serializers, class-based views, and also the view sets, you can see router. 
 3:46: Authentication and authorizations pagings and some like API versions and like I mainly use the also like for authentication JWPB and rule-based access control to secure the APIs and also focus on like proper exception handling request validations, writing on unit tests, like to make sure the APIs are like reliable. 
 4:11: OK, how did you usually handle migrations in your Django apps? 
 4:17: basically for handling the migrations, like whenever like we made changes to the models, like we would generate the migration using the make migrations, review the migration file to make sure everything looks correct, and then apply it using the migrate, like for production environments we like, never apply the migrations directly like. 
 4:38: they were the part of like, the CRCD pipeline. 
 4:41: So, like after the code was, reviewed and the tested in the development and the QA, the migrations were like executed during, deployment in a controller manner, and like we can say for the largest schema changes like adding, new columns to the high volume table for like moving data, we planned them like carefully to minimize downtime if the data transformation was, was like required. 
 5:06: we created a separate data migrations and, validated everything like before, like, promoting the changes to the production and, in last slide we also took the database backups before the major releases and coordinated with the DevOps teams like whenever the migrations like involve the critical production data. 
 5:27: OK, so, and you, you've worked on teams, before with other developers, involved in the same code base. 
 5:34: OK, have you ever had a situation where there was a migration conflict, like two migrations with the same number? 
 5:42: OK, so how would you, could you walk me through, how you would handle that? 
 5:47: Let's say that, let's say that there's like a master branch and so you're creating your, Feature feature branch on the basis of this master branch and somebody else is also creating a feature branch on the basis of the same master branch and so you both create a migration and it has the same number and so he checks his in first and merges his in first. 
 6:08: How, how are you going to handle that? 
 6:10: Can you just kind of walk me through that? 
 6:11: Oh yeah, like these things happens multiple times like in the development phase like generally. 
 6:18: let's say like both of us like created a migration from like 005, so like we both ended up with the things of the 006. 
 6:26: So if the like other developers merge first, then I pulled the latest main branch, then I have two different like the, like the 006 migration files. 
 6:36: So like the first thing I do is read this or like we can say merge the latest main branch into the into my feature branch. 
 6:44: And then like I run the migrations locally and Django will detect that there are multiple leaf migrations and Django like creates a new merge migration, for example, we can say 007 and merge which tells the Django that both migrations would be considered valid before like moving forward and then like I test everything locally to make sure that the schema is correct and the application still works. 
 7:12: Once that verified, like I commit the merge migrations and raise my PR, and if both like migration are changing the same table of the same field, then like before creating the merge migrations I and I coordinate with the other developers to like make sure like with the. 
 7:30: we are like not introducing the conflict schema changes and we had agreed like on the final model, definition first like update the migration if needed and then proceed and Also, in general, like, I don't delete or rename migration files that have already been commit committed by the another, another developer. 
 7:49: I let the, like, Django manage the migration history and like you can say, use merge migrations whenever like possible. 
 7:59: OK, sounds good. 
 8:02: So, can you also maybe, tell me about some models that you've created in Django for some particular project? 
 8:11: what were some models that you had to create and why did you, why did you choose those models the way that you did? 
 8:16: Mhm. 
 8:17: Yeah, like in my current, project, like, with the discussion department, like we build a healthcare platform. 
 8:24: that manages the citizen and family services data. 
 8:28: Like I worked on the several Django model based on like the business requirements. 
 8:32: For example, like, like we had a, a patient model that stored the basic information like, you know, patient ID name, date of birth, contact details, and the status. 
 8:43: And we also had the case model like where like each case presented to the a healthcare service request or like. 
 8:50: benefit case. 
 8:51: so a patient could have like multiple cases, so there was like one too many relationship between patient and the case and another important model was like appointment, like. 
 9:03: Which is stored appointment details, like a date, provider locations, and the status. 
 9:09: So it was like linked to both the patient and the case and we also like had document models for like storing and like storing uploaded the files and supporting the information. 
 9:23: So like the actual files were stored in Amazon S3 like while the Django model stored the file path, document type, upload data and like the related patient or the case information and for like security we extended Django's authentication system like use the custom rules. 
 9:43: So, different users like caseworkers, supervisors, and administrators had like had different levels of access by like We can say creating these models like I, I, I also like added the appropriate relationships using the foreign key and 1 to 1 fields like we are needed and like it's applied the database indexes on like frequently and searchable fields and added model like validations and generate the migration for the the database changes. 
 10:17: OK, that, that sounds really good. 
 10:21: so, let me see here. 
 10:23: I have a few other questions for you, For, sometimes with, ORMs, object relational, mapping systems, there's a common problem that they have if you're, let's say that you wanna pull in a list of books and you have a book model and you also have an author model, and in your list of books that you wanna display to the user, you wanna also show the first and last name of the author. 
 10:52: so Django, if you're not careful with Django, it can, it can do a weird thing. 
 10:57: Do you, do you know what I'm talking about right now? 
 10:59: yeah, yeah, like, basically. 
 11:03: generally like in, in that type of situation, like, like I believe like you are referring to the N +1 query problem. 
 11:10: like for example, if I like, fetch a list of books and then access the book.author.name like inside a loop, so Django may like execute one query to like fetch all the books and then the additional query for like each author. 
 11:28: So if there Like we can say 100 books, so it could end up like executing 101 queries like which obviously like impact impacts performance and like to avoid that like I use the select related method like when dealing with the foreign key and 1 to 1 relationship like because like it performs an SQL join and retrieves related data in a single query. 
 11:55: And if it's like many to many or like a reverse foreign relationship, then I use prefetch related method like which like fetches the related objects separately, but efficiently and avoids those extra queries and like. 
 12:11: Whenever like I'm working on a list API or like pages that return like a lot of data, then I pay attention to the query optimization. 
 12:21: I usually check the general SQL or like using the Django debug toolbar like in a development or like the review query logs like. 
 12:30: To make sure like we are not working unnecessary database calls. 
 12:36: OK. 
 12:36: Yeah, very good, very good, full answer there. 
 12:39: Appreciate that. 
 12:41: OK, so I'm gonna, we're gonna do just a, a, a quick exercise here about rest, queries. 
 12:48: do you have a chat button up at the top of the team's app? 
 12:52: Oh, yeah, yeah. 
 12:55: Yeah, go ahead and click that. 
 12:56: I'm gonna, we're, we're gonna do a little bit of typing into the chat here. 
 13:00: , should I share my screen? 
 13:05: no, no need to, So I am going to. 
 13:12: I'm going to ask you some questions about rest interactions and the answers that I'm looking for are always going to be, first, what is the rest method that you would be using, and second, what is the URI that you would be using. 
 13:30: so we'll start off with the URI prefix. 
 13:33: can you see that in the chat there? 
 13:35: Yes. 
 13:37: OK, so that'll be the prefix to your, your API, So for the first question, let's say that you wanted to retrieve a list of users, all users. 
 13:51: What would be the rest method that you would be using and what would be the full URI that you would expect to use? 
 13:57: OK, go ahead and type it into the, go, go ahead and take down there yeah. 
 14:41: Have you seen? 
 14:43: Yes, yeah, and, OK, so that's great, I did have APIB one, Did you see the, the V1 in the in the path there? 
 14:56: Yes, yes. 
 14:58: Oh, like slash APS slash we even slash this is the URI, yes, yeah, I like, I'm gonna say. 
 15:05: That's, that's right. 
 15:06: Everything else is great. 
 15:08: OK, so now let's say that you wanted to retrieve a particular user and you know that the user ID is 21. 
 15:15: what would you expect the method to be and what would you expect the URI to be, Like, in, like, generally, like for reviving the specific user, like I would again use the get method because like we are only the reading data. 
 15:30: So method is get like the URLC and like slash APS slash U1 slash users 21. 
 15:36: So here like the 21 is the unique identifier like of the user. 
 15:39: So like we include it as like a path parameter in the endpoint. 
 15:44: OK, yep, perfect, and, OK, so let's say that you wanted to retrieve all users with the last name of, how do you say your last name, Molly, I'm gonna name Molly. 
 15:58: Mali is my last name. 
 15:59: Is that Molly? 
 16:01: Yeah, OK, so let's say that you wanted to retrieve a list of all users with the last name of Mahi. 
 16:07: what would be the method and what would be the URI? 
 16:10: And, could you go ahead and type them into the chat? 
 16:13: Sure. 
 16:18: It seems like we are still retrieving the data, so I, I like use the get method. 
 16:23: So basically, the the the URL is like slash API slash V1 slash users question mark last name goes to the mother. 
 16:36: It's like, or depending on the API's naming convention. 
 16:41: Yeah, yeah, like I generally, I generally prefer using and you were trying to use restful principles, yes, yes, generally I prefer query parameters for like, filtering resources since we are like not requesting a specific user by ID but filtering the user collection based on the last name. 
 17:11: That Yeah, great. 
 17:17: all right, so now, same, same kinds of answers. 
 17:20: What's the method and what's the URI if you wanted to update a particular user? 
 17:26: OK, basically for, like, to update the particular user, like if I want to update an existing user, I do the put method like, like if I'm replacing the entire resource or like the patch, like if I'm updating only the few fields. 
 17:45: OK, yeah, that sounds great. 
 17:47: Basically, the method is put. 
 17:51: And like, you are a little like flash GPS slash you wanna use a slash, 21, like if it was like a particular update like changing only the email address or a phone number, then I use the method patch. 
 18:07: OK, very, very good, and how about if you wanted to destroy, completely eliminate a user record, what would you expect the method and the URI to be, OK, I'm writing in chat. 
 18:36: Basically the method is delete. 
 18:38: OK, like since we are like deleting like specific users so we identify them the resources by its ID and the UR. 
 18:49: That, he said. 
 18:52: Perfect. 
 18:52: OK, last question. 
 18:54: you want to create a user. 
 18:56: What would be the method the URI? 
 18:59: Oh, same, basically for like creating, we use the method post, OK. 
 19:06: The user like details like the name, email, or other other requirements would be sent in the request body and the like server would create a new user return the created resources or its ID. 
 19:28: Yeah, sounds good. 
 19:29: All right. 
 19:30: Very perfect. 
 19:33: OK, So, just a, a couple of additional questions, And then I'll, and then I'll let you ask any questions that you have of me, in, in our last few minutes, So can you, can you tell me what the virtual dome is? 
 19:56: OK, basically, virtual DOM is like we can say a lightweight of like we can say basically it's a memory representation of actual DOM. 
 20:05: Like instead of updating the real browser DOM every time like something changes frameworks like view JS plus like update the virtual DOM. 
 20:13: And like it then compares a new virtual do with the like previous one like to figure out like exactly what changed and based on that comparison it updates only like the specific parts of the real DM that need to change like instead of re-rendering the entire page and like since manipulating the real DOM is like relatively expensive, this approach improves performance and makes UI updates like much more efficient. 
 20:45: OK, excellent. 
 20:48: so, I, I guess, do you have any questions for me that you'd like to, to know about, guidehouse, The way that we work or anything like that. 
 20:58: honestly, like, I don't. 
 21:01: Like, don't know much, like about, guidehouse like more, but, like, still like, in like in, in your side, like, can you please tell me more about the guidehouse and what are the things and also my, my question was like, what are like the biggest technical challenges like the team is currently working or like expecting this person person to like to, help to solve it. 
 21:32: OK, sure, so, Guidehouse is a really large company. 
 21:36: I think we have 19,000 employees, and, we handle a lot of government contracts. 
 21:44: that's not all that we do, but that's, that's one of the big things that we do, and so one of our primary contracts, is with the Small Business Administration with the federal government, OK. 
 22:00: so we are taking some legacy, software and we're, modernizing it. 
 22:06: I can't remember what it was written in before, but now we're writing it in Django and Vie. 
 22:14: we are hitting an Oracle database which is a little unusual for a Django app, But that's because that's what the SBA has. 
 22:22: That's what they wanna use, so that's what we're dealing with, And that's actually one of our, one of our challenges is the, the Oracle database, and hitting that with, with Django and, dealing with the legacy data. 
 22:38: we actually have a whole second app that, that we've created for the legacy portions of it and then we have modern portions of it in a different app and so these we talk to each other and it's complicated, Yeah, anyway, that's some of the stuff that we're doing right now. 
 22:54: Mhm. 
 22:54: That makes sense. 
 22:55: Like, legacy databases integration is like, we can say usually one of the more challenging parts of like the modernizing as well. 
 23:06: Yeah, definitely. 
 23:11: Well, do you have any other, any other questions? 
 23:14: like, apart from this one, is there any other like wrong? 
 23:19: I'm sorry, could you say that again? 
 23:20: like, apart from this technical round, is there any other one? 
 23:25: For this room. 
 23:25: Oh, yes, actually, so this is, this is just sort of an initial technical interview, basically just. 
 23:34: Just to make sure that you're a real candidate. 
 23:39: and we, we've had a lot of, a lot of people who are kind of just reading AI answers, and, we, we get a lot of junior candidates, and this is a senior level position, and so this is just kind of a sanity check to make sure that you're, you're real. 
 23:56: So, the, the next, assuming that you pass this and that everything goes well, there'll be a, a follow-up interview, also technical, probably two people will be talking with you and it'll probably be longer than this one, So. 
 24:13: Yeah, and, you got any other questions for me, or? 
 24:19: OK. 
 24:21: Well, so I guess next, I'll talk with, with my people and we'll get back with, with you and, and let you know, what happens next? 
 24:32: Sure, I hope it's positive. 
 24:36: I'm, yeah, I, I hope so too. 
 24:39: Thank you. 
 24:41: Nice meeting you. 
 24:42: Bye-bye. 
 24:42: Thanks for your time. 
 24:44: See you. 
