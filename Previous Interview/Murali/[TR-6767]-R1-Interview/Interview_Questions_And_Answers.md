0:00: Hey Maur, hi. 
 0:02: Hi, how are you? 
 0:03: Yeah, I'm fine. 
 0:04: What about you? 
 0:06: I'm doing good. 
 0:07: Thank you. 
 0:07: And thank you for joining the call, last minute. 
 0:10: I know this was, It was a short time, from the meeting invite, to the interview, but I really appreciate your time. 
 0:21: No, so, let me get started, Marie, before we get started, right, do you have your ID, handy with you, and, do you mind if I record the session? 
 0:35: Yes, yes, yes, you can. 
 0:36: Yeah, you can record it, but now I don't have like, now I don't have my ID. 
 0:43: So like I have my ID, but I'm not taking it like for the session. 
 0:49: After the session, like, I will show you and like. 
 0:53: OK, yeah, sounds good. 
 0:55: All right. 
 0:56: So, before we get started, I'd like to introduce myself to you and then we can, go about, you know, discussing your background and your experience. 
 1:06: So I'm a coacher. 
 1:07: I'm part of cognizance's, business enablement team, I work for various verticals like healthcare, life sciences, comms media technology. 
 1:20: So this requirement is for a coms media technology client. 
 1:26: you will have more details about the client, in the next round of interview, but, yeah, so mainly my role is to take care of all their, resourcing needs and, on a program level, you know, their projects as such. 
 1:44: So, yeah, so, I. 
 1:49: I like to keep this conversation, casual and not, specific to interview questions. 
 1:56: My main goal is to understand your background, your experience, and how it aligns, with the, the requirement. 
 2:05: So, I have your profile with me, Murti. 
 2:08: your background shows extensive experience across Python, fast API, AWS, Terraform, distributed systems, event-driven architectures, and cloud native platforms, right? 
 2:21: So I'd like to spend some time understanding the scope of our architecture. 
 2:26: ownership that you've had, and how you've driven architectureural decisions across organizations, and mainly your approach to governance, scalability, and technical strategy. 
 2:39: So, could you tell me about the The largest platform you've architected from scratch, in your experience. 
 2:48: Yes, yes, yes. 
 2:49: So like, absolutely over the last several years, my role was involved beyond just application development into the platform architecture and like technical leadership and also my focus has been on designing and the cloud-driven event-driven events and platforms that are scalable and secure and like easy to maintain. 
 3:11: So like the, yeah, yeah, yeah, the platform was designed to integrate and process the data for multi multiple healthcare systems such as like, you know, EP EMR and HL 7 interfaces and the claim systems and also working on laboratory systems and the third-party applications. 
 3:30: So most like since the system generated large volume of data and consistency, and one of my like, primary responsibility was designing an architecture that was scalable and like, easy to maintain from the architectures like stand, standpoint, like I support and I possess the microservices-based architecture and using the Python API and which like, like each services has like clearly defined responsibility to such as in like injections, validations. 
 4:03: And like also transforming and reporting API management. 
 4:07: So these services we're like containerized using Docker and like deploy on AWS EPS. 
 4:14: So like, like which is most of the time we are using cloud side and I lead architecture decisions and around the using AWS services, I like, we are using AWS services in EKS SD. 
 4:28: RDS, Lamra, IAM, and Cloud Watch and also working on secret managers. 
 4:34: So I also work closely with the enterprises architecture and like security team and the product ownerships and also working with the engineering leadership to review architecture and decisions. 
 4:45: So yeah, it's a little bit about me. 
 4:48: All right. 
 4:49: And how do you govern architecture, sorry, excuse me. 
 4:53: How do you govern architecture across multiple engineering teams? 
 4:58: OK. 
 4:59: So, like, At the time and most of the time in like my experience with the architecture governance is like about establishing and the standards like while giving engineering teams to like flexibility to deliver efficiently. 
 5:15: So on my current project, we defined like common architecture guidelines for microservices and API design and security logging and monitoring. 
 5:26: And also like we are deployed for deployment to the like team follows and the same approaches and also most of the time, we standardize CICD pipelines using gate of actions and infrastructure, like using throughout the terraform and helms and like container deployments on Amazon EPS. 
 5:49: So, Ensure, like ensure consistency. 
 5:52: We are conduct the architecture and design review and I work closely with the architecture, like architectures and the technical leads and using product owners and discuss design decisions. 
 6:04: So yeah. 
 6:12: Sorry, I was stopping on mute, my apologies. 
 6:16: have you ever rejected a proposed solution, and what was the reason behind it? 
 6:21: And, how did you communicate any concerns, if there were any, and, any alternative, If it was proposed, so yes, I like, yes, I have like one of example during my current healthcare project, a team, like a team proposed building a tightly coupled services that directly communicated with the multiple downstreams. 
 6:48: Systems and also contain business logic specific to the A system and after that, during the architecture review and raise the concern because of the approach, you know, like would make the services different to maintain and harder to scale and also change in one downstream systems and also like. 
 7:09: cloud impact the entire application. 
 7:11: So instead, like instead of that, I recommended, splitting the functionality into the independent microservices with, clearly defined risk APIs and separating the business logics into the individual services. 
 7:26: So we also standardize the data, like the data construct to the each services had a clear responsibility. 
 7:33: And I think although we are using a little more efforts initially for the new design and the mid platform like deploying services independently. 
 7:46: OK. 
 7:47: And what architecture modeling techniques do you typically use, Are you familiar with C4? 
 7:56: Yes, yes, yes, I'm familiar with C4 working on it. 
 8:00: And how do you document architecture? 
 8:04: So, like, I documented the architecture using like most of the time we are like using import part of my role. 
 8:13: So where we are designing new solutions or make a significant archi architectural like changes and I make sure it's properly documented, so that's developer and architects and operations team. 
 8:27: And like the stakeholders all have one common understanding. 
 8:32: So typically the documents, like the documentation includes the business problems and the architecture overview and like using C4 diagrams, component like component responsibilities and API contracts and also working data flow, deployment architecture. 
 8:48: So like, with the, like behind them. 
 8:53: And for my recent healthcare platform, we documented the end to end architecture includes how the data flow and EP EMR and HL 7 interfaces and other healthcare system through the past API microservices and also Apache AR4 pipelines. 
 9:13: So, and, and it did like disaster recovery and consultations. 
 9:23: All right. 
 9:24: can you walk me through how you would document a microservices platform? 
 9:29: Yes, yes, sure, sure. 
 9:31: So, like, document the microservices platform, like we have the documenting microservices platform, I would like, structure the documentation from a high level business view and like down to the implementation details so that various stakeholders like from business users to the developers and most of the time the operations teams can understand the system. 
 9:55: And like I will start the extensive overview and explaining the business business problems, and the platform solves the key objective and the major capabilities to the improve and provides. 
 10:08: And next, I create the system contacts diagram and showing the, like, you know, external users and the system intact and the platform and in my healthcare project, for example, like. 
 10:21: This includes EPGMR, like I already talked with you, EPGMR and HL 7 interfaces and claim systems, laboratory systems. 
 10:30: So like it's interacting with our own platform. 
 10:35: So that like I have documented the container architecture and like it's identifying all the major components such as fast APM, microservices, Apache Airflow, Amazon EPS, and also working with RDS S3 Lambla. 
 10:51: And external APIs along with the communicate and after that I have like documented that each microservices individually and includes the business responsibility and API endpoints and like, you know, the request and response format so working like go through that, go through with this and like for the development teams we work independently. 
 11:18: OK. 
 11:19: And when a new project comes in, right, so how do you assess technical feasibility? 
 11:24: So basically, what factors do you consider, Yes, yes, so, yeah, you can continue. 
 11:34: No, no, that's what I was asking. 
 11:37: Yeah, OK, OK, so when a new project comes, like comes in, like I first spend the time understanding the business objectives and the functional requirements. 
 11:47: So before thinking about the technology and like I want to clearly understand what problems we are trying to solve and what we like success looks are. 
 11:57: And next I like, you know, evaluate the existing architecture and identify. 
 12:04: like whether we can reuse any existing services or platform components instead of building everything from the scratch, and then I access the technical requirements such as scalability, security, platform like performance and availability, and also like compliance and like integration with the existing system. 
 12:25: So we are, we are going with all of them. 
 12:29: OK. 
 12:31: And how do you estimate engineering effort for large initiatives? 
 12:37: OK, OK, OK. 
 12:38: So like. 
 12:40: Most of the time, the large like large initiative, I first break the project and down into the smaller downstream such as like architecture, backend services, integrations, and like database changes and also infrastructures and testing and deployments. 
 12:57: So like estimating the, like, you know, the work stream level such as such more accurate than estimating the like project as a whole. 
 13:07: So, like, next, I identify dependencies, technical risk, and like any unknown that like could impact the timeline and after like I also account for non-functional work such as security monitoring, documentation, and like, you know, performing testing and production rollout. 
 13:28: So my recent, talking about my recent project, so we are also working on it. 
 13:33: And like it's a healthcare project so we estimated the efforts separately for fast API microservices, Apache 2 pipelines, AWS infrastructure, and also working with the Kuberne deployments. 
 13:45: So like it's trying to deliver like everything at once. 
 13:50: Mhm. 
 13:51: And what is the most important technical strategy decision you've made, in your experience in the last few years? 
 13:59: OK, OK. 
 14:01: So, like, technical decisions, one of the most important technical strategy, strategy decision I made was like Recommending a cloud native microservices architecture instead of like existing the monolithic applications for our healthcare data platform at the beginning of the project, like we knew the platform had to integrated data from multiple sources like EPG. 
 14:27: Like EP EMR HL 7 interfaces, claim systems, so like it's supporting the like for the AI analyst AI analytics work workloads and the monolithic approaches will like have made scaling deployments and feature enhancement much more difficult. 
 14:46: So like, yeah, I recommended build AI independent fast API microservices and running on AWCPS. 
 14:53: So like looking back the architectural decision, like provide the flexibility and scalability and for the, for the like for growth. 
 15:05: Got it. 
 15:06: And, so, this is just a hypothetical, kind of a scenario, right? 
 15:15: So imagine, the organization that you're working in wants to build a global content management and AI powered asset. 
 15:26: platform serving millions of users. 
 15:29: the platform must ideally support cloud native microservices, AI integrations, terraform managed infrastructure, distributed workflows, media processing, search, and global scale. 
 15:46: can you walk me through your architecture, governance model, deployment strategy, Could include security controls. 
 15:58: And operating model for this. 
 16:01: OK, OK. 
 16:02: So, let, let me think a little bit. 
 16:05: I, I can, I can type down the question if you like, just stop me or, or ask me any questions if you've missed anything. 
 16:14: No problem. 
 16:15: Like, I just remember a little bit, like it's a big question. 
 16:20: So, like, first of the name, like if I were designing a platform like that, I start my understanding and the business goals, expected traffic, compliance requirement, and the AI use cases before selecting the architecture. 
 16:39: So, from an architecture perspective, I would like to choose a cloud native microservices architecture running on Kubernet such as Amazon EAS, such as like. 
 16:49: Capability content and management and also like assets management, media processing, search, searches and user management and AI services like, it would be implemented as an AI independent microservices with, like, you know, well-defined APIs. 
 17:11: This allows the team to develop and like also deploy. 
 17:15: And the skill services independently for media processing and like distributed workflow, I would use to event-driven communication like whenever the approach is, for example, for example, like when a user like upload an assets for an event. 
 17:36: Like will trigger background services to the validate files. 
 17:41: After that, generate the thumbnails, extract metadata, and also involves the AI services and tagging all classifications for the storage, I would use Amazon S3. 
 17:53: And also like for the assets and Amazon RDS for the transactional data, search capabilities and could be implemented using a dedicated search and services so users can, you know, quickly locate the content based on the metadata and AI generated text from like, from the infrastructure perspective, I will manage everything using the infrastructure. 
 18:17: For the like code with the telecom and packages application with the doctor and after that, the, like for the governance, I would establish architecture and like standards for the API design and security and also like logging and monitoring and naming convention and also checking the CICD pipelines for like for security. 
 18:42: I would like to implemented IMB and like, you know, last privilege, privilege access and after the success and using the, like secret managers for like credentials and TLC for the encryptions and also. 
 19:02: Also, like, centralized monitoring and using cloudou. 
 19:06: Yeah. 
 19:07: And after that, anything like that, yeah. 
 19:11: Perfect. 
 19:12: I forgot. 
 19:15: No, no, I, I think you pretty much covered, everything. 
 19:20: so, only on, So you're currently located in which area? 
 19:27: Yeah, I'm in Pennsylvania. 
 19:30: Pennsylvania. 
 19:30: OK, so this is mostly, a remote role. 
 19:35: So if your profile gets, shortlisted, right, so how early would you be able to join in? 
 19:41: Are you currently working with any of the clients? 
 19:45: Yes, yes. 
 19:46: So now my contract is going to be ended like in this week. 
 19:51: So after, like, after the week I'm immediately joining. 
 20:00: OK. 
 20:01: All right. 
 20:03: Take pictures. 
 20:16: So, I can't you, like your voice is not like a little bit breakable. 
 20:22: Can you hear me now? 
 20:25: OK. 
 20:25: So I was just saying that that's pretty much from my side. 
 20:29: I just wanted to kind of understand your background, your experience, and how it aligns with the requirements. 
 20:36: I will share your profile internally with the team. 
 20:39: I might have to ask you to tweak your profile a little bit. 
 20:45: aligning your experience, and, there is a certain criteria how the clients, kind of shortlist, the profiles. 
 20:55: So I'll share a dummy profile with you, a template, and, I might ask you to update or tweak your profile, accordingly. 
 21:05: And, share it back with me at the earliest possible. 
 21:09: and if you have any questions, in the meantime, you can always reach out to me on my email ID and, you know, I'll be happy to help. 
 21:17: So, yeah, that's, that's also my end at this point in time, and it was wonderful connecting with you. 
 21:25: It's nice talking to you. 
 21:29: Yeah, thank you so much. 
 21:30: Thanks. 
 21:31: Yeah, thanks for connecting. 
 21:33: Yeah, bye bye. 
