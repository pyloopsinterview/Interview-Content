0:00: , it's good. 
 0:01: How about you? 
 0:05: it's fine. 
 0:07: Sorry, I'm kind of a little out of it. 
 0:09: I had to put my dog down last night and I'm waking up at the last moment and we could reschedule this, so bear with me. 
 0:18: OK So where are you located? 
 0:22: like, basically I'm in, Missouri, O' Fallon. 
 0:27: OK. 
 0:30: Oh I'm gonna turn off my camera. 
 0:35: I'm sorry for my Non-professional, look. 
 0:42: I just woke up. 
 0:46: if it's OK, I'm gonna turn off my camera and just wake up. 
 0:51: Oh All right, so the pattern for this interview is I like to keep things simple and conversational. 
 1:03: you will have to write some code, but the objective of writing the code is not to have you build a solution that runs on an ID or any of that stuff, right? 
 1:17: the objective of this is to basically, see what your problem solving, skills are, and how do you go about like basically planning and executing a requirement and what coding practices are. 
 1:39: so feel free to use an online IDE or whatever ID you, you use, My only ask is a couple of things is. 
 1:52: at the end of the Call, I would request you to upload whatever you have written as an evidence for our hiring committee, and the second is, I would really appreciate if you don't use AI for at least for this round, Feel free to choose, like, if you want to look up Google, do whatever you want to like, you know, figure out something, that's fine. 
 2:19: Now, that said, BSF heavily encourages AI to go and use it, right? 
 2:27: So we are supporting AI as agentic development experiences for all our developers. 
 2:34: So if you do want to use AI just let me know and share your screen so I can see how you're doing engineering or something, right. 
 2:46: I'm gonna paste the problem here, like in chat. 
 2:51: Yeah, yeah. 
 3:03: Should I explain my approach? 
 3:06: Yeah, just share your ID and the overall thing is we want to spend a little bit of time on how you're designing the system. 
 3:15: And like, I want to see what the entity relation models are, and then we can write, dive down into defining the data models or data classes so you can kind of walk me through how you would design the system. 
 3:31: Or implement the system. 
 3:36: I first identify the core business entities and the relationship, because like that drives the overall system design, OK. 
 3:44: And for like for this container tracking system, I would start with 5 primary entities like the like an entity model we have the container, yard, load, train, and the like the movement event. 
 3:59: So basically the relationship is like, fairly straightforward. 
 4:03: One yard contains multiple lots and one lot contains many containers and, like a containers can move between lots, yards, and trains, OK. 
 4:12: So instead of like storing locations updates, Directly on the container record, like I would maintain a movement event history and like derive the current location from the last event, OK? 
 4:26: And basically, the movement even becomes the most important entity because it it like captures every state transitions. 
 4:35: And we have the thing. 
 4:40: location modeling for like a scalability add abstract location into the common model instead of. 
 4:47: Hard coding yard and a lot of references everywhere like I create the location entity, OK? 
 4:52: And also like we are handling the misplaced containers like. 
 4:57: when, like a container is like scanned, the system compares like expected locations and actual location. 
 5:03: If they don't match, I create a misplacement event. 
 5:07: So that even trigger like, even trigger notifications and the operations work flow. 
 5:13: So I would never silently correct the data because operational teams like need visibility into those, exceptions. 
 5:20: And also. 
 5:22: The handling container container movement like I treat every movement as in like immutable events and or like for example like in event one container arrives at like yard a lot 5 even to like Container loaded onto the train T 100 or like the event is like container uploaded at the RB lot term. 
 5:47: So the latest event like derives current location and the event history provides the complete audit ability and the system components like at a high level like I would separate the system into container service. 
 6:03: Yeah, management service, movement tracking service, notification service, or the reporting service and all movement would like generate even that flow through and consumergra location indexes, our dashboards, consumer availability system and the operations alerts. 
 6:20: And like for the like database design like for transactional consistencies like I use post cases as well like for like high volume tracking and the historical analytics like movement even like can be streamed into S3 and and carried through the athena or like the snowflake. 
 6:39: So basically like if BNSF stands from like 1 yard to the 100 yards, the design remains unchanged because locations are like. 
 6:48: A radical and the movements are like event driven. 
 6:51: So the Only thing that goes is the data volume like which can be. 
 6:57: Handled through the partitioning movement even by yard, or reason or the deed. 
 7:06: OK, that sounds good. 
 7:08: And your approach and the way you're thinking about the core infrastructure is also good. 
 7:12: I like that you're thinking about scalability, event-driven application like functional programming. 
 7:20: could you do me a favor and start writing this up, like your ERD that you mentioned. 
 7:28: how your data models would look like. 
 7:31: Yeah, sure. 
 7:45: And you to find me some properties or attributes, that's fine with me. 
 7:49: don't worry about it, yeah. 
 7:52: Mistake. 
 7:58: I was curious what happened. 
 8:00: I'll by me like, like I, I reloaded, so that's why. 
 8:07: Its functions, but let's go quick, real quick, what, what is the object level hierarchy here, who is the parent level here. 
 8:21: OK, basically, for like, like the object level hierarchy, it is like we can say. 
 8:36: Like. 
 8:37: It is like For like, basically for production system, I would like to extend this design by introducing the movement even like every container movement like. 
 8:47: Would generate an inimitable events like for auditing and the tracking and I would like also support multiple yards by like like at the yard registry and the possible things like the basically the top level parents is like yard management system because it's responsible for like managing the multiple yards. 
 9:06: Under that, like we have yards. 
 9:08: Each yard contains multiple, like as I told you earlier, multiple lots, and each lot contains multiple locations. 
 9:15: The location is like. 
 9:16: Is the leaf node because it is like the actual physical storage positions. 
 9:24: OK. 
 9:26: you mentioned. 
 9:28: Los And you mentioned yard management. 
 9:31: Can we define those classes first? 
 9:34: OK, like for defining, the yard, lords and the like yard management, basically, at this point, like, like the yard management system is like the parent object responsible for like you can say managing multiple yards, and each yard represent the physical facility and contains the multiple lots for now like I'm storing yards in our dictionary like for like. 
 9:59: Yeah, I do allow the like walk and look up. 
 10:06: OK, But if you read the problem statement, it says, and that's what I'm trying to get you towards, like, I want to understand. 
 10:18: Like you have your data models, right? 
 10:20: So what is the top level parent? 
 10:23: What is the child of that, and what are the children down to its absolute needs, right? 
 10:30: So you have to find a container, you've defined a location, you've defined a yard. 
 10:36: you mentioned yard management, so there should be another class object for that. 
 10:42: And you mentioned. 
 10:45: movements, so that should be another class as well, correct, correct. 
 10:50: Yeah, so define those classes first. 
 10:52: I wanna see the full class definitions first before we implement functionality. 
 10:57: OK, sure. 
 10:58: Like for the, like the class perspective, like, generally, like it is like, like, first, there are like classes we have the like yard management systems, yard law. 
 11:13: Locations container and like also like on the movement basically the physical hierarchy is like the yard management system, yard load, and the location. 
 11:22: Location is like the leaf node because like it is the actual storage position containers are like the business entities that get assigned to locations. 
 11:32: Moment is like the separate entity, that track container transfers between the locations. 
 11:37: So like, yeah, and for like. 
 11:42: And the things, basically we have, this is like exactly, what the things like we are generally I was focus, focusing on the object modeling and the hierarchy but not, not the methods like assigned containers yet. 
 11:56: OK, so in this design you mentioned your location is the lease node. 
 12:03: how would that work with the project like the system design? 
 12:09: Like if you read the first line, it says, or the second line, it says. 
 12:15: Yards have locations that customer either pick up or drop off containers. 
 12:20: Yeah, like I consider location the leaf node because like it's the smallest physical storage like until, like where a container can decide ultimately every container like must be assigned to the specific location and all such as like the pickups and the movement is all down to a location and also, When I'm like customer wants to find the container, like container, the lookup ultimately. 
 12:48: Sorry, didn't mean to interrupt you. 
 12:50: you said pick up. 
 12:52: Of a container. 
 12:57: then how can the location be a lymph node? 
 13:03: Like, if you were to schedule a pickup or a drop off for a container. 
 13:09: The container should be the leaf node, shouldn't it be? 
 13:13: Oh yeah, like, basically, that's a good point. 
 13:15: Like I may have used the term leave note too loosely. 
 13:18: Like location is like the lowest level, like in the physical story hierarchy, but like it's not necessarily the end of the object relationship because like the location can contain a container like, we have like. 
 13:32: We are like the modeling the actual business domain like container would be a truly entity because like it is like the object we are like ultimately tracking a location is like rela really like a storage resource that reference a container like when we perform pickup we are like removing the container from the location, which means like the workflow continues beyond the locations. 
 13:57: Right, so your true leaf in your object hierarchy model here is container, correct? 
 14:03: OK. 
 14:03: Can you go to the top of the pile and write that out? 
 14:06: Like just write the class name, arrow, class name, and write the whole tree. 
 14:13: Yeah, sure. 
 14:17: Onto my laptop, it's in refresh it. 
 14:23: Go to history and open up that last tab that you opened up. 
 14:26: I think you have some kind of malware. 
 14:34: The object hierarchy. 
 14:38: So I'm trying to understand what's your viable model. 
 14:43: So Like what depends on what Down to your absolute li. 
 14:56: basically. 
 14:59: like, like for like the viable model, like, generally, first one, like the simple, the top level objective, as I told you, the yard management system like it manages one or like more yards. 
 15:13: Each yard contains multiple locations and a location, also, also can contain, contain a container, and movement is like separate entity that tracks container transitions between locations. 
 15:25: But yeah, let's try that, yeah. 
 15:34: Yeah, I can hear you. 
 15:35: Sorry, I was making some notes. 
 15:38: cool, yeah, that looks correct. 
 15:41: Now let's start off since container is your lowest level leaf. 
 15:47: Let's start off with container. 
 15:49: don't worry about the inn describers. 
 15:52: just write, what the attributes are and show me what kind of, Functions would you add to it? 
 16:03: Yeah, sure. 
 16:09: OK. 
 16:16: Cool. 
 16:17: I like that you have that arrival time in there, Now think about that. 
 16:25: Like, don't worry about owner. 
 16:27: We can, like, we're not doing owner tracking or any of that. 
 16:31: That wasn't defined in the requirement, but like I mean. 
 16:36: I'm glad that you're thinking on that kind of time stuff for like user-based allocation and stuff. 
 16:42: That's good. 
 16:44: tell me. 
 16:46: About arrival time, why did you And this is an open-ended question, right? 
 16:53: Like, and we can iterate on this, you mentioned that you would have a separate kind of class to track movement right between like a a container going from one location to another or one yard to another, How would arrival time help you here? 
 17:19: Shouldn't it be a little bit more generic? 
 17:21: Like it could be a departure time too, right? 
 17:23: Basically, like I, I did arrival time because it can influence locations, allocations, and operational decisions. 
 17:31: For example, like if the yard is like nearing capacity, we, we may want to place containers that are like. 
 17:38: Expected to leave sooner and more like accessible locations while like container expected to like stay longer can be placed deeper in the yards and arrival time like also helps like with auditing and the tracking like we can calculate well time like which tell us like how long a container has been like sitting in the yard. 
 17:59: So that's useful for like operational reporting and the identify the bottlenecks and after that like for like the. 
 18:09: We can say between the container going from like one location to another. 
 18:12: So it is like, if like I'm introducing the separate movement class, then the arrival time probably does not belong on the container itself. 
 18:22: Like it is really A timestamp associated with the movement or like location like assignment event and like a container like can have multiple movements through, throughout its life cycle. 
 18:36: And like if I store arrival time on the container, I only capture one point in time. 
 18:43: And by stolen timestamp on movement, reports like I can track the complete history of like where the container has been and like when it arrived or like departed from like each location. 
 18:55: OK, I understand. 
 18:58: in that case, let's move on to the next object model. 
 19:02: I, I like what I'm seeing here. 
 19:04: So you have an assigned location, an update location, a pickup, and get current location. 
 19:12: cool. 
 19:14: for each of the functions, could you define what the arguments would be? 
 19:20: like for the argument's perspective, like, generally, I think. 
 19:28: It's like more. 
 19:30: Like, it's like, should I write? 
 19:35: Yeah, OK. 
 19:40: Yeah, sure. 
 19:41: The difference between assigned location and update location. 
 19:45: like, basically, the assigned location is like assign the container to a location. 
 19:51: the location is move the container to another location. 
 19:54: Like for argument like views, location, object, in the. 
 20:01: Right. 
 20:04: But your function signature is just. 
 20:07: Like setting the current location to location, both of them are identical, and there is no container stuff in there. 
 20:19: Oh, OK. 
 20:22: like how is assigned location in your current implementation functionally different from update location? 
 20:27: They, they have the exact same, function signature. 
 20:32: They take the same arguments and they're doing the same thing. 
 20:39: OK Like the sign location and update location are like. 
 20:45: Functionally identical, they both like take a location object and like ultimately set the container current locations. 
 20:52: The only difference is semantic and one is like intended for like initial placement and other for subsequent moves, but that not reflected in either the signature or the implementation. 
 21:04: Correct, because you mentioned container, and there is nothing about containers here. 
 21:13: Needs to change here. 
 21:15: You're on the right path. 
 21:17: I can see how you're thinking. 
 21:19: So let's say somebody gives you a container and you want to kind of put it into a location. 
 21:25: Out of the four functions that you've written, what would be your order of operations be? 
 21:30: What would you first go to see, can you place this container in this location or not? 
 21:37: Yeah, should I write the code for this first, then I explain it? 
 21:45: sure, yeah. 
 21:49: Location would help you marry them together because they're kind of linked. 
 21:53: Go for it. 
 21:53: I don't, I don't wanna talk about that. 
 21:55: So if you wanna kind of skeleton out location first, that's also fine. 
 21:59: Generally if somebody like gives me a container and ask me to like place it in a location, the first thing, like I do is check the weather location is available, and if it is like then I perform the assignment looking at the current 4 methods. 
 22:15: Like I actually don't have the methods that supports that validation with. 
 22:20: suggest my UPS like in like I, I, I also, I need either the location that is available method or like the yards can assign method before calling, any assignment operations. 
 22:37: OK. 
 22:40: OK, so for that you need the location model then. 
 22:44: So let's define that location model and define its helper functions first, like, in order for you to kind of do what you're saying. 
 22:56: OK. 
 23:06: returned self dark container is none. 
 23:10: OK, good. 
 23:11: Assigned container, OK. 
 23:15: Remove container And So this has been the assumption that each lot can have only one container, which is fine for the objective of our. 
 23:34: Solution. 
 23:34: OK. 
 23:35: Cool. 
 23:37: now, tell me, how would this Work with your location model. 
 23:44: Like, let's go back to that, Like shouldn't update location. 
 23:54: And Can you just pull up. 
 24:06: update location and assign location, How would the overall flow work for him? 
 24:16: OK, like for the overall, like the flow or like the location generally? 
 24:23: It was the, like now that like we have defined the location model, like I think there is like some overlap in magic container method. 
 24:32: So the like generally the flow would be checked if the target location is like available using the location or is available method and assign the container to the location using loc location or assigned container. 
 24:46: And like and then update the container state or like the location reference if we are like storing a one and looking, looking at it now like the assigned location and the update location on the container don't like. 
 25:01: Add much value because the location already manages an occupancy. 
 25:07: the only difference with assign and update is like the business context. 
 25:10: Like assigned location container is like not currently stored anywhere and update location like container is like already assigned and it being moved. 
 25:20: OK, so like I would probably not keep both methods on the container. 
 25:25: So, that is why I want, yeah, so that is why I will want you to write the location model because you would see that that state would lift to a different model. 
 25:35: And after introducing the location model, like I think assignment and the movement becomes workflow, involving both container and the location. 
 25:43: So that makes the yard is like a natural place to coordinate them and the container mainly hold the state while location manages occupancy. 
 25:53: Correct. 
 25:55: Correct. 
 25:58: OK, so. 
 26:04: Let me check something. 
 26:05: I'm, I'm sorry, I'm taking some notes, so bear with me. 
 26:12: Hm OK, one last question you had mentioned because we are coming up on time, I wanna leave a few minutes for you to ask questions. 
 26:27: You had mentioned immutable objects, just for state tracking and historical data analytics at the beginning of our conversation now. 
 26:40: Of the 4 models or 5 data models that you've defined here, which one would be the immutable class? 
 26:49: OK. 
 26:51: which one is like immutable? 
 26:53: Basically, I guess I'm not guess like of the models like we have discussed so far like container location, lot and yard like I would not make any of them immutable. 
 27:07: Because they all represent current district that changes over like the time and containers changes changes status location locations become occupied all the weekend and they are like continuously update as like the operations. 
 27:24: like, the class I would make immutable is the movement or even record that captures like the historical actions, OK, and OK, so that was where my question lies. 
 27:38: You mentioned movement and assignment or what we can call that interchangeably. 
 27:47: shouldn't that be immutable. 
 27:55: For that, yes, like, exactly, like I agree, like every, every model movement or like the assignment as like the separate entity rather than a like method call, then that entry should be immutable initially, like I was thinking of like assignment and the movement as operations on the yard, but if we represent them as like the records in the system, they like become historical events and should not change once created. 
 28:24: And once a movement has occurred, I would not update that record. 
 28:30: And if the container moves again, like I'd create a new movement record that like preserves the audit trial and make historical analysis reliable and so like I would classify my models into like generally two categories like mutable state models like container location, lot or yard and new immutable event models like assignment assignment movement, pickup, and arrival event so. 
 28:54: Generally, the mutable models tell, tell me the current state of the yard, and while the mutable models tell me like how the system like reach that state. 
 29:06: Yep Hello? 
 29:28: Yep, I'm here. 
 29:29: I'm taking some notes. 
 29:30: Sorry. 
 29:32: could you do me a favor? 
 29:33: Could you save this file and upload it to the Zoom Zoom chat. 
 29:48: OK. 
 29:50: Awesome, thank you. 
 30:00: You, what questions do you have for me now it's your turn to ask me questions. 
 30:16: like, not very much, generally like, like, what are like the, and reason project, like what are like the biggest technical challenges like the team is like currently working on? 
 30:34: A lot. 
 30:37: so think of like BNSF being a 100 year old company, right? 
 30:43: over the past 50 years, BNSF has been investing on lots of like All their technology is outsourced. 
 30:53: So, companies like Tech Mahendra or TCS or Accenture or IBM, they have built most of their legacy solutions. 
 31:02: And that accumulates to a culminative of like, let's say billions of dollars of maintenance cost every year. 
 31:12: And the NSF right now, what we are doing right now is modernizing it, which means we are getting rid of all our contractors and all our outsource vendor, projects, and we are building everything in-house, right? 
 31:30: so. 
 31:31: Like think of it from the world of Like we can't get rid of these existing software, right? 
 31:38: So there is a lot of freight management and train movement, intellectual capital that cannot be rewritten overnight because they are being written on mainframe and stuff, like very old stuff. 
 31:52: So those will kind of move in and then get modernized slowly into something like Rust or C++ or other stuff. 
 32:02: but there's also things like IOT, right? 
 32:05: Like they, they learn machine learning software on these trains to see whether they're performing well, are they going to get derailed their own prediction models. 
 32:15: So there's machine learning, there's legacy applications, plus the NSF is building their own private cloud, which means like, We are building 2 data centers, and we are building a mini AWS and a mini Azure internally here. 
 32:33: So we are basically building a completely cloud native experience for the entire company with our own intellectual solution, right? 
 32:43: Like we're not going to a cloud provider. 
 32:47: so, There's a lot of technical challenges and we have a shortage of people. 
 32:52: That's why BMSF has been doing a lot of hiring. 
 32:56: there is. 
 32:59: And that's why these interviews are very open-ended. 
 33:03: we don't quite know where we would fit you because there's so much to do here. 
 33:09: there is infrastructure, there is cloud, there is, containerization, Kubernetes, there is, migration from legacy systems to on-prem systems. 
 33:23: there is Windows apps, iOS apps, Android apps, customer stuff, there's websites. 
 33:30: There's a whole lot of stuff going on here. 
 33:33: so I can't really tell you what business problems we are trying to solve. 
 33:38: For me, I'm like, I work as part of the infrastructure team. 
 33:43: So I'm building, basically, I lead a team where I build Kuberani's cluster fleets. 
 33:50: so we manage like a cloud nated posture that we provide as a I like infrastructure as a service and platform as a service feature to other developers where they can build and deploy them. 
 34:04: Sure. 
 34:08: Any other questions? 
 34:11: OK, cool. 
 34:13: All right, Mike, it was a pleasure. 
 34:15: Thank you for your time. 
 34:16: Have a good rest of your day, yep. 
