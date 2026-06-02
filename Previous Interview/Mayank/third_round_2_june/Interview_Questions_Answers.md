0:00: A I. 
 0:03: Good afternoon. 
 0:03: How are you? 
 0:05: I'm good. 
 0:06: Good afternoon. 
 0:06: How about you? 
 0:08: I'm doing good, thank you. 
 0:10: my name is Salman Gopalakrishna. 
 0:12: Am I visible to you? 
 0:13: Yeah, yeah, I can see it. 
 0:16: Yeah, me as a politician, so I've been with BNSF for about 10 years now. 
 0:22: I work primarily on the intermodal and automotive side, so it's a little bit of a, compared to other railroad, railroad segments, intermodal and automotive is a little different in that we actually touch the cargo that we, that we ship. 
 0:38: in other places we don't typically touch the cargo, but that's what's different. 
 0:42: so that's just about me. 
 0:44: before we move forward, quick question, can you verify your phone number, please? 
 0:48: sorry, phone number. 
 0:52: Yeah, like it's 301-447-0998. 
 1:00: And your email? 
 1:02: it's Patil.m0220@gmail.com. 
 1:06: OK, all right, perfect. 
 1:10: so this is going to be the systems design new and in this, hopefully you're already familiar with the format. 
 1:16: There'll be two big behavioral questions and then we'll get down to the actual, actual, you know, whatever the segment is in this case, it's system design. 
 1:25: So I have a problem for you that, you know, for you to generate a systems design on, yeah. 
 1:33: Now with systems design you're free to use any tools you want. 
 1:36: If you're comfortable using any diagramming tools, go ahead and use that. 
 1:41: All I ask is share your screen and then towards the end extract that into a PDF or JPEG or whatever it is and send it to me. 
 1:48: that's the only thing, What questions do you have for me before we get started? 
 1:55: like, currently I don't have any questions. 
 1:58: OK, alright, we'll circle back again, towards the end to see if you have any questions. 
 2:05: are we ready to jump in? 
 2:06: Yeah. 
 2:08: All right, awesome. 
 2:09: So the first question I have is, tell me about dying. 
 2:13: you had a significant change that required influencing others who didn't initially agree. 
 2:20: What pushed you to action, and how did you get alignment? 
 2:24: OK. 
 2:26: Basically, On that like. 
 2:31: one example that comes in comes to mind is like from current to life and Prudentials like where we were like building out the claim processing platform. 
 2:40: So at the beginning of the project like different teams had their own processing workflows and we can say. 
 2:49: Many of them like preferred continuing like with like more traditional synchronous architectures. 
 2:56: So because that like was what they were like familiar with my proposal was to like move forward like toward an even driven microservice architectures running on the AWS and the Cubans I like. 
 3:10: document injections, classifications, validations, enrichment, and like the routing would be like handled by the independent services. 
 3:18: So initially, like there was some resistance. 
 3:22: The main concern was like we increased the complexity operational. 
 3:27: So I like learning curve associated with the, distributed, system. 
 3:33: So some stakeholders felt the like existing approach was like good enough and like were worrying, like worried about the introducing the additional moving parts. 
 3:43: And, so instead of like, pushing the idea immediately, I focused on understanding their concerns and gathering the data like I organized several architectures review sessions like where we, discussed current bottlenecks, processing delays, scaling the limitations, and the failure scenarios. 
 4:02: And apart from that, I also like created a proof of concept, demonstrating the how like how our synchronous processing could improve, throughput and the isolate failures without impacting the dialog workload. 
 4:16: And also I showed, advices from like our testing including the improved processing times, better the fault tolerance, and The ability to like independently scale services during like peak claim volumes and I also like work closely with operations and the development teams like to address concerns around like monitoring, logging, deployment and the supportability and over the time like as people saw the data and understood the, long term benefits like we gained alignment across the teams and also like the solutions was approved and implemented successfully. 
 4:54: So as a result, the platform began significantly more scalable and resilient and processing thousands of claims documents efficiently like. 
 5:04: reducing manual, interventions and like operations bottleneck. 
 5:08: So, like the biggest, lesson like I learned was that influencing people is really about like convincing them, like you are right. 
 5:16: It's about listening to their concerns, involving them into the like decision making process and like using data and results to like build trust and alignment. 
 5:30: OK. 
 5:31: so how long did you think from proposing to, you know, when you thought you got out on the other side, how long was that, time? 
 5:45: Generally It was like from the time like I initially proposed the architecture until like we had broad alignment like all the teams like it was probably around 2 or 3 months. 
 5:59: The first few weeks were like focused on understanding concerns and gathering requirements from the different stakeholders. 
 6:05: After that, like, we spent time building like a proof of and we're reading some of like the assumptions around like scalability, reliability, you know. 
 6:14: Operational support and once we had the data from the POC and like a few architecture use sessions like the conversations become like much easier because people could see the benefits rather than just hearing about them theoretically so like I, I mhm. 
 6:33: so who would you think was the was the stakeholder who was pushing hard of all the, all, all the people, pushing back hard. 
 6:47: Like the most resistant stakeholder were like actually some of the application owners and the operational leads from their perspective. 
 6:56: The existing system was stable and familiar, so moving to like event-driven microsurface architecture like introduced concerns around the operational complexity, debugging and the monitoring and support. 
 7:08: their biggest concern was not whether the architectures like would work technically. 
 7:13: It was whether the teams could like, effectively maintain and supported in production. 
 7:20: So they were like worried about the things like distributed tracing, troubleshooting the failure access, and the learning curve associated with like Cubans and like the as synchronous workflows. 
 7:31: And also I complete, completely understood those concerns because they were like valid. 
 7:37: Instead of like treating the resistance as a roadblock, like I viewed, viewed it like a valuable feedback and I spent time like working closely with with them demonstrating like our monitoring strategies, logging framework, alerting mechanisms. 
 7:53: So we also evolved them early in the design review so they failed ownership of the solutions and. 
 8:01: once they saw that we had addressed operations celebrity and the supportability like. 
 8:06: they become strong advocates for the approach. 
 8:09: In fact, some of the people who were like initially the most, skeptical later helped like the drive adoptions across the, across the other teams. 
 8:19: OK. 
 8:20: did you have to, bring a new tooling for this, or did your existing tooling was already, the existing tooling you had. 
 8:30: Already able to support the new architecture. 
 8:34: Basically, it was like the combination of both. 
 8:37: Like we already had some of the foundational toolings in the place, like particularly around the AWS containization and the CSCD. 
 8:45: However, like moving to like the more distributed even different architectures required us to like expand our like the tooling in the few areas, for example. 
 8:54: Like we enhanced our observ stack by understanding the centralized logging matrices collection and distributed tracing. 
 9:02: So that was important because debugging, a microservices environment is like very different from debugging a mono the applications and we also like. 
 9:12: Introduce additional monitoring and alerting capabilities like to help operations teams gain visibility into. 
 9:19: The service has messaging processing and failure scenarios and on the deploy deployment side like we further standardize like our cument needs deployment patterns and automated more, more of the like the release process through, through all of the CICD pipelines. 
 9:37: OK. 
 9:38: did you have to scale down any of your initial thoughts, or were you able to roll it? 
 9:45: To your satisfaction. 
 9:47: Yes, like, absolutely, like, in fact, I think that's normal part of any large initiative, like initially. 
 9:54: My vision was to have every stage of the claims workflow, workflow like fully separated into independent microservices from like day one, as we got deeper into discussion, it became clear that the introducing too many services at once would like increase operations complexity and the slow adoption. 
 10:14: So like, we like scaled back the initial scope and focused on like. 
 10:21: Breaking out the area that would provide the most immediate value. 
 10:25: So such as like document injections, classifications and or like so some of like the less critical components like remain more tightly coupled during the first phase. 
 10:37: So that approach like allowed us like to deliver the business value faster like by giving the teams like time to become comfortable with the new architectures and operations model and Looking back, I think it was the right decision. 
 10:51: Like we still achieved the scalability and the reliability goals were like we targeting, like, but, but we use implementation risks and made the transition much smoother for the organization. 
 11:03: OK, OK, all right, awesome. 
 11:06: That's all I had on that one. 
 11:08: my next question is, tell me about a time you had to make a tough call, one where you held firm on quality or standards even when there was pressure to cut corners and move on, and how did you handle the pushback. 
 11:23: 01 time. 
 11:26: Mhm, one example like that comes to my mind was, during the development of like, the claim processing platform at Prudential, like we were approaching a major release milestone. 
 11:41: And there was significant pressure to deploy because several business teams were like waiting to start onboarding their workflows. 
 11:50: So like during the final validation phase, we identified reliability concerns around like some of the synchronous processing panels under, under like the certain failure conditions and messages like could. 
 12:04: But we delayed or tried multiple times like which created a risk of like duplicate processing. 
 12:11: So these are like understa understandable like pressure like to move forward because The issue was not occurring frequently and the fixing it would delay the release like by by a couple of weeks. 
 12:25: So some stakeholders felt like we could address it in a later iteration, but like I felt strongly that since this platform handled claim related workflows, reliability and the data integrity, so we're like non-negotiable. 
 12:42: So if duplicate processing occurred in like the production. 
 12:46: it could, it could create downstream operational issues and reduce the trust, in the platform also and rather than, simply say no, like I gathered the engineering leads for the stakeholders and operations teams and like walk them through the prudentials intact and I, I quantified the risk and also explained the failure scenarios and outline what, what would be the required to resolve the issues properly and we. 
 13:13: Ultimately, I decided to postpone the release slightly and implement additional safeguards including the like the stronger potency controls, improve the handling and like the more comprehensive like the testing around the failure recovery scenario, so. 
 13:39: All right. 
 13:40: any learnings from, from that? 
 13:43: yeah, like the lesson was for me was that maintaining quality standard does not mean being inflexible. 
 13:50: It means clearly communicating it is, using the data to support decisions and helping the stakeholder understand the long-term impact or like the short term compromises. 
 14:02: OK, did you get any questions on why you ended up that way and how you had to, how you ended up answering those? 
 14:14: basically, Like, definitely, like one of the biggest lessons I learned was the reliability and the quality requirements like need to be discussed like much earlier in the project life cycle and looking back. 
 14:27: like, we were like heavily focused on delivering and like. 
 14:32: These things are like and after the experience, I become like much more proactive or like, about like defining the non-functional requirement upfront and yeah, and just like I did some like stakeholders naturally wanted to understand like why we were like recommending our delay especially like since the issue was not causing failures all the time. 
 14:54: So my approach was to like walk them through the data and I showed the load testing results, explained the failure patterns like we were seeing and outlying was good. 
 15:05: Happen if the traffic increase in production. 
 15:12: OK. 
 15:13: All right. 
 15:16: Perfect. 
 15:17: That's all I had. 
 15:19: moving on to systems design in this section, you know, feel free, as I said, to use any tools you want. 
 15:26: And if you're using additional tools, please share your screen in the back and see what you're doing. 
 15:32: Whenever you're ready, Let me know when you're good to go. 
 15:40: I just use, order. 
 15:43: numbers Yeah. 
 16:44: All right, perfect. 
 16:45: So, the question we have is, you're responsible for designing a train wheel crack detection and safe stop stop system. 
 16:56: what that means is the wheels are the wheels on the cranes and locomotives, they're made of cast iron and are prone to cracking due to environmental exposure, you know, things like temperature swing, moisture corrosion. 
 17:08: And mechanical pressure. 
 17:10: Now, if these cracks are undetected, they can propagate and lead to real failure and eventually to derailment. 
 17:17: so how would you design a system that can detect cracks in real time and stop the training before a derailment occurs? 
 17:26: OK. 
 17:30: Generally for this type of scenario, what I usually did. 
 17:38: mostly, like my, my primary goal is like to early crack detections and preventing, derailment by stopping the train safely before the, catastrophic wheel failure occurs, and since this is the safety critical system, so I'd optimize fault reliability, fault tolerance, and the low false negatives. 
 17:58: Missing a missing a crack is like significantly more costly than the occasionally generating false positive that requires inspection. 
 18:09: So like the high-level architecture was like the wheel sensors, edge processing on boarding, crack detections in general, the ML model and risk assessment and to see. 
 18:20: Continue unsafe or like stop train and and last like big control or like monitor. 
 18:27: So step two is basically it's a sensor, like I, I will not rely on a single sensor because safety systems require redundancies. 
 18:39: should I draw this first? 
 18:42: Yeah, sure, go for it, yeah. 
 21:45: Drawing skills, not, not like as good much on that. 
 21:51: No worries. 
 21:56: Generally my design, like it starts with multiple wheel sensors like feeding on the onboard edge processing system. 
 22:04: Basically the edge system performs the rule based on, amalgaming crack detection and calculate, calculates the confidence scores and sends, sends the results to the decision services based on the severity of the risk. 
 22:19: The system can alert the driver, reduce the speed, and like initiate an emergency stop. 
 22:26: At the same time, like the telemetry is sent to the centralized fleet, monitoring platform, like for maintenance. 
 22:34: And also, like, the design, the key design goal is like ensuring the safety while the minimizing. 
 22:43: The false positives and like operation independently or like the network connectivity. 
 22:50: OK, so these sensors, where, where are they located? 
 22:54: the census? 
 22:56: Yes, so starting with the sensors, where are the 
0:00: the sensors? 
 0:02: Yes, so starting with the sensors, mhm, where are the sensors located? 
 0:07: Like, I would move non vibrate vibration sensors on, like the near wheel, axle, assembly. 
 0:15: So especially around the axel box or the bearing house, mounting them directly on the wheel is not like practical because the wheel is rotating continuously. 
 0:24: So the axle and the bearing assembly provide the stable location while still capturing vibration pattern caused by the wheel defects. 
 0:31: So like the so this is, these are sensors that are going to go on every wheel axle across all of the network, yeah, obviously like. 
 0:41: basically, for like, that's like if we have the, like, like if we were like talking about like deploying the across of the entire network, like I would probably revisit the architecture because instrumenting every wheel XL with multiple sensors would become like very expensive like from both like the hardware and the maintenance perspective and like network is here. 
 1:08: I would like, like move towards like the hybrid approach. 
 1:14: Like, what do you mean by that? 
 1:17: like the train, passing, then we have the track side sensor or like the inspection gate, and then we have the detection agent and then last like alert or like we have to stopping like instead of placing several sensors on like every wheel set. 
 1:32: I would use trackside inspection station like strategically, positions to put the network such as like the rail yards, maintenance facilities, high traffic corridors and major checkpoints as trains pass through these inspection points like we can use acoustic sensors, vibrations analysis, thermal imaging, laser scanning, or like. 
 1:55: Ultrasonic inspection systems to like evaluate wheel without requiring the extensive instrumentation on the like the train itself. 
 2:04: OK, does this change any of the flow that you have here if we went down that path? 
 2:17: Yes, like, some, some parts of the architecture would change, but like the overall flow remains largely the same. 
 2:24: The biggest change is like where the data originates and where the reduction happens. 
 2:29: OK. 
 2:31: All right, if you need to make any adjustments towards that goal, Go ahead and make that and then we can continue discussing. 
 2:40: Yeah, sure. 
 4:15: like, I modify the architecture by moving the sensing and the initial processing from like onboard systems to strategically located, track side inspection station. 
 4:26: So generally this reduces inspection station, so like. 
 4:31: this reduces the deployment and maintains the cost while still allowing us to inspect every wheel that passes through the network. 
 4:38: So the downstream components, and the directions, risk scoring, decisions making like, and the fleet monitoring remains largely unchanged because those responsibilities are like independent of where the census data originate. 
 4:53: And there were more things. 
 4:55: Oh, OK. 
 4:58: Now, is that changing any of the downstream flow? 
 5:06: on how we detect, can you notify, like for most of the part, like, like, you know, the downstream flow remains very similar because the responsibilities of the detections does not like reply, rely depend on like, where the data comes from. 
 5:23: We still need risk assessment, decision making, and like some speed monitoring. 
 5:28: OK. 
 5:29: Now, we have sensors on the train or the wheels, that's one thing in terms of identifying where the issue is. 
 5:36: Now, these are going to be sensors that are sitting outside. 
 5:39: How do we correlate those that data back to knowing which train is, is the one that we need to stop of, of the, because we have about 2000 trains running across the network every day. 
 5:57: like, once we move the sensors of the drain, like correlation becomes a critical part of the design. 
 6:03: I would also like to introduce an identifications and correlation before, before like the detection engine. 
 6:09: So, like, firstly identify the drain like first. 
 6:13: I need to know Or. 
 6:16: Which train is like passing the inspection station. 
 6:20: Then once I know the train, I need to know which area rail car is like generating the signal. 
 6:28: And this is like actually very realistic because North America railroads like already use AI tags. 
 6:37: I, I, I likely, leverage the AEI tags that are like already commonly used across the railroad for equipment identification. 
 6:47: And after that, suppose the train is moving through the station like. 
 6:52: So each wheel passes the sensor at the specific timestamp and also I would coreate the sensors reading using the timestamp and the train speed, Axel counts and car configuration data. 
 7:07: OK, I'm curious about your knowledge on AI data. 
 7:11: I mean, that's not, you don't have a railroad background, I presume. 
 7:17: OK, I'm just curious where you learned that we use AI, AEI readers. 
 7:22: OK, for like the AI thing, like, it was like. 
 7:29: you ask about like the AI or AEI? 
 7:34: You mentioned AEI leaders. 
 7:35: I was just curious where you would come across number one. 
 7:39: basically, I don't, first of all, like I don't come from the like the railroad, so I was thinking in terms of like the, generic seat identification patterns that I like use in other industries like if they're like the railroad disposal mechanism already in place like for. 
 7:56: Identify rings on the car. 
 7:58: So as they move to inspection points, I would absolutely allow those rather than doing something new. 
 8:05: So yeah, like, to be transparent, like I don't have direct railroad estate experience. 
 8:11: I came across the technology while doing some research and preparation around like the railroad operations and the asset tracking use case. 
 8:21: My understanding is that the railroads use equipment identification system to track the locomotives and the rail cars across the. 
 8:29: Networks and AI seems like a potential mechanism for like coating inspection data like to the specific assets. 
 8:38: OK. 
 8:43: Perfect. 
 8:44: so let's go down the The data flow, can you walk me through it? 
 8:50: OK. 
 8:53: basically for like the, data flow, it was like. 
 8:58: as, like the train enters the inspection zone, and the first thing like we need to do. 
 9:06: Is like identify the drain and establish an inspection unit. 
 9:11: So like the train arrives, the train ident identification and the train even created. 
 9:17: So that gives a like unique event ID that all census readings will, will like will be associated with. 
 9:25: And then the second step is like the data collection like onto the census look like. 
 9:32: As like the train moved through the like inspections at the station. 
 9:38: Multiple sensors collect data simultaneously. 
 9:41: And at this point, the data by itself is not very useful because we need to know which we generated which reading. 
 9:50: So the sensor data like the correlation services. 
 9:52: So the correlation service combines stamps, trainee speed, axel counts, and the train identification data to map like each leading back to the specific train real car excel and the weak. 
 10:03: And after that, once the data is correlated, it moves to the detection engine. 
 10:09: The rule engine like. 
 10:12: looks for like known failure conditions while anomaly detection model looks for like unusual patterns compared like to the historical data. 
 10:22: And after that, the outputs from multiple sensors are like combined into the confidence score and then the decision services like the risk score is then passed to the decision, service and depending on the severity, different actions can be taken and in parallel. 
 10:40: All inspection data is sent to the fleet monitoring. 
 10:44: So, yeah, like over the time we accumulate infection history for like every wheel set and this that allow us to identify the degradation times improve like for detection model and proactively schedule maintenance before the failures occurs. 
 11:00: OK. 
 11:01: Can you slow down just a little bit? 
 11:04: So where is correlation happening in this? 
 11:08: like for the poditional things,. 
 11:13: It was like, like correlation would happen simultaneously after the data collection and before the detection engine. 
 11:21: The raw sensor data coming from the acoustic thermal, laser and ultrasonic system, like what was flow into the correlation of it, it's, responsibility is like to associate each sensor reading like with the core, the Axel and the wheel. 
 11:41: Got it. 
 11:41: OK, I'm curious, where, which component that you've drawn here does that. 
 11:47: If it was the detection engine or if it came from up above in the sensors. 
 11:57: basically. 
 11:58: It was like, I would prefer to the correlation before the detection and the, the, the inspection station is like already collecting the raw sensor data. 
 12:08: So that's a natural place to associate the reading with the dream that passing through, along, along with the car position, axel position of the location information so. 
 12:21: OK, OK. 
 12:23: , right. 
 12:25: What can you tell me about operational efficiency? 
 12:31: Or like, operational efficiency. 
 12:35: when I think about operational efficiency in the system, I'm looking at like How we maximize safety while like. 
 12:43: Minimizing unnecessary inspections down time and. 
 12:47: Maintenance costs, so that like. 
 12:50: Then I break it down to the reduce the manual inspections, predictive maintenance, reduce the unplanned downtime, privatizing the maintenance resources. 
 12:59: Right, but how are you going to achieve that? 
 13:01: Can you be a little bit more specific? 
 13:04: for achieving that. 
 13:07: Oh, like. 
 13:11: one way we improve operational efficiency by like moving from like time-based maintenance to condition-based maintenance like today. 
 13:21: A wheel might be inspected every 30 days regardless of its condition. 
 13:26: So with this system, like we are collecting health information every time, so the train passes an inspection station. 
 13:34: So if a wheel consistently show healthy reading. 
 13:38: We can avoid unnecessary inspection. 
 13:41: If we'll be show signs of like the degradation, we can simultaneous like proactively, schedule maintenance before it becomes a safety issues. 
 13:51: And another area is like is reducing the manual inspection effort like. 
 13:56: instead of like having maintenance person inspect every wheel, equally, the system can like automatically rank wheels by the risky score. 
 14:06: when I, when I said operational efficiency, I was thinking more on the, of the current system, you know, things about reliability, performance, and all that. 
 14:18: How can we achieve those in the current system architecture? 
 14:23: OK. 
 14:24: For like achieving that. 
 14:27: Like from like operations perspective, like moving to trackside inspection stations improves the reliability and when I say the operational efficiency, I was thinking more about the system itself. 
 14:41: So what, when I think about the operational efficiency, like I'm focusing on the reliability, performance, scalability. 
 14:49: Like since this is the safety critical systems, reliability would be my top priority. 
 14:54: OK, like, and if, if an inspection station goes offline, the system like should continue operating through nearby station and alert operational items and If one sensor type fails, such as the thermal imaging, the system should still function using the acoustic and the ultrasonic data, like, although like perhaps with the reduced confidence and. 
 15:18: Performance is important because trains are like moving continuously through the inspection station. 
 15:23: So the train passing inspect and analyze then the decision. 
 15:28: So these detection pipelines should process sensor data in near real time so. 
 15:34: Bad results are available before the train moves too far beyond the inspection point. 
 15:45: OK. 
 15:49: So you talked about reliability. 
 15:51: Now, how can we ensure that we are Stopping the train only when we. 
 15:59: I think we need to. 
 16:01: We don't want to be unnecessarily stopping the train because, you know, stopping the train unnecessarily is going to really cost us money. 
 16:07: We need to be delivering on time. 
 16:12: for the For this, like, generally, That In a system like this, the goal is not simply to detect tracks. 
 16:24: The goal is to make the correct operational decision. 
 16:28: If we stop the SSI we create significant operational and the financial costs, yes, right. 
 16:33: firstly, like we have like the multi-sensor validation. 
 16:36: Like I would never stop the train based on the single sensor reading. 
 16:41: Like in that scenario, I would generate an alert or the request additional inspections. 
 16:47: Rather than immediately stopping the train. 
 16:50: And I would also combine signals like from multiple inspections methods and like calculate an overall confidence score. 
 17:00: And this is like the, also we have the thyroid response model. 
 17:05: This is probably like Instead of having a binary decision of stop or don't stop, I would implement multiple response level like. 
 17:14: risk is like smaller than 60%, then continue. 
 17:18: This is, this is between the 60 to 80% alert operation risk. 
 17:23: It's like 80 to 90% reduces speed. 
 17:26: Risk is like greater than 90% than the stop. 
 17:29: So that allows us to match the operational response. 
 17:36: OK. 
 17:37: All right. 
 17:37: what can you tell me about the safety? 
 17:41: Safety For like the safety perspective. 
 17:47: Safety would be the like the highest priority requirement because The consequences of the missed detection could be a development. 
 17:56: When I think about safety, I think about designing the system. 
 18:00: So that the single failure does not result in an unsafe outcome, like no single point of failure like this, the first thing I would do is eliminate single point of failure. 
 18:13: OK, so the system should continue operating even one sensor type becomes unavailable, and we have also the multi-sensor validation. 
 18:20: Like I would not allow a single sensor reading to trigger like a critical safety action. 
 18:25: Multiple independent signal should agree before we make a strong decision. 
 18:31: Then for safety critical scenarios, I'd rather investigate the suspicious wheel than miss an actual defect. 
 18:40: At the same time, like. 
 18:42: We discussed, we, we like, we discussed the business impact or the false, of like false positive. 
 18:48: So I like used, confidence thresholds and thro response rather than stopping everything. 
 18:55: OK. 
 18:56: So we talked about sensors, avoiding single point of failure. 
 18:59: Now, what about the rest of the components here? 
 19:03: OK, how do you ensure that, for like the rest of the components, generally, Like, I would not run a single detection in an instance like I would deploy the multiple instances behind the load balancers or like use active active active processing. 
 19:24: So like we have the detection engine and in that like we have instance ABC. 
 19:28: So if one instance fails, another instance continues processing inspections events. 
 19:33: So the, and also the correlation service like. 
 19:37: The coalition always is like critical. 
 19:40: Because if it fails, we lose the ability to associate defects with specific wheels. 
 19:49: OK. 
 19:51: so, from overall, the system, what can you tell me about, security? 
 19:59: Overall security. 
 20:03: Like. 
 20:07: How secure the system? 
 20:08: Yeah, like for a system like this, security becomes like especially important because we are like dealing with the safety critical operational system. 
 20:16: So a malicious actor should not be able to manipulate, infection. 
 20:21: It also trigger falls in stops. 
 20:24: So the first thing I had secure is the inspection station itself. 
 20:28: So these devices are like physically deployed in the field, so they could potentially be tampered with, like, for example, in the secure boards are signed from the device certificate. 
 20:40: So only trusted software, software should be allowed to run the like inspection hardware, and we have also secured the communication. 
 20:48: Like all communication between components should be encrypted in transit. 
 20:54: And also the access control, like not every user should have the same level of access, and the data integrity is also important like. 
 21:03: One of the biggest concerns would be ensuring that the inspection data cannot be altered. 
 21:16: All right, yeah, do you have anything more to add to this? 
 21:22: no, like, not yet. 
 21:25: OK, right, can you please, you know, do an export to PDF or PNG and then paste it in the chat that way I can add it to your, yeah, sure, right back. 
 21:37: Just give me a second. 
 22:31: OK OK, cool. 
 22:36: I see it. 
 22:37: Thank you. 
 22:38: Let me go ahead and save this. 
 22:51: so what questions do you have for me? 
 22:54: know. 
 22:56: Honestly, I like, currently I like don't have any questions. 
 23:00: OK, OK. 
 23:03: That's fine. 
 23:05: so that's all I had. 
 23:07: thanks for your time, Mike. 
 23:09: That was good talking to you. 
 23:10: Yeah, thanks, thanks. 
 23:11: Goodbye. 
 23:12: Same to you too. 
 23:14: Yeah, see you bye-bye. 
