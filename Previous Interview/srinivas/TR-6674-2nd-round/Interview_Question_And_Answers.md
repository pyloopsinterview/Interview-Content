0:00: It's, it's Adam, and yeah, there's you, OK, there you are, 3 of us, all right. 
 0:04: So yeah, and I'm a different Ryan is recruiter Ryan, so I'm a different Ryan, but, yeah, so I was just trying to make sure you got connected with and see if you're doing so you're talking with Adam Jena from Corteva. 
 0:15: So I hope you guys have a great conversation. 
 0:18: Perfect. 
 0:18: Thank you, Ryan. 
 0:19: Yeah, see you. 
 0:22: Hi. 
 0:22: Nice to meet you. 
 0:23: Nice to meet you, Adam. 
 0:24: How are you? 
 0:26: I'm doing well, thank you. 
 0:29: So I was hoping I can learn a little bit more about yourself and you can tell me a little bit about the things that you've been working on and what you've been up to, and I'll take a moment to talk to myself and my team and the things that we've been working on and then we'll dig into some questions. 
 0:43: Does that sound good. 
 0:48: So how about you keep this up so can you tell me a little bit about what you've been working on. 
 0:54: How about you kick us off? 
 0:55: Can you start off by, talking about some of the things you've been working on recently? 
 1:00: I don't know. 
 1:01: So hi Adam. 
 1:02: My, my name is Shiraz. 
 1:03: I'm a Python backing and data platform engineer with around like 12 years of experience building like scalable enterprise applications, like APIs, cloud-ned platforms, like, like foundational data services that you know, supports mission critical business operations. 
 1:19: So like my expertise is primarily focused on the Python backend development. 
 1:23: And like distributive systems, API engineering, microservices architecture, cloud platforms, and like. 
 1:31: Large scale data processing like solution using technologies such as Python, Fat API, Postress, AWS, AW Slamba, Docker, Kafka, Rapid MQ, and so, so many like my Microsoft Intra ID, Azure, CICD workflows. 
 1:45: So yeah, so like currently I'm working as a, I mean working on a like large scale healthcare platform supporting like tenet healthcare, like, where I contribute to the, you know, development. 
 1:56: of like foundational backing services used to like across multiple enterprise applications and much of my work focuses on like building the and maintaining like core platform services, related to authentication, authorization, user identity management, and secure data access and like which, which, which are consumed by the various, business and clinical applications across the organization and like. 
 2:24: like, in addition, like I worked on like implementing like fine-grained authorization models using relationship-based access concepts and policy-driven like access controls to ensure that, that users could access only that, that data and resources like relevant to their roles and organizational relationships. 
 2:44: And like, like the platform is like, also included like location-based, healthcare data services where like geospatial, information such as facility location, service regions, and patient access zones, were like managed and exposed to secondary care and where my my like My, my primary, focus was like back in engineering, and I collaborated with teams like leveraging geospatial technologies, like, front-end applications to deliver like location aware functionality across the platform. 
 3:21: So yeah, this, this is all about like, and what excites me is about the like this opportunity and this, the focus on the foundational platform engineering and authentication authorization services. 
 3:32: So yeah, I'm also looking for, I mean seeing work or like rela related work about the which, which I'm also have worked throughout my career, so yeah, that's why I'm I'm just interested in that. 
 3:47: That's fantastic, and I, I appreciate the background. 
 3:50: it sounds like you have some really great experience working on very similar technologies that we're here using here at Corteba, so that, that's great to hear. 
 3:59: a, a little bit about myself. 
 4:01: My name is Adam Johnson. 
 4:02: I've been with for 15 years working within the research department. 
 4:07: my team right now, it works within a project called Granular Insights. 
 4:11: We have several teams working to deliver the same product. 
 4:14: We use Python microservices and eventual consistency to collaborate across the team to keep, team working independently from each other but also within the collaboration, that comes with that. 
 4:28: specifically bringing insights is a, a tool that helps deliver agronomic. 
 4:33: Information to the, the pioneer the seed fabrics. 
 4:37: So they're trying to help the farmers find the right products for what they're trying to grow their operation and there's lots of different insights that they can provide of analysis that they provide on their reading geospatial rosterization of images, like soil information, weather information, as well as like growing grape and things like that, although aggregated for farmer, on their behalf. 
 5:00: so it's just a nice, nice display for them to see into their, their operations on a day to day basis. 
 5:07: my particular team touches on a lot of things that we touched based on, which is we handle the authentication and authorization for the entire department, as well as those core data concepts like what's the virus operation and what are the fetal boundaries. 
 5:22: And so we, we, we do all this through using Python. 
 5:25: we have Microsoft as our identity provider, but we, and we also provide, a Reebok style authorization model. 
 5:34: OK, OK. 
 5:38: any, any questions I can answer on that before we hop into any other questions? 
 5:42: No, no, I don't have any questions. 
 5:44: question. 
 5:47: Sounds good. 
 5:48: Well, I'm, I have some questions here that are relevant to some of the things I just touched base on, and we'll, we'll just dig into the different pieces there. 
 5:56: OK. 
 5:58: So, so to start us off with, you mentioned you have a background in Python, and one of the things that we noticed that, you know, as the transition from Python 2 all the way to Python 3.14, 1 of the things that has evolved several times over that time frame is how Python develops asynchronous programming. 
 6:18: from your perspective, when would you apply asynch weight and when would you consider different approaches from using ay rate? 
 6:28: OK. 
 6:28: Oh yeah, for like, as we know that, yeah, Python can really well handle the Aingeing programming and in, in its structure. 
 6:36: So, first of all, that's a great question. 
 6:39: So that's why, like I typically use async of it when I'm dealing with like input outbound operations where the application spends like time waiting on external resources such as database calls, SJPI calls, message queues, or like cloud services I'm working on. 
 6:57: like, on the other hand, like if I'm working with like, intensive tasks such as, large scale calculations, image processing, or like, you know, heavy data transformations on, on machine learning workloads, so you think AV doesn't provide much benefit, because the CPU remains, you know, busy. 
 7:17: So in, in such situations like,, I would like to look at the alternatives such as multi-processing, distributed workers or like AWS lambda paraization. 
 7:29: So, or, or like background processing frameworks, which, at least so that, we can, we can get the optimal results. 
 7:37: And in, in my mind, general rule is like. 
 7:40: I mean, is that like do you think of what is most effective for high concurrency and input output services like input output heavy services, but which is why like, it, it's commonly used in CPI, like, modern microservices architecture for CPU bound workloads. 
 7:58: I prefer approaches that are leveraged, like that can be, leveraged like multiple courses or like separate work processes. 
 8:06: So this is the, I mean, in my practice, I try to evaluate the. 
 8:10: Bottle bottleneck first and like if the services is services is spending like most of the time waiting on external systems so I think is usually a good fit and if it's spending most of the time like processing computation that like other concurrency models are often more appropriate than I mean in that case yeah. 
 8:33: So we then 3 more, we, we found the same thing that typically fanning out across multiple processes and things like is more often a better solution than unless, unless they've been something very high and focused, you're right, but that the senses the alternatives to perse pretty sure that. 
 8:53: OK. 
 8:55: So let's say that then you you're delivering an API that exists today, and you are going to introduce a breaking change to your clients. 
 9:05: So something about your API is changing that will break your clients and make them no longer work. 
 9:10: can you describe what a breaking change would be to your API and then what steps you take to help mitigate that breaking change. 
 9:17: OK, OK. 
 9:19: In that case, like, first of all, I'll have to look into, I mean, look through that very properly, and, like, what steps for, for, I mean, before taking the steps, like, sure, I, I can break, making changes is, is in any modification to, if that. 
 9:35: Contract that causes like existing consumers to feel without making changes on their side. 
 9:40: So like if it for example it's like if they are currently like returns a field called customer ID and and we renew it to the client ID. 
 9:51: So existing application that depends on the customer ID would break, of course. 
 9:55: And similarly like removing fields, changing like data types or modifying response structures like changing required like request parameters and or like al altering the endpoint behavior can can all be like considered making changes like. 
 10:13: Then when introducing like breaking change or my first preference is to, you know, avoid, breaking consumers altogether. 
 10:20: Like if, if possible, I would maintain a backward compatibility by keeping the existing contract and like introducing the new functionality along with it, alongside it, and like If, if, baking change is unavoidable, then I would typically like to introduce API versioning such as like we, we do that like creating, we do V2 endpoint or like V1 endpoint. 
 10:44: If it's, there is no V1 endpoint, then we can start with the V1 endpoint. 
 10:49: So, you know. 
 10:50: Like continuing, like to, to support, you know, for, for a defined period. 
 10:55: So this, this like gives you the consuming teams, time to migrate without, disrupting their applications and I, I would also communicate like That change early and like provide like updated documentation, migration guidance, and like sample request and responses. 
 11:14: In addition, like I would use automated integrations and like contract testing to verify that. 
 11:21: Both versions behave as expected and like before, deprecating the old version, I would monitor our users to, you know, understand which consumers are still using it and work with those teams to complete the migration. 
 11:36: So in general for dog like. 
 11:38: Platform services that are, you know, consumed by multiple teams. 
 11:42: I view like API contracts as long-term commitments first of all. 
 11:47: So I try very hard to evolve like APIs in a, in a way that minimize disruption and like gives consumer, consumers a predictable migration path at least. 
 11:58: So that's my approach I would say. 
 12:02: Excellent to you. 
 12:02: Thank you very much for the day. 
 12:06: I, I agree, and we often are locked, we feel locked in at times to the API contracts that we deliver, and we have to support them for a long time and, and delivering new versions is a great way to mitigate that and helps a lot in making sure we have a a migration path all of the versions and it it's a process. 
 12:26: It takes time, but it's, you know, better to bringing people in life for sure. 
 12:32: so, right, so we have this API, we're hosted on AWS, for example, and we now we have to make a decision on how do we persist the data that we're representing with the API. 
 12:44: Often choices we use here at Winteva is PostS SQL and then Dynamo DVD. 
 12:49: And so I'm curious, when evaluating which technology we use, what are some considerations that you decide between, NoSQL database and relational database? 
 13:00: Got it. 
 13:00: Got it. 
 13:01: So, like, of course, like, this is a very, very, important question comes around when, when we are going to have to choose the database, what kind of database we have to work on or work with for a long time. 
 13:12: So, for, for me that choice usually starts with the, I would say access pattern first of all, like. 
 13:19: Data relationships, what we have to like create or like is scalability requirements also like, like consistency needs to needs of the application that that that matters for choosing this making this choice. 
 13:33: And if the data has complex relationships like requires joints, transaction across like multiple entities, or, or like we want a strong consistency or a well-defined schema, then I generally lean like towards our relational database like post resistor. 
 13:50: So for example, like involving users permissions and or like some transactional business data like often fit fit very well in the, you know, relational model because like the relationships are, you know, important and data intellig. 
 14:07: Data integrity is also critical here. 
 14:09: So on the other hand, if like, if application requires really high scalability, like, predictability, like, it, it has a predictable access pattern only. 
 14:20: So low latency lookups or like flexible schemas, then are like there are no sequel solution like Dynamo DV can be a great fit for that. 
 14:29: Dynamo DV works like especially well when, you know, when you have You know your access pattern like upfront and like can can design your partition keys and indexes around those patterns only. 
 14:43: So in my experience, like it's really about one database being, being better than the other. 
 14:49: It's more about like choosing the right tool for the platform. 
 14:53: So for example, like in a, in a platform like handling authentication and authorization data, I would likely favor like with the festival, because relationships and consistency are very important here. 
 15:04: So but if I were like storing large volumes of event data or like session data or cache information somewhere or like how to to put look look up data I have to see. 
 15:17: So Daniel Levy could be the better choice for that. 
 15:19: So I also look at like Operational considerations such as like scaling requirements, maintenance overheard or like disaster recovery is there or or or or one of the important like consideration is cost so dynamically we give, gives you a lot of managed scalability like while post SQL such as like powerful querying capabilities and like you know it's strong relational modeling. 
 15:46: So my approach is always like to start with the business requirement as I see and access pattern first then choose the database technology and that best is the requirement. 
 15:59: Mhm Please. 
 16:02: OK, so what's happened in this particular case, we have, a postscript database, a relational database, and now we have an existing table we can call customers, for example, and it has columns and orders ID, the name of the customer, etc. 
 16:17: etc. 
 16:18: and we want to add a new non-nodeable column to the table. 
 16:23: How would you go about adding that column to the table and what steps would you take to avoid a downtime? 
 16:30: OK, OK. 
 16:31: So for that purpose, like, if I have to like how would I about adding the column to the table, so, like If, if that table like already exists, contains data, and I, I need to add a new column then, or new non-enable column, so I, I, I would be careful not to introduce the column as non non-nullible immediately because like that could fail for adjusting records and potentially impact the application availability. 
 17:04: So, so my typical approach is, is, is like it's a phased migration I would say. 
 17:11: we are going to do the migration in phases. 
 17:13: Like, 1st, 1st phase you can choose. 
 17:15: Like I would add the new column as nullable. 
 17:18: this is generally like, see if a schema change, allows the database migration to compete without affecting existing rules. 
 17:27: And next I would, deploy and, you know, application change that that it starts populating a new column for all newly created or updated records at the same time. 
 17:38: So at the same time, like, I would also would, backfill the existing data and usually through control migration script for batch process. 
 17:48: So once I read, I would verify like that all existing rules have valid. 
 17:54: Values or and like application is consistently writing the writing to the new column then I would run validation checks to confirm that there are no null values remaining. 
 18:06: Finally, in, in a separation migration, I would, like, you know, like, in our, in our last migration, I would say it's, it's a final migration. 
 18:14: I would add the no non-con constraints to enforce the requirement at the database level. 
 18:21: So this, this, this phased approach I would avoid, in my point of view, like it avoids the downtime because, you know, the old and the new application versions can, can coexist and during the migration also, and we are not making assumptions about data that already exists in the table. 
 18:39: So, in general, like when, when working with the production systems, I would prefer like, expanding the schema first and migrating the data, then only like then enforcing strict stricter constraints that reduces the risk and allow for, allow for the safer deployments. 
 18:59: That's your rash. 
 19:01: I appreciate it. 
 19:03: And, and so we have this API thing and it let's say that it still has that posters database and so now one of the decisions we need to make is how do we expose this API, how do we host this API to our clients to consume. 
 19:17: We've already talked about a little bit about Lambda, that, you know, and AWS has lots of options for hosting Lambda Institute, etc. 
 19:24: etc. 
 19:25: what considerations do you put into your hosting platform and servicing like this kind of application? 
 19:33: OK, so, like, while choosing the, like, booking platform you were saying like, yeah, so yeah, yeah. 
 19:43: Like when selecting a hosting platform, I would usually like, start by, you know, understanding the application's requirements first, like rather than picking a technology first because we would first of all we have to understand our requirements and the main thing I would, evaluate like, first of all that traffic patterns. 
 20:02: Or like scalability requirements or like latency expectations like operational overhead system and also as I say like cost or security requirements or what I mean what is the requirement for that and also like it it can depends on the Nature of the workload, like what kind, what kind of work. 
0:00: Also, as I say, like cost or security requirements or what, I mean, what is the requirement for that. 
 0:06: And also like it it can depends on the Nature of the workload, like what kind, what kind of workload do you want to put on that particular cloud platform. 
 0:17: So, so on the other hand, like if, if, if the application has like long-run connections, that requires more control over the runtime environment or has the predictable, high, I would say. 
 0:31: traffic or, or like involves the complex background processing, then, then we can choose the services running on the ECS or EKS or, or even EC2 might be a better fit. 
 0:43: if for the previous example, if I, I'm thinking right now like, if the API is even driven. 
 0:48: And has the available traffic or like doesn't require long running processes. 
 0:54: So then EWS lambda is also often a strong option for us. 
 0:58: So it provides the automatic, scaling and reduce the infrastructure management and can be very cost effective for workloads that are not running continuously. 
 1:08: So that is the approach I mean, I would take for choosing the services and, I also like consider operational factors such as deployment strategy, observability, or like, you know, logging and disaster recovery and, and like team expertise. 
 1:27: So, so, you know, sometimes that technically. 
 1:30: Best solution is the, you know, best business solution. 
 1:33: if it's, if it like introduce operational complexity, that the team isn't prepared to support them, it's, it's not going to be the best, option to, I mean, work with, with the work on like for the team. 
 1:46: So for an API they can buy like. 
 1:49: With this SQ and I would like also look at like connection management with lambda, for example, like database connection handling becomes, you know, an important consideration because rapidly scaling can create large numbers of connections and in those cases like solutions such as connecting connection pooling or RDS proxy can help us in, in that case. 
 2:12: So ultimately I try to balance the sustainability or reliability. 
 2:16: Cost and all also the maintainability so that right hosting choice depends on the, you know, workload characteristics and like long term operational needs of the platform. 
 2:25: So that would be the approach overall approach I would take, Adam, so that. 
 2:30: we don't have to, you know, while after choosing that, we, we are rethinking about choosing our choices. 
 2:36: So yeah, I think that's, overall approach I would take so that, once we, we choose the right platform and right service, then we are good to go. 
 2:45: Then we also just work. 
 2:47: So yeah, that, that's what my. 
 2:51: If that's. 
 2:52: I was actually gonna follow up my question about some connection for me, and you, you've popped right into it, so I, I appreciate you going the attention to that. 
 3:02: just, just a bit of a little bit, And we, we've talked about authentication and authorization and your a little bit of your experience with it. 
 3:11: So just at a high level, can you break down authentication versus authorization of what each term means, and then we'll dive in a bit more from there. 
 3:18: Of course, of course, a very, very, very famous question, a very basic to question, yeah. 
 3:25: Yeah, thanks a lot for asking this because it's one of the favorite question we we just like to talk to you because the situation happens to us like when are you the logs into our application. 
 3:36: To revalidate their identity through an identity provider such as Microsoft Intra ID, once the user is successfully authenticated, the, the identity provider issues a token, like typically, AWT, that contains information about the user and their identity. 
 3:54: And, on the other hand, like authorization happens after the authentication, like once we know. 
 4:00: Who the user is, then we evaluate like whether they have permission to perform a particular action or access a specific resource. 
 4:09: So, for example, like in a healthcare environment like a user may successfully like authenticate through a Microsoft ID but that doesn't, you know, automatically mean that they can view every patient report. 
 4:22: So the authorization layer determines whether that authenticated user has the, you know, appropriate permissions or relationships required to access that specific data. 
 4:34: So, authentication answers the question like who are you and, the, the right authorization answers question like, what are you allowed to do? 
 4:43: So that, that's what I would summarize, and this is the famous I would like to see about the authorization and authorization because that's just some of the answers. 
 4:52: So yeah, that's happened. 
 4:55: Absolutely, and you already touched on it a little bit of authorization, but, can you explain some of the authorization concepts, and when you deploy one over over another, yeah, yeah. 
 5:09: So of course authorization has different concepts available here. 
 5:14: So like there are several authorization models out there. 
 5:17: So, that, that right choice really depends on the complexity of the, you know, business requirements and how access decisions, needs to be made. 
 5:26: So the most common model is, our back or the rule be access control. 
 5:30: So, and like there is also like, reback like with, which, which. 
 5:36: Relationship-driven, access, it provides like very useful in the complex enterprise systems and also there is AAC like which is flexible, attribute based rule rules. 
 5:47: so that's how like, we can, I mean, there are different policies. 
 5:51: So, if I talk about the, normal success control which is very famous and mostly used, like in the, in the scenarios. 
 6:00: So like in such roles, like, Such as roles have like admin, manager, sales, or like viewer or users inherit permissions through, through those roles and our back is relatively like, you know, simpler, simple to implement and work well when when you know access requirements are fairly consistent like across a group of users and all so, and if I talk about another model. 
 6:31: EBAC. 
 6:32: So, EBAC is a relationship-based, access control, and like, which is, which I have worked with my, in my current healthcare platform like in Rebok, like access decisions are based on, you know, relationships between entities. 
 6:45: For example, physician may only be allowed to access our patient record, if there is a valid relationships, between the physician and the patient and the healthcare facility, is present there. 
 6:58: So this model works, you know, very well when the access depends on the business relationship rather than just a static rules. 
 7:05: So that's how, I mean, the back is very, useful in that case. 
 7:10: if I talk about the attribute-based, access control, then it can be very useful, when access decisions are based on the attributes of the user like, or, or, or like of the user or the resource or for the environment even. 
 7:25: Like, the, for example, like, access might depends on, on a user's department, location, time of the day, resource classification. 
 7:36: So this provides like more flexibility, but, but, but can more, complex to manage. 
 7:42: So this is the, I would say attribute based role, role access control I mean provides you. 
 7:49: And for me, like, RBAC is greater, I mean great for simpler organizational permissions. 
 7:56: ABAC is like, I would say useful when attributes drive, you know, assess decisions, and EBA is like often the best fit when relationship between the users and the resources are central to the authorization model. 
 8:09: So these are the few, I mean, I would say, rules, and other than that, like, there are other rules also like, which provides you like, such, such, and. 
 8:19: Which is similar to the EBAC and the RBAC. 
 8:22: So yeah, so these are the major models I, I remember, yeah, I don't know about and policies and enforcement are the different ones with which we can work on and those views, very nice. 
 8:33: So yeah, I know about those, but never got the chance to, you know, work thoroughly on this. 
 8:40: Absolutely, and we, we mostly use Reebok and AOC within our organization. 
 8:45: So what, what you're saying rings true for me as well. 
 8:49: So, we also use Microsoft Intra as our authentication, our identity provider for our, our authentication, and one thing that we adds a bit of complexity there in this book you mentioned the is help with with JWTs. 
 9:05: however, we have customize the JWT a little bit before issuing it. 
 9:09: And do you have any experience with GWT customization from an identity provider, and if so, walk me through that experience. 
 9:18: Of course, of course, like, I have, really to use with, GWD customization from it. 
 9:25: Identity provider. 
 9:25: So I work with like JWT claims and JWT customization also like although like my involvement was has like Primary based primary being from the application and the back end integration side rather than being on the administrator or the identity provider itself but in our environment like after a user authenticated. 
 9:49: through Microsoft In entirety and, GWT contains, you know, standard claims such as subject to or audience or aspirations even like user identity identity information. 
 10:01: So you also like leverage the custom claims and like application specific claims that that could be done, you know, that could be used by downstream services for authorization decision. 
 10:14: So like if for example, if I take like certain business attributes like user roles or organizational identifiers and like group membership could be the, you know, included as claims within that token. 
 10:28: So our Python services would, like validate the token and then use those claims as input into the authorization layer. 
 10:36: So from a banking perspective, the important part was ensuring that the claims were trustworthy and like. 
 10:45: Validating the token signature and also like if you're like validating the token signature and the audience and the expiration, so they should be they validate and then using the claims consistently across the services. 
 11:00: So yeah, that, that's, I haven't like personally spent most of the time on the configuring like intro ID policies or like creating custom claims mapping within the identity platform itself, but I have worked like extensively with the consuming like customized GWT. 
 11:16: GWTs and like validating them and those using those like Custom claims to derive the authorization, decisions and distributed systems. 
 11:29: We, we do something very similar here. 
 11:30: We have our own organization ID that we admit in the claim, and it, it can be kind of tricky to get into the token, but like you said, once you have it there, you can make the authorization decisions based on that. 
 11:42: So I appreciate the call that. 
 11:44: OK, so, let, let's go back to that, conversation we had about the API where we were hosting something in AWS as its database back then, we've been making changes to it. 
 11:55: Here at Porteva we do CICD. 
 11:57: Any change that you make goes straight up to production, and so there's inherent risk that comes with that. 
 12:04: And in this particular example, let's say that we made a change and it caused an incident. 
 12:08: So we caused an outage for the our users, and now we need to work on making our services health again we get back to green. 
 12:17: Can you walk me through the steps that you would take to get us back to that green state? 
 12:22: OK, OK. 
 12:23: So for that purpose, like if I have to take the steps, back to that green state, so my first priority during, you know, incident, if like if restoring services quickly like, I mean, I would try to like do it as quickly and safely as possible. 
 12:41: So while understanding the root cause is important, so the imaging focus is, you know, minimizing user impact and, getting the system healthy again, first of all. 
 12:51: So the first thing I would, do to, you know, assess the scope of the incident, like I would, look at monitoring the dashboards and alerts like logs and the markets to, you know, understand what's failing. 
 13:03: So, how many users are affected and whether the issue was isolated to a specific service or impacting the broader platform. 
 13:13: So if the outage was, you know, was introduced by a recent deployment, which is often the case, I would, you know, immediately investigate that deployment. 
 13:22: So depending on the severity and confidence level, I would, like, I would typically consider rolling back to the last, last known good version. 
 13:31: To restore like, service quickly rather than, you know, trying to fix the issue directly in the production only. 
 13:37: So yeah, this, this, this restoring service I would communicate with like stakeholders or the other team. 
 13:43: So you know, so you can understand the current stereos and the impact is all so my. 
 13:48: once services is stabilized, I would dig deeper into the root cause. 
 13:52: I would review the application log, cloud watch matrix, and like, deployment history, also like database changes, infrastructure changes, or any like dependencies that that have contributed to the offensive infras. 
 14:07: So, after like identifying the root cause, I would implement a permanent fix, validate in the lower environments first of all, then deploy it to the normal CICD process and finally, like participate in the post incident review and the goal isn't just to, you know, fix the immediate problem, but to understand why, why, why it just happened and what improvements we can make. 
 14:31: So that would include adding data monitoring and improving the automated test and strengthening like Deployment safeguards or or updating the operational procedures to reduce the, you know, reduce the likelihood of similar incidents in the future. 
 14:51: So that, that's how like we can fix the problem and also like reduce the likelihood of similar incidents in the future so that like I said. 
 15:02: So, so my general approach is, is, like accessing the impact and restoring, services quickly, as soon as possible, and, like identify root cause, of course, and implement a permanent fix so that can improve the system based on the what we have learned. 
 15:19: So yeah, that, that's that. 
 15:21: After which I would think. 
 15:25: Thanks dude, I appreciate that, and I, I agree that that stabilizing first is always a good approach, so minimize the impact and making sure we can get us back online and figuring out what's going on and virtual right afterwards to to learn from it, so. 
 15:42: we got one more question for you then I can open it up for questions that you may have for me. 
 15:47: so we do general practices here, some of our own version of Scrum, this at all, are all are a little bit different. 
 15:56: Inevitably, you'll, you'll end up getting a jail ticket, that may not have as much detail as you'd like to complete the ticket, and so when you're dealing with that ambiguity, what steps do you take to resolve, that, those questions that you can perform your work that you need to do? 
 16:15: Of course, like, there's an issue of ambiguity as I, as you like, so like that's actually, you know, pretty common situation first of all. 
 16:25: So especially when you are working on platforms like, platform teams or foundational services where the requirement can evolve as people learn more about the problem. 
 16:34: So when I receive a year ticket that is ambiguous or lacks enough detail. 
 16:39: The first thing I do is to try, you know, understand the business objectives behind the request rather than, you know, focusing immediately on the implementation details, or I want to understand what problem we are trying to solve and who is impacted. 
 16:54: So next, I would like to review any available documentation like related tickets, you know, design documents or like, previous implementations or, or like, or like food that might, you know, provide the additional context for me. 
 17:09: So often like there's information available elsewhere that helps, fill fill in some of the gaps. 
 17:17: So that, that's what I try to assess and if question still remains like proactively reach out to the product owner or the business stakeholders or like architect or the team members who may have like context as well. 
 17:30: So rather than like simply saying, I don't, understand the ticket, so I will try to, you know, come prepared with, with the specific questions or potential approaches. 
 17:40: So for example, I might say, based on my understanding, I, I, I see two possible implementations. 
 17:48: which is, which is, which of these aligns better with the, with the intended outcome. 
 17:52: So that's what, I would, take the approach of fasting. 
 17:56: So, so that's how like they don't, I mean, you know, they, they can, I mean, understand my approach and can provide the better solution rather than like thinking that I don't understand, you know, fully. 
 18:07: So yeah, if, if, if the work is like, particularly complex, then I may should a quick discussion with the, you know, relevant stakeholder to classify. 
 18:17: Assumption before, you know, development begins. 
 18:20: So yeah, that, that's, like once I have, enough information, I like to, you know, document the believed upon, you know, assumptions and the acceptance criteria so, so everyone has a, have understanding moving forward and that helps, I mean, reduce the, you know, misunderstanding later in that development. 
 18:42: Cycle and I would find that ambiguity is often unavoidable sometimes. 
 18:47: So but clear communication or asking thoughtful questions is important and validating like assumptions are usually prevents the bigger issue later. 
 18:58: So yeah, that, that's what I My boss. 
 19:03: Yes, thank, thank you for that detailed explanation. 
 19:08: OK, I, I think that the questions that I have for you. 
 19:12: what questions can I answer for you? 
 19:15: so yeah, I would like to know like, what, problem we are trying to fix, like what feature or what platform, what type of, technology we are building, and what is the role going to be, performing in, in that in that case I would like to ask that. 
 19:34: Yeah, absolutely, as I mentioned, we are a team of 5 engineers who handle the authorization, authentication and coordinate concepts for the platform that is getting their insights. 
 19:47: so we work with several other teams and they have features that they are trying to deploy for this, this application, and we are there to help support them because we're not one of those foundational teams that helps deliver the core concepts that they need to do their jobs and so we We have to eat that complexity for them so that they, they can ask simple questions like is this user allowed to do this and we can provide the solution for them. 
 20:12: that requires integrating with several other stream resources that we don't control, that where the users may come from, where the authorization rules may be defined, and we help, present all that up in a nice package for them to consume. 
 20:26: And we also deliver important concepts to them through eventual consistency. 
 20:32: So we publish streams to sis, and we let them, we represent our data APIs that that we can great, but then we also can consume those streams and to, handle that eventual consistency and own their own stability at that of the journey. 
 20:49: some common things that we're thinking on right now is again expanding some of the stro concepts that we have all the data concepts that we wanna present. 
 20:57: And we also like to, there's a big push now for standardization for our solutions. 
 21:02: So there's a lot of different ways, as you mentioned, to solve authorization. 
 21:06: But right now our current implementation is following standard Reebok patterns and ABC patterns, but, it is an in-house solution and our goal is to minimize that and transition to something more off the shelf because I'd rather spend your guys' time focused on private and problems. 
 21:24: rather than just that other authorization system. 
 21:27: So standardized that likewise I mentioned with the authentication, we do have some customization with the JWT, well, you mentioned you haven't dug into that side a little bit that much yet, it can be kind of complex, so there's a, a Microsoft likes to do things in its own way a lot of the time, so it's a big knowledge, training there, and I wanna minimize that as well so that you can get your standard JWTs on this side, standard authorization on this side, and then we can focus on bigger problems like the erospatial problems with the on the boundaries or, introducing new layer types for better analysis, things like that. 
 22:03: Got it. 
 22:03: Got it. 
 22:04: Thanks a lot for the detailed explanation of that. 
 22:06: I'll just get the overview and high-level implementation and the approach for from you. 
 22:11: So my like my last question is going to be like, what can be the next processes from here, and if any feedback from, for me, like from here if you can get. 
 22:24: Sure, so in the process and we're being a bit aggressive with the hiring process, so you should hear an answer within the next week or two, assist you from there. 
 22:34: I'll work with Ryan to make sure we deliver that, Coca is going through a company split right now, so we do need to have this position filled before, this fall because then at that point they're gonna do certain things. 
 22:45: So we do wanna make sure we're within that time frame. 
 22:48: So we're looking to get it filled this summer in that regard. 
 22:53: and so we we should have answers for you soon. 
 22:55: in terms of feedback, I thought you did a, a fantastic job in interviewing. 
 22:59: I can tell you're very well practiced and your years of experience are really showing, through this process, and I, I appreciate the level of thought that you put into my questions. 
 23:09: I had a series of, different, levels of answer and detailed answer, and I so appreciate that that went into great details and you know. 
 23:18: So, I appreciate the thought. 
 23:23: Thanks, it's, it's, it's really nice talking to you. 
 23:26: Like it's a very back and forth question and answering, and it's, it's, I didn't feel any like it's an interview, so yeah, it's, it's so nice. 
 23:38: I appreciate your time today, and look forward to chatting around in the future. 
 23:43: Thanks a lot. 
 23:44: Have a nice day. 
 23:51: I 
