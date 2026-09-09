0:00: Please let me know. 
 0:04: yes, more than you are, yeah, yeah, OK, a few things, while you're on this call, do not switch that from this one to any other call is prompted, so it might show up in the report. 
 0:14: Secondly, I will be adding just 4 quick questions, like 4 to 5 quick questions, and we'll be requesting you to share the screen, and then you can take it forward from there, OK. 
 0:24: OK. 
 1:06: taking time. 
 1:07: I don't know. 
 1:08: Is it visible now, Trisha? 
 1:11: Yes, it is. 
 1:12: So you can go to task number one. 
 1:14: A scenario is given over there. 
 1:16: Just prepare your answer first. 
 1:17: Once you are ready to answer it, click on start recording. 
 1:54: OK. 
 1:57: only you can keep that video tab down. 
 1:59: I will be switching off my car and, OK. 
 2:03: OK, OK. 
 2:04: That's that. 
 2:06: OK. 
 2:06: Yeah. 
 2:07: Is that fine? 
 2:11: If it's fine, you can start or I will keep myself on mute, OK, so and that's like. 
 2:19: Yeah, so I would pro I like, I would profile and validate like each incoming source like against an expected schema for for fields where the structure can legitimately evolve and I would define our schema evolution strategy. 
 2:35: Like for example, allowing new malleable columns handling compatible data type changes explicitly like rejecting. 
 2:47: Like rejecting the incompatible changes rather than silently converting them and like I would avoid relying heavily on the schema insurance for like watching backing data and like because it was like it can introduce inconsistent types of impact the impact the performance here. 
 3:06: So for the actual injection. 
 3:08: I would use an explicit passport and pass passpar schema read the data in controlled, way. 
 3:15: I would, let them perform the lightweight validation as early as possible here and think like, required fields, data types, ranges, the valid ranges, and business rules, and I would like a, a source identifier and And injection or batch IDs so that every record can be traced back to, back to its origin. 
 3:37: For corrupt record, I would not feel like the entire pipeline. 
 3:40: I would separate valid and invalid records and valid records, continue to like normal transformation and processing path while invalid records go into the, quarantine or dead litter location with the original record. 
 3:55: And this gives us like ability to investigate and reprocess them later. 
 4:01: And for, from a performance perspective here, I would like to make sure these validation and distributed spark transformation rather than Python side loops of all UDF wherever possible. 
 4:14: So yeah, that's what I would try to take down. 
 4:17: A OK, so. 
 5:32: So yeah. 
 5:32: First of all, like I would first focus on keeping the service available and like identifying whether the issue is resource exhaustion or like application problem and I would check what the status, like events or like log logs using documentunities like, QCTL get pods or like QCT pods, here like, QCTL logs, like since the failure happens during, transaction spike, I would like, I would try to like, specifically check CPU memory or, port limits and like, whether HPA is a scaling, application. 
 6:16: Properly. 
 6:17: I would verify the, readiness and liveliness, process, probes like, do you know, to unhealthy pods stop like, receiving traffic here. 
 6:27: And if we like identify a bad deployment here, so I would, I would use the community's rollout history and like perform a controlled rollback here. 
 6:37: So, So my priority would be like matrics and loads for diagnosis and HPA for scaling and probes for like availability and in this case, and rollback are like for the quick recovery. 
 6:51: So that while isolating the failing parts, so the healthy instances continue serving customers here. 
 6:58: So that what I try to do and, and Yeah, so, and rolling the deployments with the rollback for the safe, yeah, remediation here. 
 7:09: So, yeah, my good, my goal would be to stabilize the service first and isolate the failing component and identify the root cause using matrix and logs and then make the permanent fix without like impacting the healthy cust customers here. 
 7:25: So that's what I would try to follow, yeah. 
 8:33: Yeah. 
 8:34: Yeah, so like I would use a combination of like calendar or month series here. 
 8:39: this work I have done before also, in my work, so. 
 8:42: Aggregation or like left joint to make sure like a month with no payments or like are also included here or not. 
 8:49: And first I would generate the six month date date range including the current month and like present each month as a, as a, as the first day of that month and then I would aggregate the payments by customer ID and the month using date trunk or the equiving function for the database here. 
 9:09: and then. 
 9:11: I would like, the, the important part is that I would like, would not start the query directly from the payments table because, because customers are like, months with no with no payments will would disappear in this case, and instead of, I would create the customer month. 
 9:29: combinations with the like left joint and the aggregated payments to them and then I can use police function and like with with inside the sum of the amount and so the missing payments show as zero here. 
 9:43: So for performance, I would make sure like payments have an index on like a customer ID or like a, a payment date and I would also filter the six months date range as early as possible and, and avoid like applying the functions to indexed column in the, in the filtering. 
 10:04: Predict, like filtering up predicted when, when, whenever possible, and this gives like, accurate month to, like, accurate, monthly total and like while like showing zero payment months and like keep the query scalable in this case, for resolving this. 
 10:22: So that's what I feel and that's would be my answer. 
 11:27: OK. 
 11:29: hm. 
 11:29: So in this case, like, I would like to break the UI into the separate components such as like, maybe, we can break it into account summary or like transaction list and or like a transaction item or like transaction filter in this case and like each, component would have a single responsibility which which keeps the application easier and like to maintain and like. 
 11:56: To take, to test also. 
 11:57: So for estate management, I would keep the local UI state, and such as filters or like selected transactions, inside the relevant component using the user state for, for, shared account, information, I would use the context or a centralized state solution depending on the application size. 
 12:16: And for server data, I would prefer like keeping API state separate, from UI state and using a dataset layer. 
 12:24: With like caching and resetching here and for live stream, like, live, live stream or like live transaction feed, I would try to like use the back sockets or like service and even so that, I, I would like keep that connection inside our customer only and such as, as I say like use transaction feed, I can use, as a, as a customer. 
 12:49: So, so like, rather than like putting the connection logic directly. 
 12:53: into like UI components, the hook would like handle, like connecting the like who would handle the connecting and like, like receiving the updates and cleanup and reconnections here and I would use, use it carefully for side effects and, always clean up, subscriptions and components, on Mount Hill and for performance, I would use, I would avoid to like, unnecessary read and those using memorization. 
 13:22: Where it actually helps, and this, this gives good separation of concern like keeping the banking dashboard responsive. 
 14:38: only this need to be done in Java, actually. 
 14:41: P fault. 
 14:42: OK, that's fine. 
 14:43: yeah, I'm, I'm just using the comfortable language more, but it's OK. 
 14:47: Java is also OK. 
 15:40: Michelle, should I need to, do I need to like, explain anything or just, do it and explain later what I, you know, anything, is there any questions? 
 16:00: Yeah, can you tell me your name? 
 16:02: What's, what was your name? 
 16:04: Yeah, I'm asking that like, is there any process for calling. 
 16:10: Like the, the process for this, yeah, like, I have to just code and clean or just keep on coding what I understand. 
 16:18: No, no, I see you can see under the class outcome. 
 16:20: You just need to write your code on the public strate and so. 
 16:25: Yeah, just feel like. 
 16:28: So I think the syntax or the logic out I I understand the solution I'm just asking is there any process going on. 
 16:40: no, nothing in particular. 
 16:42: So once you are done with the code, you can run it out as well to check if it is running or if there's any issue or. 
 16:48: OK. 
 23:47: OK, well, thank you for this. 
 23:50: This has been submitted. 
 23:51: We can end the call now. 
 23:53: Once I have a report, I will be keeping you posted in the next step's OK. 
 24:00: That's, OK. 
 24:02: I'm I getting it right. 
 24:04: Sure, OK, thank you, thank you, for sure. 
 24:06: Yeah, have a nice day. 
 24:07: Thank you. 
 24:08: Bye-bye. 
 24:09: You too. 
