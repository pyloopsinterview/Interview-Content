0:01: Hey. 
 0:02: Hi, David. 
 0:03: How are you? 
 0:05: OK, sorry, I know we're starting a few minutes late here. 
 0:10: Unfortunately I have a hard stop at the end of this. 
 0:14: I am going to, we're, we're doing a DSA, so essentially I'm going to provide you, a problem set to solve, some data to expect, and we'll time box this and say we're going to finish the coding piece of this. 
 0:34: No later than 11:35. 
 0:37: That'll give us a few minutes to talk at the end, OK. 
 0:41: OK. 
 0:43: Give me 1 2nd here. 
 0:49: So basically we are going to be organizing a rail yard. 
 0:54: a rail yard. 
 0:57: Under real world circumstances, takes trains in, reorganizes cars into outgoing trains, and then sends the trains out. 
 1:07: To simplify this problem set, given our time constraints, we are going to keep the trains together and shift them out based on their departure time. 
 1:19: That way we don't block any trains at any point going in or out. 
 1:24: So we have two different types of data. 
 1:27: We have trains and we have tracks. 
 1:31: here's what a train, might look like. 
 1:37: And here is what a track might look like. 
 1:45: As you can see, the trains have a unique identifier. 
 1:48: It can be anything you want. 
 1:50: It has a length, just call it units. 
 1:53: I don't know if they're feet or what have you, we'll just say 2000 versus 5000. 
 2:01: status is less important. 
 2:02: We're not gonna do anything with status on this. 
 2:05: The departure time is really the key factor there. 
 2:08: With tracks, they have a physical, maximum length and a status of, whether they're in service. 
 2:19: So don't, you know, you, you just need to make sure that you don't send a train to a place that can't accept it, basically. 
 2:27: let's say there's an upper max of 30 tracks to keep it simple, and you can use any language you like. 
 2:36: You can use any IDE you like, just no AI, influence. 
 2:40: Yeah, should I, use like any online compiler. 
 2:46: yeah, that's fine again, as long as it's not providing more than auto complete, I don't care at the end of this, at the end of this, I do need an export of the code that you produced to just make sure it's something that can provide us a text file or what have you at the end of this so I can. 
 3:04: I can absorb that and give the hiring committee something. 
 3:08: Sure. 
 3:12: OK, go ahead and share your screen, please. 
 3:25: At this point, just making sure you don't lose track of time. 
 3:32: basically. 
 3:34: Like inside the signing fiction I first, the trains by departure time because the departure order is like primary, business requirements. 
 3:43: And next, like I filter out the tracks, that are like not in service. 
 3:47: And then for like each train I read through the available tracks and find the first track that is like not already used and has the sufficient capacity. 
 3:56: And once, like a match is found, like I told the assignment in my dictionary and not the track as occupied. 
 4:03: That's like no suitable that address like I add that train to an unassigned list and then finally I returned both the assignments and we stop the unassigned train. 
 4:18: Basically, for large scale systems like I would use the best fit allocation strategy instead of like the first we optimized, track utilization. 
 4:28: OK. 
 4:31: Complicated given the time constraints. 
 4:34: It's better to have something that works. 
 4:40: Retention issues like maybe from the compiler side. 
 4:45: Now, I can't see the invitation issue myself. 
 4:52: It takes you pretty close to the problem. 
 5:01: Algorithm rather than fighting with the index, I don't want you to lose the last 8 minutes. 
 5:11: What's that? 
 5:14: moment as well. 
 5:18: So for train trains. 
 5:23: Tracking the tracks. 
 5:28: Excuse me, so, Let's assume. 
 5:40: Check it back. 
 5:42: Let's assume we have to scale your solution, say 10,000 trains and 1000 tracks. 
 5:49: What would you change? 
 5:54: like, for the changing, changing perspective, like if, if we need to scale from a like number of like games 10,000s and like 1000 tracks, like my first focus would be reducing the complexity of the track assignment algorithm like for like a smaller data set. 
 6:14: The simple lean is can cross track is like acceptable. 
 6:22: However, like I'm sorry, I'm having trouble hearing you. 
 6:23: Now it's good. 
 6:25: Better, yes, yeah, like for a smaller data set, like a simple linear scan across the drag is acceptable. 
 6:33: However, like, at larger scale, repeatedly checking every track, like for every train would, like, become, inefficient. 
 6:40: So I would maintain the track, you know, like, minute order like by the earliest track available time and for like each incoming train, I would like, only compare against the track that becomes available the earliest. 
 6:55: And if the track is free before the train arrives, like I can reuse it. 
 6:59: Otherwise, like, I, I allocate a new track. 
 7:03: So basically, this reduced the assignment operations from potentially, like go like the number of tracks, for the train of like all of, the log number of tracks. 
 7:17: Got it. 
 7:18: What is the time complexity now? 
 7:22: basically, now the time complexity is like, oh, like there is like 0 and of log in like where n is like the number of things and like so yeah, basically all of like and login. 
 7:40: The time complex. 
 7:42: OK, and where would it be if they made that change? 
 7:47: Or like I think. 
 7:52: before the thing, if, if, like I was scanning every track for like each train, the complexity would like be over and, I need to k like where N is the number of trains and k is the number of tracks. 
 8:04: After the introducing the minute to track, the earliest available track, each assignment becomes O of lock key instead of OFK. 
 8:12: So processing all trains becomes like O and lock key, including the initial sorting hit. 
 8:17: The overall complexity becomes like. 
 8:19: Of analog m plus analog key, so which simplifies to like all of an analog n. 
 8:27: OK, very good. 
 8:31: Let's see here. 
 8:33: Track goes offline midday. 
 8:35: Which trains do you reassign? 
 8:37: How do you How do you reassign the work? 
 8:44: Or like a family law. 
 8:47: Generally, so the system designer operations thinking like basically I use like if a track goes offline in the middle of the day, like the first thing I would do is like identify all the trains that are currently assigned to that track and determine the status. 
 9:03: Any train that is like already departed or in the actively using the track. 
 9:08: would be handled according to the operations contracts, but for the future scheduling, that have not yet arrived. 
 9:16: I would mark them as like needing reassignment. 
 9:19: So how would you determine the changed between, you know, just so you would know that the track went offline or it was on my previous. 
 9:32: Like I would maintain the like tracks assignment as and the track status as for part of the like system state. 
 9:39: Every track would have the status such as like available occupied or offline like when a track goes offline that the state team would donate anyway. 
 9:48: So the scheduler would then look up all the future training assignments associated with that track by like comparing the previous state and the new state. 
 9:57: I can identify exactly like which fields are like impacted. 
 10:03: OK. 
 10:07: So you're you're sorting the trains based on departure time, which is correct, but you're doing it once, if you had to reassign trains, how would you manage that process, ensuring that they ended up, you know. 
 10:26: Not blocked at that point. 
 10:30: You sorted once initially the frames needed to be reassigned later, like, like basically if the schedule is static, starting once is enough. 
 10:40: Like, however, if. 
 10:41: I, can go offline and the training needs to be reassigned dynamically. 
 10:45: Like I would not rely on the, one-time shot. 
 10:48: Like instead, I would, maintain the upcoming trains, you know, like priority you order by the departure time and that way, like when I track, becomes unavailable, I can remove only the affected trains and put them back into the queue and. 
 11:03: The prior you automatically keeps the drain order so I don't, don't need to solve the entire data set again and I simply reinsert the impacted drains and then run the allocation logic against the remaining, available tracks. 
 11:21: Very good. 
 11:23: I wanna give you an opportunity to ask questions to me. 
 11:28: I've only been at the railroad for about 3 months, so I don't have a long tenure to lean on, but I'm happy to answer any questions about the organization, the people, technology, anything like that, but I can't. 
 11:44: there are some question like, what are the, like the biggest technical challenges the team is like currently facing with this, like. 
 11:53: On the technical aspects. 
 11:58: So the biggest technical challenge right now is the fact that we're in the middle of a big technology, upgrade, you know, we're, we're going from a very old stack to something more modern and in doing so, you know, we're, we're dealing with growing pains in terms of migration, headaches, and, you know, building out a platform that meets everybody's needs, you know, it's it. 
 12:25: It's Greenfield and at the same time, we're still trying to keep the trains running. 
 12:31: So that it, it's an interesting combination of the two, OK. 
 12:38: but I've enjoyed the challenges that I've faced at the real world, you know, it's, it's really interesting stuff. 
 12:45: The people are top notch, and that's. 
 12:48: You know, even coming from Salesforce, I, I would say they're on par easily. 
 12:57: Overall, I, I would have no, hesitation to rejoin if I were to make the same decision today. 
 13:06: OK. 
 13:10: let's see here. 
 13:14: I'm on the infrastructure side, so obviously my job is different than yours would be, so that your mileage may vary, of course, different organizations, but, that's been my experience. 
 13:35: is there anything else, that I can help you with? 
 13:38: No, no, not yet. 
 13:42: OK. 
 13:44: can you make sure I get a copy of your code? 
 13:46: Yeah, sure. 
 13:49: The easiest way to do it is just to save it as a file and then attach the file and chat. 
 13:54: That way we maintain all of your indentation and all of that correctly. 
 14:00: Yeah, sure. 
 14:08: OK. 
 14:21: Thank you very much. 
 14:23: It was a pleasure meeting you, and I wish you the best in your interviews. 
 14:27: Let me just make sure that I can read this file that I downloaded, and if I can, I'm gonna give you a few extra minutes to rest before your next round, and I know this is stressful. 
 14:38: We've all been through it. 
 14:40: Yeah, Shawn Davis. 
 14:44: Oh Got it. 
 14:50: OK, thank you so much, and again, it was a pleasure meeting you. 
 14:54: Best of luck. 
 14:55: Thank you. 
 14:56: Bye-bye. 
 14:57: Thanks. 
