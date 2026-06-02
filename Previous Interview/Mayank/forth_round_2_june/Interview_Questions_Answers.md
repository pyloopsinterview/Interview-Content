0:00: , so this, the way this is gonna work is, we're just gonna be talking about your work experience for this hour. 
 0:06: So, we're not gonna be asking coding questions, but I will be going into, some of the systems that you've helped build. 
 0:17: Oh yeah, can you, let's start out. 
 0:20: So can you tell me about the, the, project you've led with the biggest scope. 
 0:26: OK, basically, like for the project. 
 0:31: Or like sure like. 
 0:34: The largest project like I led was the Enterprise claim processing platform at the Prudential Financial. 
 0:41: Like prior, prior to this initiative, Like, claim processing all like the multiple disconnected systems and like a significant amount of like the manual effort so we can say the claims were like coming from different channels and the formats like which, like created delays and inconsistencies and the operational challenges. 
 1:05: So the goal, sorry, what company was this experiential Financial. 
 1:11: Yeah, so the goal of the project was to build the centralized platform that could automate the end to end cleaning workflows like by supporting. 
 1:23: Multiple business teams across the organizations and from like the scope, scope perspective, the platform handle document ingestions, classifications, data extractions, validation, and like routing so we also integrate the AI capabilities to assist with the document understanding and the claim processing. 
 1:44: So I get actually we built it as like the distributed microservices platform using Python, Qubates, and AWS, so. 
 1:52: Generally the services like communicate through the asynchronous workflows allowing us to like the scale different parts of the systems independently. 
 2:01: So my role was leading the overall back end and the platform architecture. 
 2:06: I was responsible for the system design, service decompositions, cloud infrastructure decisions, deployment strategies. 
 2:15: And also the mentoring engineers on the team and one of the, like the biggest challenge was designing a platform that could reliably process high volumes of documents while maintaining the, low latencies and the operations visibility, so we address that the true event event processing, distributed tracing and the automated deployment pipeline. 
 2:40: So that platform like ultimately reduce the manual processing, processing efforts and like the scalable foundations that. 
 2:51: Multiple business units like could use. 
 2:56: OK, so what was, what was this in response to? 
 3:00: Like what did you have before? 
 3:04: For the response teams are generally before this platform. 
 3:09: The claims were like spread across the multiple systems and involve like a lot of manual intervention. 
 3:16: So claims were like coming from different sources such as like the uploaded documents, emails, and the external partner system. 
 3:23: So different teams are like using different tools to like process various parts of the workflow. 
 3:29: For example, like, documents intake, data extractions, routing were like often handled by the separate applications or the manual processes. 
 3:39: So because of that there was not a single end to end view of claims, so that a lot of like information had to be reviewed or re-entered manually as clean, claim volumes increase, those limitations become like more one example what was one example of like having to reenter stuff manually, OK, generally, a claim might arrive as a like a PDF or, or a scanned document. 
 4:07: So an operations team member like would review the document and manually enter the key information such as, policy number, claims details. 
 4:16: So letter, letter like in the workflow, another team like might need that the same information in a different application used for like the validation also because those systems are like not fully integrated. 
 4:30: So some of the data had to be manually re-entered or like the verified again so that not only increased processing time but also like reduced the risk of the data entry errors or inconsistencies so yeah. 
 4:46: Question, So this new system, was there, like, what, what are the limits that were placed on you? 
 4:54: was there like a deadline? 
 4:56: Oh yeah, obviously. 
 4:58: like, first, like we could not do a like complete replacement of all the existing systems because, several downstream applications were like still being used by the different business teams. 
 5:12: So the new platform had to integrate with existing systems while like gradually, modernizing the workflow and second. 
 5:21: we were like dealing with sensitive, insurance and the customer data, so the security compliance and audibility were like not negotiable requirements, and every decision on the data she needs to be traceable. 
 5:33: And the third was like the business could not afford a long migration period or like the operational, disruptions claims. 
 5:41: Claims were like being processed every day, so like. 
 5:45: We had to like deliver we can say like to deliver the platform incrementally while like continuing to support existing operations and another constraint was the data quality since the information was coming from the multiple sources and the document formats so we had to like build the strong validation and reconciliation mechanism to like. 
 6:10: And show accuracy before the data moves to the workflow. 
 6:17: OK, so the, the input data essentially came from, what, what were the, what the, what were the sources, for the sources like,, like the data like came from the multiple sources like which was actually one of the reasons the project was needed in the first place, like the primary source was claim related document sources like the PDFs. 
 6:40: The scanned forms I mean like who was who, what was it companies giving you this or was it like customers directly interfacing with this? 
 6:48: Like were you supporting other enterprises like what who are your inputs? 
 6:52: Like it will be actually a combination of both. 
 6:57: Like some claims were like initiated directly by the customers to the various commissions channels. 
 7:03: Well, like, well, they would provide the forms and supporting documents, and we also received the information from like external parties involved in the claim process such as like the healthcare providers, employers, service, service providers, and like partner organizations, depending on like the type of claim. 
 7:22: In addition, like, we pulled policies and the, the customer information from Prudentials internal systems like to validate coverage and then enrich the claim details. 
 7:35: explain what you mean by that. 
 7:37: I'm sorry. 
 7:38: Old po policies from internal. 
 7:40: What does that mean? 
 7:43: like the policies from internal is basically when I say the internal policies, I am, referring, like Generally, I'm referring to the system where the provincial stores information about the customer insurance policies. 
 7:59: For example, like, if a customer submits a disability claim, life insurance claim, or another type of benefit claim, so we need to Verify details such as whether the policy is like active, what coverage the customer has, eligibility informations, coverage limits, and other policy related data. 
 8:21: So that information already exists. 
 8:23: So you have to like you're having to pull from that source, you, you have to pull data from that source. 
 8:30: Oh yeah, yes, like once we extracted information from the claim documents, we would call external APIs like to retrieve additional policy information from the policy administration system. 
 8:45: Like if we accepted a policy number from the. 
 8:48: Sumitted claim we would use that policy number of like to fetch details such as like policy status coverage informations eligibility and other data needed for like the so the reason we did that was to avoid the like relying solely on the information submitted in the claim document. 
 9:07: So we wanted to validate the against the system like to record and enrich the claim with. 
 9:14: Alternative data before like moving it to the workflow. 
 9:17: So yes, like a key part of the platform was like pulling data from those internal systems and like combining it with the information extracted from the claim documents. 
 9:28: So can you tell me what, what was the phasing you mentioned this had to be done in phases. 
 9:33: What were the phases that you, you, how did you deliver stuff? 
 9:37: Yes, like we approach it in another phase because phases because like we're doing a big bang migrations like, would have been like too risky for like a a business critical process like the claims. 
 9:50: So, the first phase was focused on document ions and centralizing claim intent, so. 
 9:59: We wanted all incoming claims, and supporting documents to entire through a common platform, so we had to the single entry point and the second phase was like around the document classification and data extraction. 
 10:11: So this is where we automated the extraction of. 
 10:16: The claim information that was previously being entered manually by the operations teams and the third. 
 10:23: So these phases are so just so it sounds like the phases you're launching pieces of the system. 
 10:30: So like how did you launch? 
 10:32: Were you like replacing the old pieces with the new piece? 
 10:37: like we were not launching the entire platform to all users at once. 
 10:42: Like instead we roll it out incrementally. 
 10:45: Like during the initial phase we onboard the limited set of claim types and the business teams onto the new intake processes while the existing process continued to be operate in parallel so we monitor what I'm wondering is that like you, you for phase one, for example, you built this document intake so how did In order for that to be launched, the old document processors would have to be reading the outputs of your new intake system. 
 11:17: So like, did you have to do that integration? 
 11:20: yeah, generally, Exactly like that was, one of the key challenges of the phase rollout. 
 11:29: Like we could not just build a new intake system in the isolation because the downstream claim processing systems are like still being used by the business. 
 11:38: So in phase one, like we had to build integration layers that allowed the new intake platforms to like feed data and documents into the existing downstream, system. 
 11:48: So the way, like we approach it was like to keep it downstream processes largely unchanged initially and our platform became the new entry point, but after ingesting and normalizing the data, we transformed it into the formats that the existing systems like could consume. 
 12:04: So these allowed the business teams like to continue working with the familiar systems while like we gradually modernize the upstream portion of the work. 
 12:15: So it wasn't, isn't that Transformer all throwaway? 
 12:18: It's, it's like work that you don't need by the end of the system, like after launch, yeah, like some of the, like, transitionals by designers, like when you are like modernizing a business critical systems, they are like often a trade-off between, building on the perfect and the state architecture and like minimizing the migration risk. 
 12:41: So we intentionally accepted some, temporary integrations component because They allowed us to deliver the value incrementally without like forcing a large scale cutover. 
 12:51: So that said, like we tried to avoid pure throwaway work, many of those. 
 12:56: How did you, how did you avoid it? 
 12:58: What, how did you minimize the amount of throwaway work? 
 13:02: for like minimizing the throttle walk. 
 13:06: One thing we did was like they designed the integration layer as like the reusable service rather than just building point to point custom transformation for like each downstream system. 
 13:16: We defined the canonical claim data model, like, within the platform and then the transformation layer map that model to the formats required by existing systems and that gave us 22 benefits like first. 
 13:30: We avoided the duplicating transformation logic across the like multiple integrations and second, as a legacy system we retired we could simply remove specific adapters by keeping the core platform unchanged and we, we also prioritize the integration based on the like long term target architecture. 
 13:50: So this transformation system, that, that handled those temporary transformations, like where did you have to build a new system or was that system already existing like what did these transformations look like? 
 14:05: Mhm, like we do not build it com completely separate transformations platform from scratch since like we were already building the claim processing platform, so we Like incorporated the transformations capability as like part of the platform architecture. 
 14:22: So, the idea was to establish a canonical claim model inside the platform and once the data was normalized into the model, integration components like could translate it into the formats expected by the various transform system. 
 14:35: So that approach allowed us to like keep our transformation logic centralized in the reusable rather than just creating custom point to point integrations everywhere. 
 14:46: So they said the transformer itself was like a part of the of the platform. 
 14:54: Yeah, the only thing that was special was this particular, yeah, exactly, like rather than creating the standalone transformation program we treated it as a core capability of the platform itself. 
 15:07: So the platform responsibility was to ingest data like from. 
 15:12: Different sources normalizing into the common internal model and then expose that data like to downstream system in the like format they required so the the transformation layer like was not a separate system sitting off off to the side and it was like a part of the platform architecture that saw as the like bridge between the new platform and the existing ecosystems. 
 15:35: Mhm, OK, so that. 
 15:38: So in phase, phase one that was document ingestion. 
 15:41: Phase 2 is document classification and data extraction. 
 15:44: What's phase 3? 
 15:48: like, normally the phase 3 was the validation and enrichment. 
 15:52: Like once we are like able to ingest documents and extract key information from that, the next challenge was making sure that the information was accurate and complete before it like. 
 16:05: moved, further through the claim workflow. 
 16:08: So in this phase, we integrated with internal policy administration systems and other enterprise data sources like if, if we accepted the policy number, customer information, all like the claim details from a document, so we would validate that information against the systems of records and You drive additional information with different processes, so these fields was important so you integrate with internal policy systems, but you also, you mentioned that you had to integrate with external ones too, validate customer information, right? 
 16:40: Yeah, basically. 
 16:43: we did it like, although the internal integration was generally the primary source of the, so internal policy systems provided information like policy status, coverage details, eligibility, and customer reports, but depending on the claim type, we also. 
 16:58: Integrated with external data tools and the partner system like to editize supporting the information to get during and the processing like some teams require documentation or like the data from external organizations like you know from the training process so rather than relying solely on the information in the document we put those integrations to fill, fill in the missing information about and it's the claim reports. 
 17:29: I see. 
 17:30: So that's phase 3 validation and enrichment like more cases. 
 17:35: I, like there are some couple of the more cases like after the validation and arrangement, the next media was like the workflow orchestrations and routing. 
 17:45: At that point, we had the validate game record to the. 
 17:49: to, how can more. 
 17:54: Do you feel like the loss of that doubting was manual teams would review information and decide like where a game should go next so we also like automated much of that decision making we don't clean entire business rules and also like we have the testing monitor. 
 18:13: Mhm, I see. 
 18:14: And so what you replace it with, what type of workflow architecture? 
 18:21: Oh so. 
 18:23: And much of the manual team of our work with the distributed like what what type of What type of system do you use? 
 18:37: Like, what type of technology? 
 18:39: OK, generally we implemented the on the event-driven microservice architecture services like communicated to the synchronous messaging with the completion of like one stage generated at the event that that triggered the next stage in the workflow like the orchestration logic was handled, yeah, yeah, basically like and from the technology perspective, we have The services were built in Python deployed on the Cubans in AWS and integrated to the messaging and APIs and yeah, like we used workflow architero like the the services communicated as through the event and DPS and the workflow itself was driven by the business stake or transitions rather than the manual hands. 
 19:27: and the cubes, was it like Kafka or did you use like SQS like what's type of system, sorry, we use, Kafka like Kafka, OK. 
 19:39: I, So, how, like when, what was your, what were you done? 
 19:48: Like, so when you, we've gotten 4 phases, like is there, what was the, how long did the vision for this product go? 
 19:56: Like how, how much of a plan was there that, that you had like drawn out in the design. 
 20:03: The lyrics are like. 
 20:06: We, we had a long term vision like, but we intentionally did not try to define every retail several years in advance because both business priorities and the technology needs were like evolving, right, but how far did, how far did you get, in the initial design? 
 20:22: Like how far did it take you down the road? 
 20:25: Oh Like. 
 20:30: At the initial design stage like we focus on defining the core platform capabilities and like. 
 20:38: Like the initial design will take to take through the most major phases and modernizing, efforts and so is that like through phase 3 or phase 4 like were, were all 4 of those phases including the initial design. 
 20:52: like Like, at a high level, yes, like the major capabilities were like identified early on. 
 20:58: Like we knew that the document, intake data extractions, validations, and then print and the workflow automation. 
 21:06: All necessary parts of the target platform. 
 21:08: So like what was not fully defined upfront was exact implementation details sequencing on the scope of like easy, for example, like we knew we would eventually need workflow automations, but we did not design every workflow rule or integration for like. 
 21:27: On this one, so those were as we learn more from the users and from the production. 
 21:31: Similarly, we knew AI assisted capabilities would likely become important, but the, did this happen in any of those initial four phases, or was that like afterwards? 
 21:46: the initial focus was like was building the four platform capabilities like in in sections and we wanted to establish a reliable and scalable foundation for and, once those capabilities were in place, like we had a good understanding of the workflow, we started. 
 22:05: identify areas like where AI could provide the. 
0:00: Those capabilities were in place, like we had a good understanding of the workflow we started. 
 0:05: identify areas like where AI could provide the most value. 
 0:09: So AI was not prerequisite for the platform. 
 0:12: It was an enhancement that we introduced, after the core, processes were like stable, and we, so what were some of those enhancements? 
 0:20: So like you mentioned the initial four phases. 
 0:23: What was some stuff you couldn't get to until later that you had like designed for? 
 0:28: Mhm, yeah, like for enhancement, like, one example was the AI assisted document understanding and the decision support like we knew early, on that there was a potential there so but we, deliberately did not make it the part of initial rollout. 
 0:44: So the reason was that we first needed a reliable intake extraction validation and workflow automation. 
 0:51: Without those, foundational capabilities in reducing AI. 
 0:55: Would have the added complexity before we have the sta stable process and the yeah yeah. 
 1:05: All right. 
 1:05: And any, any other additional features you had thought of like that that had to wait, hm, yeah, like, obviously like, apart from that there was that, definitely like additional, like ideas like once the area was, was predictive processing and the prioritizations, once we had enough historical claim data we wanted to. 
 1:27: identify things that, were the likely to require special handling and to prioritize them accordingly. 
 1:33: And another area was like more advanced operational and it's like early on like we focused on processing teams efficiently, but later we wanted deeper visibility into the bottleneck, processing trends, teamworkers, and over like the workflow performance. 
 1:51: So that, that's what like operational onboarding to like telemetry platforms. 
 2:01: getting that visibility, what, what does that involve? 
 2:04: Yeah, like that's a part of it, yes, but it was thinking a bit broader than just telemetry. 
 2:09: Telemetry and monitoring help us to understand the health of the platform, things like that. 
 2:15: Processing value. 
 2:18: Latency error rates and the system bottlenecks, but operational analytics also includes business level insights such as like how long clean is spend like each each of the workflow, like where the manually reviews are likering which clean types are like causing delays and overall in the throughput trends. 
 2:36: Mhm. 
 2:37: So, that's interesting. 
 2:40: So I guess what, That, that's, that's an example of like customer information telling you how you work. 
 2:48: So was there any Any customer feedback or like customer experience that could change the design at all,, just like. 
 2:59: Even though like most of other direct users were like internal operational teams like customer experience or like it's still one of the primary drivers behind the platform, so before the platform customer would sometimes experience longer processing times because the information has to be reviewed manually and. 
 3:16: Entered into multiple systems or like validated through the several hands of one of the mattresses we paid close attention to our likeround time and as we automated the intake inspection validation routing, we, we were like able to reduce the delays and provide more consistent processing and we also received feedback from operations teams about like. 
 3:39: Cases that were like getting stuck, information that was like difficult to find, or like workflows that required the excessive manual efforts. 
 3:51: And then So, I'm just taking notes, so that's why I'm trying, I'm trying to catch up to our conversation, so. 
 4:05: What's an example of, of like one of those customer issues that cause problems? 
 4:10: Oh, like the thing for those like. 
 4:15: for example. 
 4:17: Like involve incomplete or inconsistent information is like submitted claim documents. 
 4:23: Like a customer might submit a claim form with submitting document, but some of the information will not exactly match what existed in the policy system. 
 4:32: So it could be something as the simple, like as missing information, outdated it is, or like inconsistencies across the document. 
 4:40: So in the old process, those situations often required, multiple manual reviews and the back, back and forth communication. 
 4:48: which increased processing time and created frustration for like both the operational teams and the customer waiting for a decision. 
 4:54: And one of the improvements we made was automating much of the vegetation process. 
 5:00: We could identify missing or inconsistent information much earlier in the workflow and around those cases appropriately instead of like having done. 
 5:10: Sit in queues waiting for like the manual discovery. 
 5:14: Mhm. 
 5:14: So, this was like That process, I guess that's in phase one. 
 5:20: So how did you like collect that cus customer information about like where they were getting stuff? 
 5:28: basically, for like. 
 5:31: The information primary came through the claim, submission channel. 
 5:35: The customer will submit claims, from, forms along with the supporting documents, typically as the PDFs, scanned documents, or like, so there are some digital forms depending on the like. 
 5:48: I can say, submission channel. 
 5:51: So those documents entered the engage platform where like we stored them and then ran, classification and extraction, processes to identify the key information such as like, policy numbers, customary bills scale types, and other relevant at attributes so. 
 6:09: We then, combine that extracted information with the data derived from like internal policy systems and other sources during the validation and inter phase. 
 6:20: Yeah, I, I guess I'm just wondering like, so. 
 6:24: You had anticipated that customers would have issues with their inputs, so that didn't exactly change your design, like that was part of your design, right? 
 6:37: So is there, were there any like customer interactions that like that changed the design at all or was it pretty much according to plan? 
 6:49: Like, yes, like there were definitely teams, definitely the cases were like the feedback, influenced by design. 
 6:58: Like one example was around the exception handling and the visibility into the team status. 
 7:03: Like initially, we were like very focused on automations, getting documents to, intake, extraction, valuations, and routing as like efficiently as possible. 
 7:14: But that users started like working with the platform operations teams like wanted more visibility into the why certain teams were like being flagged, delayed or like routed for the manual debu so that led us to invest more heavily in the auditability we work for the status monitor tracking. 
 7:33: So like what was, what were some, what are, what were some of the auditing like, ches that you added that did that hadn't been part of your initial plan, for like the. 
 7:44: Auditing like. 
 7:46: Users wanted to like understand exactly like what happened to claim as like moved to the workflow so we started capturing details, audit events like for like key actions such as the document injection, data section results, validation outcomes, and for example like if a claim was routed for like manual reviews, users wanted to know why. 
 8:08: So was it because, information was missing so they have like validation rule fails and did. 
 8:15: Data from the submitted document like not match the policy system you also add the visibility into who made the changes when those changes were made and what the previous values were. 
 8:26: So these are, this was the particularly important for like compliance and the operations investigation. 
 8:32: Where do you show the auditing information? 
 8:35: sorry. 
 8:36: What did you show that auditing, so you got audit events of like when teams pass certain points in the claim process. 
 8:43: So where did those show? 
 8:46: Yeah, like primary to the operational users in and support, support dashboard by the claim teams or specific claim users could view, view it processing history and receive the major events that like are controlled for the like throughout the life cycle. 
 9:01: So it's like not exactly customer information. 
 9:04: It's so it's operators intervening on customers' behalf. 
 9:09: That's what it is, OK, yeah, like, like in, in, in this case, like, the direct users of the platform are like primary operational teams claim processes and the support, support, personnel rather than just the customer themselves. 
 9:24: So most of the feedback that influence the design came from the people processing claims on, on behalf of customers. 
 9:32: So they have really to quickly understand claims status, investigate issues, and that is all the exceptions had like the direct impact on the like the experience. 
 9:43: OK, so how did you learn about these these requests for audits, like how, how, how did you get that information that customers wanted more auditability? 
 9:55: we learned about them, primarily, through the operations teams that were like using the platform every day. 
 10:02: So during the phase rollout, like we had regular feedback sessions with the team processors, supervisors and support teams as they like started using the new platform they would tell us, like where, where they were spending time investigate investigating the, where they lacked visibility into what the system was doing. 
 10:25: I see. 
 10:27: so this is like every week, you said? 
 10:29: . 
 10:32: Sometimes, like, not necessarily every week, but fairly like during the rollout period. 
 10:37: Sometimes a week, sometimes twice a week. 
 10:41: OK, perfect. 
 10:42: So like, Pretty much like near by, yeah. 
 10:50: OK. 
 10:52: it's just easier to type that way. 
 11:01: So what's, now that you've built the system, how, what would you have done differently? 
 11:09: Like what were some things about the design that like you would design differently now, now that it's behind you? 
 11:15: Mhm, So like. 
 11:20: Looking back, one thing I would invest in earlier is observer and the operation slowly. 
 11:25: Like we initially focused heavily on the core business workflows, OK, like intake extractions, valuations, and routing, which was like the right priorities. 
 11:34: But as adoption view, we realized that the operational visibility become just as important as the workflow itself. 
 11:42: So we ended up adding more auditability facility and we can say exceptions management capabilities based on user feedback and if I, I were starting again, I would bring more of those capabilities into the platform earlier because they significantly reduce troubleshooting time and improve the user's confidence, in the system. 
 12:06: Was that like did you get burned by issues that you didn't know were happening before you had this observability of the integration? 
 12:20: yeah, like, one area that surprised us was the amount of effort required for like exception handling and the investigation work. 
 12:28: Early on, we were very focused on the happy path, getting claims through, through the intake extraction of validation and routing efficiency. 
 12:36: But once the platform was in production, we realized that the operation team spent a significant amount of the time dealing with edge cases, valuations, expenses, In complete submission and we investigate indications issues within the system. 
 12:52: So the system was technically working, but the users are like often, like needed, better visibility into as something, happened. 
 13:00: So that's what drove, many of the auditability and exception management in answers like, we added, later. 
 13:09: OK. 
 13:11: so can you, can you tell me what the I guess the, the system that had the biggest change from its old version to its new version. 
 13:27: Generally, I would probably, like still point to the claims platform because the change was quite significant, before the project, but the process was fragmented across the multiple systems and heavily, dependent on the manual coordination. 
 13:44: Oh, I'm, I'm still talking about the claims system. 
 13:47: I'm just, I mean like within that you had a couple of systems that you had to replace, and I'm wondering like what was the, what was the component that changed the most. 
 13:59: Yeah. 
 14:02: Like all, all the subsystems, Yeah, Eugene, like. 
 14:08: I would say the document intake and the extraction component changed the most. 
 14:13: Like in the old processes, incoming documents were like largely handled through the manual reviews. 
 14:21: So someone would receive the documents, inspect them, identify, identify the relevant information, and, enter the key details into downstream system and in the new platform we transform that into an automated pipeline documents and documents were like ingested centrally classified automatically. 
 14:39: And then made available to downstream workflow. 
 14:42: So that fundamentally changes how informations entered the system instead of the people acting as the integration point within the documents and the business systems. 
 14:53: So that platform became the integration point. 
 14:57: I see, OK, so were there any dependencies that that were so actually hm let me think about it. 
 15:07: So how many different like sources are you pulling from when, when like both getting claims from from people who send you PDFs or like systems or having to pull data from them like how many integrations are they? 
 15:23: It depends on the workflow like but generally. 
 15:27: We were pulling from several categories of posts, like 1st. 
 15:31: We had the claim submissions to the Excel and documents and the forms coming from the customer or the external parties. 
 15:37: Again, we had internal policy administration systems like which we, which were like typically the primary systems of the report of like for the coverage coverage and eligibility and the policy details and other we had the customer and the account related systems that contained the additional information stated during the validations and the processing. 
 15:59: Mhm. 
 16:00: So this claim processing system, did you have, did you like modernize every aspect of like the previous system, or was there some stuff that you had to leave, to leave alone, like some stuff that you, you didn't, redesign, Mhm, That was actually one of the key constraints like we had to work with them. 
 16:20: Like there were, several downstream systems like that but still critical to the business operations and replacing them like would have, introducing significant risk and required. 
 16:32: Much larger organizational changes. 
 16:34: So our approach was to modernize the areas that were like creating the most operational structures. 
 16:40: So things like documenting, extraction, evaluation, and workflow coordination. 
 16:45: So while you continuing to integrate with some existing systems that were still providing value and in other words, like we, like, like what, like what are what internal systems were not changed. 
 16:56: Oh, recently. 
 17:01: Those systems were like already the systems of the record of policy information covering details and customer policy details. 
 17:09: So replacing them would have been much larger business initiative with significant risk. 
 17:14: So we also have the several downstream claim processing enterprise system that were like deeply integrated into the existing business operations rather than replacing them immediately, we need, like. 
 17:26: Integrated with them to the APIs and standardized interfaces. 
 17:31: So these are downstream claim processing systems. 
 17:34: You said how, how are they different than the claim processing system that you're building? 
 17:42: Mhm. 
 17:43: Only for that the platform we were like building was not intended to replace every function involving the claim processing, so it was focused on August, augustrating and automating the front and, front and middle portion of the workflow. 
 18:01: For example, we handle document intake, classifications, data sections, and routing. 
 18:08: So, however, there, there were like existing enterprise systems that handle the specialized streaming function like such as team and just adjustation streaming processing regulative report the other businesses specific activities. 
 18:23: So those systems are like already deeply embedded in the business operations and contained years of like business logic. 
 18:30: So rather than, rebuilding all, all of that, the functionality our platform acted as the like coordinations and the automation there, so we collect, collected and prepared the information when you needed and then passing the the thought that that was not automated is what you automated first, yeah, yeah. 
 18:51: Yeah, like, firstly, what, what we did, like we started, we started, by identifying the, the parts of the process that were like creating the most operational, frictions areas that like the, significant manual efforts repeatedly by the, document review and the workflow and so, so those are the, places like where they. 
 19:15: Automations could like provide the biggest immediate benefit. 
 19:19: So that's it like we were not just automating the task 11 for one in many cases we go for like a standardize and redesign the parts of the workflow because automating an inefficient process like does not unnecessarily solve the like underlying problems. 
 19:36: Mhm. 
 19:37: And, What improvement did you get? 
 19:45: All the improvement, the biggest improvement was like the processing efficiency, consistency, and visibility. 
 19:52: Like before the platform, a lot of like time was spent on manual document view. 
 19:57: We reentering information into the multiple systems and like moving work between teams. 
 20:04: So by automating, intake, extraction and routing, we significantly reduce those manual touch points and we also improve the consistency because. 
 20:14: The same validation rules and the workflow logic were being applied, systematically rather than depending on the individual, interpretations, and one of the major improvements was visibility. 
 20:25: Like previously, it could be difficult to determine where like a claim was the process or like why it was delayed. 
 20:35: So with, with the new platform we had to end to end tracking and auditability, throughout the workflow. 
 20:42: Mhm. 
 20:43: Let's see. 
 20:44: And did you remember like any, like any percent increase or like, like the amount of money that you guys like saved or something. 
 20:55: I don't remember the exact percentage off the top of my head, so I don't want to guess. 
 21:02: OK, that's, that's cool. 
 21:04: So like the, there was all these like, how, how many times would, like, would an operator be pulled into like entering some manual data like every week? 
 21:15: Did you like remember that? 
 21:16: Like how, how many times do they have to be engaged on like entering that data before this automation? 
 21:23: I don't remember the exact volume, but a manual intervention was like the common you know that it was like meaningful operational concern. 
 21:31: And one of the main reasons the project was funded, so the manual work was not necessarily entering and the entire came from the scratch every time. 
 21:39: More often it involve extracted information resolving validations, exceptions, investigations that completely eliminated. 
 21:51: Were, were those manual reviews completely eliminated? 
 21:58: Like, no, not completely, and that was not really the goal. 
 22:03: In the claim environment, there will always be scenarios that require human judgment, incomplete documentation, unusual claim situations, so policy exceptions or cases that need additional investigation. 
 22:16: So what we were trying to eliminate was the routine manual work, for example, like. 
 22:23: Manually entering information from documents, performing, repetitive, validation checks and moving like one between the teams or like looking up the data across the multiple systems. 
 22:34: So by automating those activities like, we reduce the number of the teams regard the manual handling. 
 22:42: OK, thanks. 
 22:44: So I think that, that's enough. 
 22:46: I have enough material, so I think we can call it a little bit early, but, it was, nice to talk to you and, good luck with the rest of your sessions. 
 22:54: Yeah, thanks, G. 
 22:55: Thanks. 
 22:55: Nice to meet you too. 
 22:57: Yeah, nice to meet you. 
 22:58: All right, see you. 
 23:00: Bye. 

