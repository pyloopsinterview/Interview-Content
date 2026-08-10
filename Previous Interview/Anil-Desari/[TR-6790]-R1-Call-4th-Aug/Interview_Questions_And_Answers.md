0:00: Open until you guys opened it. 
 0:02: Cool, I'll let you go. 
 0:03: Thank you. 
 0:04: Thank you very much. 
 0:06: Hey Neil, how are you doing today? 
 0:09: Hey, Joe. 
 0:09: Hi, I'm doing good. 
 0:11: Yeah, thanks for asking. 
 0:11: What about you? 
 0:14: not too bad. 
 0:16: just, you know, normal Buffalo's rainy summer day. 
 0:25: so, before, before we get started with this, you wanna tell us a little bit about yourself? 
 0:31: OK. 
 0:32: So, like, yeah, my name is Enigma Deari, and like I have around 12 years of experience in software development and like primarily working with the Python, P API and Azure cloud technologies and throughout my career, like I've been working through like across healthcare service and financial services and insurance, retail, and etc. 
 0:55: So like currently I'm working as a lead Python developer at 11's Health on an enterprise healthcare analytics and provider management platform and like the goal of this project is to like modernize legacy healthcare applications and like one of the major initiatives which I worked on was like integrating our applications with the like Ping Federate and Ping Directory like to. 
 1:20: Implement SSO using OA or 2 and Open ID Connect and SAML. 
 1:26: So and like I'm also actively involved in production support and like whenever issue arises I analyze logs, identify the root cause, and coordinate, coordinate with the infrastructure or security teams if needed and yeah like that's a very brief intro. 
 1:47: OK, cool, So, did you see what the job description was? 
 1:55: basically we're looking for a couple of things. 
 1:59: the primary role, is to take some of these applications that we have, the ones that are gonna make it through to pass next year and get them co-located between our local data center and our cloud. 
 2:13: have you worked on this type of project before? 
 2:15: Do you? 
 2:16: Understand the, the pieces that are required to be able to co-locate the software and have it be kind of transparent to the customers. 
 2:24: Yeah, I do understand and like, yeah, I worked with all of this. 
 2:29: I'm familiar with these things and like, like my current role at 11 Health, like one of our major initiatives was also in like modernizing the legacy healthcare applications and which was like available across both on premises infrastructure and the Azure cloud and like from the application perspective like the work involve like several informa important pieces and Another important part is like identity and access management and like since users were accessing application across like different environments, so like we also integrated there like with the Pink factor and the Ping directory to like provide a consistent single SSO and so yeah. 
 3:13: I'm familiar with all of that stuff, yeah. 
 3:16: OK. 
 3:16: What, what do you consider the biggest risks when extending our authentication platform into Azure? 
 3:23: OK, so like the biggest risk, I would consider for, the situation would be like, like maintaining a consistent and, secure authentication experience like across, both on-premise and as your environment would be like, like during a hybrid m migration, let's consider so like users shouldn't like. 
 3:44: Have to authenticate differently depending on like where an application is hosted and like if the identity in the integration isn't like designed properly, it can like lead to login failures or token validation issues or inconsistent user access so like. 
 4:06: Another important risk would be like is to like protecting the authentication tokens and our sensitive credentials and like when applications move to Azure and it's critical to like ensure tokens are transmitted securely. 
 4:21: So like, you, you need to have the like correct expiration policies and, and aren't exposed in logs or our application code. 
 4:30: So yeah, like I also think high availability is very important. 
 4:34: And yeah, finally, I believe that testing is a major part of like reducing the risk and before rolling changes into production, yeah. 
 4:43: OK, cool. 
 4:47: How, how much, so how much automation have you done around these platforms, more specifically things like certificate management, and that type of work because that's part of what we're looking for as well. 
 5:02: Hm. 
 5:03: So yeah, like I have done quite a bit of automation in my current role and like, especially talking about the application, deployment or the infrastructure operations. 
 5:12: So like, the main goal like was to like reduce the man. 
 5:16: Will work and like improve consistency. 
 5:18: So for example, I would consider like I developed the Python PowerShell and Bash crips to like automate the application deployments across environments and like instead of manually performing deployment steps every time. 
 5:31: So yeah, like I also. 
 5:34: This made our release like much more consistent and significantly like reduced the deployment time and I also worked on like automating the server configuration and like the certificate management so yeah like we had a repetitive operation tasks that were like prone to human human error so we automated them to ensure every environment followed the same. 
 5:56: Configuration standards and another area like I am remembering was like an operational monitoring so I created the the automation to like perform the health checks and collect the application status after the deployment so that potential issue like could be identified early so and since our application also use like a pink red so. 
 6:18: Automation also ensured like help ensured deployment consistencies and whenever the authentication related configurations or certifications are updated. 
 6:28: So yeah, overall the automation I built using pattern like reduce the manual effort and yeah. 
 6:35: That, What, what kind of, how deep is your open shift container type experience? 
 6:44: OK, so for this, considering open shift, container type experience, like, I haven't like, in this, my container platform experience like has primarily with the docker and the joy Cer needs and, oh, good, so you have Kuber Daddy's experience, just not specifically open ship, OK. 
 7:06: OK, I mean how deep is that experience? 
 7:08: Are you? 
 7:10: Platform maintenance type of work getting deep into the back end or is it just with the working with the containers themselves, you know, deploying and so like primarily it was like on the application side rather than on the like the platform administration and like like not primarily responsible for like maintaining the Cuban needs and all like my work was involved in like kind of. 
 7:38: Containerizing Python applications with Docker and deploying them to OpenShift and configuring like so yeah I like I would say I have like solid hands on experience on deploying and supporting the on OpenShift and but not deep experience with cluster. 
 7:59: have you done any deployments with Prey for co-location? 
 8:05: Yeah, I do. 
 8:07: OK, and, and how have you experienced any issues around replication between the on-prem and off-prem? 
 8:18: databases. 
 8:20: OK, so like talking about my experience with Pink Director has been like from the application integration side and my, in my current role at 11 Health as I mentioned, our application integrate with the Pink Federate on the like to provide the SSO and all and for deployments, I was like responsible for the application side deployment into our like Azure environments and Including the automating deployment using Python and PowerShell and Batch and validation, the, the authentication flow after the deployment and working with the like IM teams to verify everything function correctly. 
 9:00: So, regarding the ping directory co location deployment like I have did like but not directly deployed or administered the ping directory platforms across multiple environments, but my experience is like integrating the applications with it and validating the secure authentication after deployment or troubleshooting authentication issues, so yeah. 
 9:24: Ouch. 
 9:27: have you, done any work with pass keys? 
 9:31: Yeah, I did. 
 9:33: You've, you've done rollouts of Patsky and the TOTP type authenticators. 
 9:39: Hm. 
 9:40: Google Authenticator that kind of stuff. 
 9:42: Yeah, I worked with the gas and like from the application integration perspective, my, like gas was part of our enterprise authentication ecosystem. 
 9:53: And where the focus was on like the ensuring the applications could securely authenticate and communicate with the organization identity platform and my involvement was primarily around integrating our fast API applications and with the authentication infrastructure and valid validating authentication flows and troubleshooting login and access issues. 
 10:18: So like. 
 10:19: From our fast API microservices, we like verified the rest API and validated the Pink Federate SSO authentication flow and checked the connectivity like with the dependent services and monitored the application logs after deployment. 
 10:37: So like if any issue were identified, we investigated the root cause, fixed the problem, and revalidated before completing the rollout. 
 10:47: Thank you. 
 10:49: All right, yeah, if you don't mind, I'm gonna ask you a few questions here. 
 10:53: just one thing I'm kind of interested in and looking back on your migration experience, what was, what would you say was one of the biggest lessons you've learned from a project that didn't go as planned? 
 11:05: One of your biggest lessons learned, right? 
 11:07: Yeah, yeah. 
 11:08: So like talking about one of my biggest lessons everything goes perfect. 
 11:13: So, the biggest lessons I would talk, Bob is like I learned is that, successful migration is much more about like planning and coordination, than just moving the application to the cloud. 
 11:25: So yeah, like, in one of our modernization projects at 110, we migrated the legacy application to fast API microservice running on Azure Cubic service. 
 11:35: From a technical perspective, like, building the services wasn't the hardest part, but the bigger. 
 11:41: Challenge was making sure the authentication and the API integrations and dependent system continued to work seamlessly. 
 11:48: So yeah, so the experience taught me the importance of like validating every dependency early and involving the infrastructure or the security teams from the beginning and. 
 12:00: Having a detailed rollout and rollback plan. 
 12:03: So, the biggest takeaway for me was that the cloud migration isn't just a technology project, it's a collaboration effort. 
 12:13: So when the application and the infrastructure security business teams stay aligned throughout the migration, the deployment is much more smoother and production issues are significantly reduced. 
 12:25: So yeah. 
 12:30: Yeah, and you did mention, you know, like documenting flows and things like that, I guess like, before migrating a critical application to a colo, how would you identify all the different application dependencies, you know, just some of them. 
 12:44: OK, OK, OK. 
 12:45: So like the sum of the dependencies I would list down would be, before migrating a critical application is the first thing I would like to understand how the application works in production. 
 12:56: And I would review the existing architecture and application documents or the deployment configurations and environment settings to identify everything and the application depends on. 
 13:09: So then I would work with the business infrastructure and database and security teams to map out all the integrations, and that includes the databases, external APIs, authentication. 
 13:22: Services like Ping Fed rate and file systems. 
 13:25: So like if any and or any network connectivity, like I would like also review application logs and configuration files because they often reveal dependencies that are undocumented. 
 13:37: So yeah, like we followed a similar approach like when modernizing our legacy applications into the fast API microservices on AGR. 
 13:45: So yeah, I found yeah. 
 13:50: Yeah, for sure. 
 13:52: All right, now I'm going to go through a weird scenario here. 
 13:54: All right, so let's say it's migration weekend. 
 13:58: The application server is up in the colo, but users cannot access the application. 
 14:04: just kind of walk me through some things that you would look to troubleshoot, like what would your process be for that. 
 14:10: OK, so for this, my process to troubleshoot would be, like this is a classic production for troubleshooting. 
 14:19: so, the first thing I would do is, avoid making assumptions and follow a structured troubleshooting approach and first, like I would, confirm the scope of the issue and, I would check whether the, like, application is unavailable for all users or only a specific group. 
 14:40: And then the like that helps determine if it's a system-wide issue or something related to the like authentication, networking or user access. 
 14:50: So like next I would like to verify that the application itself is running correctly. 
 14:55: I would like check whether the application ports or the services are healthy and. 
 15:02: Review the application logs. 
 15:03: So like the, if the application is healthy, I would start checking the dependencies. 
 15:07: I would, verify database connectivity, connectivity to downstream APIs, and after that, like I would also look out for the infrastructure infrastructure side with the infrastructure team to like I would verify the DNS solution, load balancer, configuration, and firewall rules. 
 15:27: So like, and confirm that the. 
 15:30: certificates and environment specific configurations were deployed correctly. 
 15:35: So yeah, throughout the process I would compare the new environments with previous production environment and the most important thing during a migration weekend is to restore services safely and communicate clearly with all the teams involved while working throughout the root cost. 
 15:53: All right, cool, thanks. 
 15:55: So let me ask you, do you have any questions for us about the company, about the job, about. 
 16:02: OK, OK. 
 16:03: So like one of my question would be like what are the like major roles and responsibilities like I would be dealing for this role, particular role, sir. 
 16:13: But for this particular role, the first priority is to get us into our co located data center. 
 16:21: So we have a couple of applications that we know for sure are gonna have to be migrated, a few that we're not so sure if they'll have to be or not because we're trying to get off of them. 
 16:31: We've recently started, we've recently rolled mostly to a new identity provider that is fully cloud located, so, you know, a lot of the stuff that we have that's on prem we're slowly trying to work away from. 
 16:44: to avoid having to do this is part of the reason, beyond that, we're looking to do things like, move to more current MFA methods, so we're, you know, looking to switch from. 
 16:59: Like a ping ID type authenticator or the old hard token type authenticators to more current methods like Google Authenticator pass key, that kind of stuff, and then the next thing beyond that is automation of our current services, things like being able to. 
 17:20: React to new tickets in ServiceNow with API calls to create things like a new OIDC client for a new application and stuff like that. 
 17:32: OK, yeah. 
 17:33: OK, that makes sense. 
 17:35: Like I have worked with, in the similar hybrid environment, yeah, sounds good. 
 17:44: And so just a little bit about us that I probably should have stated at the beginning, MMT is a fairly large banking organization. 
 17:52: We're modernizing all of our authentication platforms, so we're, you know, currently going through numerous projects to move all of our customer authentications to a single platform, move out into the cloud as much as feasible, That that kind of stuff we're trying to, you know, kind of lessen the dependency on our local data centers and be more resilient. 
 18:21: OK, sounds, sounds good. 
 18:22: That sounds interesting. 
 18:26: All right. 
 18:27: Have any, any other questions, bud? 
 18:29: like, what would be like the further steps or rounds after this, like, particular. 
 18:38: Yeah, that's so, so the, the next, after, after we get everything into the cloud that has to go into the cloud, the next steps are to start working on MFA migrations. 
 18:47: We have a couple of applications that are using very old MFA methods, so we want to get them modernized. 
 18:56: And then after that then we'd start working on automation. 
 18:58: So we're we're looking at probably up to a one year engagement. 
 19:03: OK sounds good. 
 19:03: , like, one more question, like I was having like for the like interview process, like what would be like the further rounds and like interviews that would be conducted, yeah. 
 19:18: There, there may not even be further rounds, most likely, I, I'm gonna interview, we're we're gonna interview a handful of people, and, you know, try to, try to pick the best, two because we have two positions open, So I appreciate the time that you've given us and we will definitely one way or the other get back with you. 
 19:40: We have, you know, interviews scheduled all this week, and I'll go through all of them and then pick the ones that, seem to fit best. 
 19:47: But so, so far from the answers you've given, and you seem to have. 
 19:52: The right, the right answers to the right questions, so you're, you're certainly on the list of, of a consideration. 
 19:59: OK, thanks for the feedback and like I understand it. 
 20:03: Yeah. 
 20:04: Yes, absolutely. 
 20:05: But, I don't have anything else. 
 20:07: I don't know if there's anything else. 
 20:10: No, I'm all set. 
 20:11: Thank you for your time. 
 20:12: OK, we appreciate your time and we will let you know one way or the other, probably by the end of the week. 
 20:18: OK, or next week. 
 20:19: OK, sounds good. 
 20:20: Nice meeting you. 
 20:22: Yeah, OK, thanks. 
 20:23: OK, thanks. 
 20:24: Bye bye. 
