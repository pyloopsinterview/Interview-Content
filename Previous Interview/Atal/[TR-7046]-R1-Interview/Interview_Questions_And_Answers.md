0:01: We'll make sure to give you a chance to introduce yourself, And ask, ask some questions, so we wanna make sure that we definitely save time for you to ask questions as well. 
 0:12: So please feel free to pepper them in or save them for the end, whatever you wanna do. 
 0:16: but yeah, I will. 
 0:18: I have a quick introduction for myself and background, and then I'll probably hand it over to Topeka and Kelly to do the same. 
 0:27: Then I'll give an overview of the project at the goal. 
 0:30: so I've been with the VA for about 12 years now, and working in a lot of different areas within the VA, sometimes on the government side, sometimes on the government side, sometimes not even to do with, software at all. 
 0:48: So it's been a lot of fun. 
 0:50: I've been on this project in particular for the past. 
 0:54: 6.5 years basically since it started and again not always on the dynamics team. 
 1:00: I used to run the power platform team before they combined and then before that I've done a lot of, a lot of other random things. 
 1:10: so I'll, I'll pass it over to Depeka. 
 1:12: Depeka is our release manager, so I wanna make sure that you get a chance to talk with him. 
 1:18: Hey, this is. 
 1:18: Hey, hi. 
 1:21: OK. 
 1:22: Yeah, so Whitney already introduced me. 
 1:24: This is Deepika. 
 1:25: I'm the release manager supporting the applications of all the application portfolios that VA. 
 1:33: I manage planning, scheduling, coordination, the deployment readiness across environments. 
 1:42: so our team, I mean, it's been over just over 2 months I've joined VA. 
 1:49: So, I'm still learning under Whitney's guidance now. 
 1:53: Yeah. 
 1:57: Nice to meet you. 
 1:57: OK. 
 1:59: Nice to meet you, Jodie. 
 2:01: Thank you for that. 
 2:04: Kelly, you're up next. 
 2:05: Yeah, hi, Adam, this is, Carli Devminini, and I'm a dynamic and Perla technical architect. 
 2:14: So I've been working in CRM for a few years, from 8 years, 78 years. 
 2:19: So I just joined 2.5 months ago. 
 2:22: So I do architecture reviews and provide solutions and all that. 
 2:26: Nice, nice meeting you. 
 2:27: Nice to meet you. 
 2:29: OK, so let's just do this is my time. 
 2:31: So yeah. 
 2:32: Hi, my name is Attal, and I have around like 11 years experience working on a Microsoft Dynamic CRM. 
 2:38: I also work on D65 and Power platforms. 
 2:41: I'm more strong focused on the, D65 customer engagement, data work, Power Automate, Azure, tation. 
 2:49: And, and enterprise application deliveries and over the, over the year, I have worked across like both like deploy deployment side and release and release engineering side, but in, you know, in my recent project, I am major part of my responsibility has been like dynamics of ALM, ALM deployment, and I manage solution across deployment, test, UATs, production environment, including like solution packaging, dependency validation, version management. 
 3:16: Yes, these are a couple of responsibilities. 
 3:18: I've handled most recently I am working with the like Williams Williamsson Kingston Health as a lead dynamic CRM and power automate platform solution developer and yeah, it's a healthcare environment, so I have released governance and control deployment and yeah like especially are important. 
 3:36: I work on closely with the developers and functional side as well, integration teams and architectural decisions as well. 
 3:43: I have contributed as a part of the team as well. 
 3:46: I have also, you know. 
 3:48: I have, I have also experienced in the troubleshooting solution, imports, failures, plug-in issues, data wars, yeah, a couple of areas which I have, major experience. 
 3:57: Yeah, that's pretty much about me. 
 4:01: Awesome, thank you. 
 4:02: I appreciate that. 
 4:03: Good coverage and you hit on a lot of points that we'll definitely cover today. 
 4:06: That's great. 
 4:09: so I'll give you just kind of an overview of what the project is and how our team kind of fits into it. 
 4:15: So DPC is called Digital Transformation Center. 
 4:18: It's basically the VA's attempt at modernizing DA. 
 4:22: Everything at VA is very old. 
 4:24: It is ancient, and BPC is there to try and help people either get like the. 
 4:30: Commercial off the shelf products that they need or a platform, low code no code version to meet their needs. 
 4:40: And so we are on the platform side of things, of course, and we manage the power platform and dynamics. 
 4:46: Tenant for the entirety of the VA, but we are on the governance side of things more than anything else. 
 4:53: And so what happens is that there are Third-party development teams that are hired by the VA to do the actual work, to make enhancements, to maintain and Make sure that everything is up and running and they. 
 5:14: Own what would be the lower environment. 
 5:16: So any dev test and anything along those lines, they have their full control to be able to deploy, do their testing, move from one environment to the other. 
 5:25: But when they get to production and production, then it changes over to the other arm ownership. 
 5:32: And so the VA has a zero trust policy, which means that they strictly. 
 5:39: Enforce who has access to our environment. 
 5:42: Only the people who absolutely have to have access. 
 5:46: And so, That is where our team comes in basically. 
 5:50: They are working in the lower environments, but once it's time to move to pre-product production, they hand the package to us. 
 5:56: They hand us the digger. 
 5:56: They hand or the design. 
 5:58: They hand us the finite instructions. 
 6:01: And any of the documentation around that. 
 6:03: And they Basically, are hands off at that point. 
 6:08: They do join the deployment calls, and a lot of times they'll point out things or they'll realize that maybe they documented something incorrectly, but it's on our responsibility for them forward. 
 6:20: As part of that, we also, have to do all the environment management, so secrets and searchs, that's a big one, making sure they're always up to date and correctly rotated and correctly stored thoroughly. 
 6:34: Going through and doing any environment. 
 6:39: Updates, so. 
 6:41: DLPs, Trying to think, my mind's just gonna go on blank for a second. 
 6:50: But there's a lot of it that kind of just falls within our purview. 
 6:56: The main thing that's a little weird, I would say is that you mentioned Azure and several of the applications that we support have Azure as their infrastructure in the back end. 
 7:07: We don't actually touch so. 
 7:11: It's a weird line, and I always want to bring it up to people because it always kind of throws people, but we are not actually allowed to touch the Azure side of things. 
 7:20: There is a different contract again because VA likes to separate things as much as possible to maintain security. 
 7:27: so there's a separate group of people that maintain Azure. 
 7:30: They have to do their piece. 
 7:31: We have to do our piece. 
 7:32: So there's a lot of collaboration, It can get a little bit tricky, especially the development teams don't always understand that. 
 7:40: So they think you're gonna be doing something, but really it's either on them or somebody else. 
 7:45: So it can be a little fun. 
 7:46: Yeah, yeah. 
 7:47: I feel like I've been rambling a bit. 
 7:49: I will probably Go on mute and let Depeka and Kelly ask a few questions. 
 7:56: they're probably gonna be the more technical questions. 
 7:58: I'll fully admit, I'm management space and not as technical as they are, which is why I wanted to join with you today. 
 8:06: but yeah, ask questions as we go along if you want, and we'll happily answer them. 
 8:11: And thanks for giving me insight and it's, it's obviously like when you're working on the government project. 
 8:17: They are in a couple of restrictions and but yeah it's surprising to know like they are not using Azure because you know mostly these projects are like mostly built on the Azure sites so yeah but yeah they're good to know. 
 8:29: So they are, they are using Azure we just don't, yeah, for this particular, yeah, I understand. 
 8:35: Yeah, it's weird, yeah. 
 8:39: OK. 
 8:40: Yes. 
 8:41: Thanks, Whitney. 
 8:44: I would let, I would let Carli ask more technical on CRM questions, but I would go through a few, on the release end. 
 8:54: So, So what do you verify after a successful pre-pro deployment or a pre-production deployment before allowing the safe release to proceed to production? 
 9:05: OK. 
 9:06: So, yeah, like if, you know, after successfully, like people or department is like, I may focus on the confirming that the department is not just a tech technically successful, but, but, you know, that, that the environment is actually ready for the validation or production. 
 9:23: I first I verify the solution version and that and make sure you know expected managed solution and components are import imported successfully or not. 
 9:33: Then I check for any missing dependency solution layerings issues, import wiring could be in a potentially cause problem later so I focus on that. 
 9:43: Next, I evaluate the environment specific contribution, especially, you know, connection difference, environment, and environment variables, security rules, indication end points. 
 9:53: I also make sure that components like Power automatefus, plug-ins, and any, any dependent indication are enabled or configured as per expected. 
 10:03: And from, from the functional side, I coordinate with the testing team to run the, run the keys smoke test, business critical scenarios. 
 10:12: If they are, if they are, if they have plug-ins or indication involved, I will, I will also, I will give you the plug-ins, trace logs or an applications, application level site. 
 10:23: But yeah, this is how, you know, I, I go validate the after deployment and, and run the successful runs. 
 10:31: You're talking about the pre-road validation right now because my question is about how would you assure that it's already for the production before I get into the production. 
 10:43: You, yeah, you, you did, bring up a few points I understand, but is there a tool in the past which you have used to, do a dependency check. 
 10:53: How, how, how do you do this dependency checks? 
 10:55: Yeah, I was looking like evaluation after preport deployment, and the main thing I verify like same package we intend to move the production correctly and deploy, deployed, and it's in a dependency environment specific, and yeah, I would typically check solution version, manage solution, as well as like as I can say as I earlier said, these are the major thing I have, reviewed and yeah, And I like, once, once everything is validated, I make sure, department valuation release notes signed approvals, evidence are documented. 
 11:29: So yeah, these are a couple of things I, review. 
 11:35: OK, I'm not sure. 
 11:35: I'm, yeah, I give him correct answer in order, but, it's for you ask question, but yeah. 
 11:41: Yeah, but she is, so say you're deploying the production and the deployment, phase halfway through, what would your, what would be your immediate steps? 
 11:53: OK. 
 11:55: Yeah, so I would like, I, I would, you know, I would capture the deployment or solution ports logs and, identify which component field. 
 12:05: In the, in the dynamics, I would check whether it's dependency issues, solution learning problem, version mismatch, data was dependencies. 
 12:14: I would also determine whether the failure actually, actually left any component part of like partially imports or a change in the production environment, and that's important before, you know, taking any corrective action. 
 12:27: And if the deployment is a part of a To approve changes, I would follow the document rollback or recovery, procedures rather than, you know, making any, HOCA changes and the production. 
 12:39: And I would also coordinate with the deployment team and, and functional team, you know, if their failures required code solution correction or not. 
 12:47: And once the root cause is identified and correct, I know, and corrected, I would validate the package again. 
 12:54: And you know, preferably in a lower environment or people or then, you know, follow the appropriate changes control process before ending the production again. 
 13:03: And the key, basically key key for me is to protect production first, understand the failure, then recover in the controlled and peaceful way rather rather than you know simply running, reading in the deployment and potentially making the situation worse. 
 13:18: So this is, this is my approach going to be. 
 13:22: And you would also understand the impact of it, communicate with respective team members, and then depending on the impact, determine whether it's, it's whether the fix is can be available soon or could be rolled back. 
 13:38: Yeah, definitely, definitely. 
 13:41: So I know if I can say the standard for me and, and I would not treat impact assessment as a part of fast response as well and before, you know, deciding whether the, whether to continue or fix forward or roll back, and I would understand what was the already, already, you know, changed in the production and whether the business functional or indication are effective and yep, that's, that's how, you know, I will handle this kind of scenario. 
 14:08: Constitutions. 
 14:11: OK. 
 14:13: Have you worked with the application secrets or secret quotations or certificate renewals? 
 14:20: Yeah, yeah, in the past, yeah, I have worked with application secrets, as a part of, you know, managing dynamics, 365 and power, environment, particularly where the integration and a role-based service are involved, and typically I will like dealt with the things like client secrets, AI. 
 14:38: Cents and certificate connection information and that application need to be communicated securely. 
 14:44: My approach, you know, my goal is to make sure those values are, are, never hard coded or stored directly into the solution files or source, store sorted like because they, because they should be managed through the appropriate secure configuration mechanism and with the access restricted based on the environment. 
 15:03: And, and the pipeline lease privilege and for the deployment, I will also, you know, verify that the requirement, secrets or certificate is available or correctly configured in the target environment or not because because our solution can import, import successfully, but the integration can still be the credentials or the certificate are missing or expired. 
 15:27: So yeah this is I know this is how I handle the this kind of, you know, outside of just and this is I can say these are you know team directly managing the infractures that outside of our responsibility but I am comfortable with working with the them and make sure any requirements are securityly available and without any any any kind of in the way. 
 15:50: I do have a question for that if that's OK. 
 15:54: what kind of tools have you used for securely tracking and maintaining secrets and searchts in the past? 
 16:00: Yeah, for dynamics like power, like there, you know, previous, like primarily I worked with environment variables connection difference to keep, you know, key environment specific configuration separate or Azure Azure indication project, I have worked with Azure key vault for security. 
 16:15: Managing secu secret certificate or keys and application sites for troubleshooting when, when, when, when the integration failed after the configuration credential change. 
 16:25: And from the, from, from like, from the release side, I have worked with the your DevOps pipeline for passing configuration securely between the deployment staging without exposing the sensitive values or in a pipeline or the source control. 
 16:38: So these are a couple of tools which I have used. 
 16:41: Perfect. 
 16:42: We use that to keep size was curious. 
 16:43: Thank you. 
 16:48: So, OK, so you explained what would you, what you would do on the secret citation and so it's. 
 16:54: So how would you prevent, prevent from discovering an expiring secret during a production release? 
 17:00: I know you said how would you would work on it in advance. 
 17:05: But what if you discover during a production release there's a secret or a or a certificate for expiry? 
 17:11: Yeah, actually this will be the, major, major issues if we are, you know, exposed the secrets in the production side. 
 17:19: But yeah, this kind of a situation, I faced earlier when I worked with juniors, some of the juniors, but yeah, first I like maintain, inventory of the secrets and Like cert certificates like used by each application and environment including the expiration date and ownership. 
 17:40: Then I would set up the monitoring and alerts with the like enough lead lead time then typically 1316, or 19 days depending on the organization policies or, and for a job-based components, Azure key vault and, and it's like it's monitoring capabilities can help identify the become the expiration. 
 17:57: And on the, on the power platform side, I would also verify the related connection difference, application registries, integration, configuration during the release validation, and yeah, for, for like for the, for the roti rotation, I would follow the control process where the new secret certi certificate is. 
 18:15: provi, provised before the existing, existing one expired. 
 18:20: So yeah, I would make sure, you know, make sure, ownership and escalation path are clearly documented so that, that way if, if alert kind of comes in, we know that exactly what teams need to be at. 
 18:33: So yeah, this is how I'm going to handle. 
 18:38: Mhm. 
 18:40: How did you have, yeah, OK, thank you, April. 
 18:44: Thank you. 
 18:45: So, what, what are the managed and unmanaged solutions like how do you explain? 
 18:52: What are the advantages and yeah, the main difference between like, like unmanaged solution is typically used in the, in the development and developer can directly modify components like tables, column plug-in, and other customization. 
 19:06: That change, changes become a part of development environment. 
 19:10: So if, if it gives the, if it gives the, development team flexibility while doing that, while building that building and testing and manage solution is like. 
 19:20: Can see what I would normally use for downstream environment like UAT and production. 
 19:26: It's like treated more like a deployable package and component are controlled through the solution life cycle rather than, you know, being, directly modified in those environments. 
 19:37: And in my, in my project we generally follow the pattern of unmanaged in the development and manage for the downstream environment and before, you know, promoting, promoting a you know managed solution. 
 19:48: And yeah, that's a major difference. 
 19:52: OK, can I answer that with another question, Kelly? 
 19:55: I'm sorry. 
 19:58: I want to bring up something that I think is another interesting point that What we are dealing with here at the VA, which is a lot of these dynamics apps are legacy apps, and they are all Inherited from one development team to the next. 
 20:12: Usually a development team is only around for maybe a year or two, and then a new team comes in and a lot gets lost in translation. 
 20:21: the new team is inheriting whatever the last team did. 
 20:24: It's not, it's not ideal, and so a lot of our deployments. 
 20:30: I wanna, I wanna say maybe Topeka, would it be about fifty-fifty, do you think that are not using managed solutions in the African environment either. 
 20:38: so I just wanted to make that clear so you're aware, but also ask about your experience with doing manual deployments and deployments with, Maybe less than ideal situation. 
 20:52: Right. 
 20:53: And, yeah, kind of situation and Like, is it, is you wanted to explain, like, yeah, so yeah, oh yes, so like, I worked with like legacy demo and then with them I mean where you know where solution structure wasn't, always clean. 
 21:18: And where ownership, changed, like between deployment teams, dey teams. 
 21:23: So in those situations, I did not, do not, you know, assume like that's that expect like existing environment follow the ideal ALM model. 
 21:33: My, like, like I would like usually use. 
 21:36: Like, you know, understand that, what we are actually inherit and what solutions are installed, whether they are managed or unmanaged, and what, what, you know, what the publisher are and who are the components are you know layered and what dependency exists between solution. 
 21:55: And if the environment is using unmanaged solution, I would, I would very, would, you know, very careful about the trying to change immediately, especially in the, in the production, and unmanaged unmanaged layer can be contained more like important customization that, you know, other, another team or application dependent on it. 
 22:14: So removing or replacing without, you know, understanding that dependency. 
 22:18: change would create a bigger problem which we are currently, which if we are currently dealing with any kind of problem. 
 22:24: So it's, much bigger than that. 
 22:25: And for me, the, the, practical, I can say approach is stabilize first, document what exists, identify like ownership or dependency, then, you know, gradually, I can say improve the ALN model where, where possible. 
 22:42: And yeah, I am, to work on this kind of environment previously. 
 22:46: So I have seen a situation where the documentation doesn't completely match what actually you don't deployed. 
 22:51: So rely on the environment, so I, I know, I have, I have history previously on this kind of situation. 
 23:01: Thank you, I appreciate it and thank you for letting me into it now. 
 23:04: Sorry, yeah, no problem. 
 23:06: Yeah, so, but, have you like, developed a pipeline, CSCD pipeline, or a power alternate pipeline? 
 23:14: Yeah, actually, not directly. 
 23:17: I have, you know, I am, I am more on the maintenance side, but, OK, yeah, so, but I, I have no, I have experience in the CICD side. 
 23:24: I have involved with the CIA like, DevOps team, and, the, you know, building entire CNCD framework from. 
 23:31: Scale, I'm not, I'm not gonna complete anything because I've not done that. 
 23:35: But, when, but when, but when I, you know, I work closely with the pipelines and and and like deployment forces including, value in the solution package, manage, you know, versioning, checking dependency. 
 23:48: I have also involved with these released steps around like A or DevOps where the pipeline handle activities such as like building packaging, solution, running the validation, generating the deployment of artifacts, and promoting the, promoting the same version to the environment based on the approval. 
 24:06: So yeah, this is the experience I have in the KGB side. 
 24:10: OK, got it. 
 24:12: And have you used any XRM tools for the deployment? 
 24:16: Yeah, I have like any other, yeah, yes, on the release and maintenance side, I have worked with several tools depending on what needed to be troubleshoot or automate from dynamics and power platform. 
 24:28: I have used the solution checkers, plug-in, plug-in trace logs. 
0:00: I have also involved with these released steps around like A or DevOps where the pipeline handle activities such as like building packaging, solution, running the validation, generating the deployment of artifacts, and promoting the promoting the same version to the environment based on the approval. 
 0:18: So yeah, this is the experience I have in the KDB side. 
 0:22: OK, got it. 
 0:23: And have you used any XRM tools for the deployment? 
 0:27: Yeah, I have like any other, yeah, yes, on the release and maintenance side, I have worked with several tools depending on what needed to be troubleshoot or automate from dynamics and power platform. 
 0:39: I have used the solution checkers, plug-in, plug-in trace logs, power platform, admin center, database tools to validate. 
 0:47: Solution or troubleshooting deployment are running or runtime issues from CSCD release posts. 
 0:53: I have worked as a DevOps for like with the out of teams and for a source control pipeline. 
 1:00: So yeah, these are a couple of tools I have, I have experience and work on. 
 1:06: OK, and, let's assume there are, there are around 200 power ultimate flows, and you want to activate or update the connection. 
 1:14: So how do you do that in the bulk? 
 1:16: There are around 200 power ultimate flows and you need to turn on all. 
 1:20: So how do you like actually do that if there are bulk, so many power ultimate flows? 
 1:24: Yeah, so lift, lift around like, you said like 200, right, so. 
 1:29: I would not, I would not manually open and activate them one by one. 
 1:34: I would treat as a bulk administrator, administration and deploy deployment task. 
 1:40: First, I would identify the flows and confirm like that they are belong to the same solution or application and make sure, you know, make sure their connection references are correctly configured in the target environment. 
 1:55: And for the, for the actual bulk operation, I would use Power Peed from CLI and PowerShell automation, depending on the, depending on what access and tooling the environment is allowed. 
 2:08: I would retrieve the list of to validate their current state connection and before, before, you know, enabling all 200, I would, I would also, you know, test the process with the smaller groups first, maybe, you know, maybe a few, representative tools to make sure connection difference credentials work correctly or not. 
 2:28: Yeah, this is, how, you know, handle this kind of scenarios. 
 2:31: Yeah, that's a great question. 
 2:36: OK, so, if, let's assume there are some solutions. 
 2:41: One is a managed and one is managed solution. 
 2:44: And when we are deploying to different environment, how do you deploy? 
 2:50: Like, how do you manage the versions? 
 2:53: Version control, yeah, in different environments. 
 2:55: OK, so for version control, yeah, I have worked on that and, like as per my experience, the main, you know, main, like for like for one managed solution I would, you know, generally keep that, that in, in dep deployment and The, and sorry, development and, and, and development where the team is like actively making changes. 
 3:20: Once the changes are ready for promotion, I would I would package the release with the appropriate version number and move, move the validate artifacts forward for manage solution. 
 3:32: I, I, I would, I would use the same version package through the test UAD and production rather than, you know, rebuilding it separately from each environment, and that's basically give us traceability and make sure we are promoting the exact artifact that was tested. 
 3:47: For example, we might, we might have versions such like, suppose 1.4 in the test. 
 3:54: So valuate it there and promote the same version to UUT, then promote the same version into the production. 
 4:01: And after approval, if the another another release we are increment, we like increment the version such as like 1.5, so I, I also make sure version is reflected in the release note changes request or documentation. 
 4:17: So yeah, the main principle is one control, one controlled traceable version moving, moving, moving, you know, moving through the environment rather than creating a slightly different version for each environment. 
 4:30: Yeah, this is my approach going to be. 
 4:34: OK, so like if, if the, if you're deploying the same version, right, we'll have the same changes. 
 4:39: So if you want to, if you want to deploy the solution with more changes, so what do you do with the mission? 
 4:47: OK, if like, if you're adding more components to the solution and we want to deploy that to a different environment, so what do you like, how do you actually manage the version? 
 4:59: Like if I need to deploy solution, with the additional changes, I would 1st, 1st, 1st make sure those changes in the, development environment. 
 5:09: Updated the solution version. 
 5:11: I would not directly modify the managed solution in a UAT or production, and then I, I would make sure that, sure, you know, all. 
 5:19: All, all the new components or modification are included in the solution. 
 5:24: Check, like, check for any, any new dependency after that, I would, you know, I, I would export, export the update solution from the, typically as a managed solution and from the time like for, for downstream environment. 
 5:38: Before production, I would deploy the same update version through the normal path. 
 5:42: And such as like test DD and one important thing like I would, I would also check solution laying and update behavior if it is an update to the existing manage solution I would need to understand whether if we are simpl and like updating the existing. 
 5:59: Component or whether like whether components are being added or removed if components need to be removed, I would consider the appropriate, manage solution and I would consider the appropriate like, sorry, I upgrade the spreadsheet rather than just doing the standard import. 
 6:16: And once the UT is validated and approval are completed, I promote that exact list version to the production. 
 6:23: Yeah, this is, you know, this is, this is the process which I have followed, during this kind of scenarios. 
 6:31: OK, sure, thank you. 
 6:33: one more, question about the data imports. 
 6:36: Have you done the data imports? 
 6:37: Like if you have done, like, what is the process you have done? 
 6:40: Yeah, I have worked with data imports like in the dynamics and dataverse as well. 
 6:44: I have handled the input, import as a part of migration and application changes. 
 6:49: All, all my primary focus has been on release and LM side. 
 6:55: My approach depend on the like volume complex. 
 6:57: of the data for a smaller smaller and controlled data set, we, we like, I can say we can use the tools such as like data versus import capabilities, Excels and CSB imports, power, power platform tools for larger and more complex migration. 
 7:13: I would, typically work with the, government and data migration team using like using prop like appropriate migration tool. 
 7:21: and evaluating the result. 
 7:22: I'm not remembering the exact two, but yeah, I have worked with them, and the important part for me is dependency order. 
 7:30: For example, if we are importing accounts or contacts or keys or records, I make sure the parent records are required, reference data, data are available before importing the dependent records, and I will, I would, you know, I will also verify. 
 7:46: The required fields, lookups, alternate keys, ownership, or data type. 
 7:50: So after, after the import, I, I validate the, the record counts and key business scenarios. 
 7:58: Check for the failure or rejected records or any review indication or plug-ins error that may have occurred. 
 8:06: So, yeah, this is, you know, this is I have experienced in in the daytime import side. 
 8:12: OK, and also what was the like most challenging release you faced you know in the projects, like most challenging, and how did you like fix it? 
 8:23: Yeah, actually, every, every release is challenging, and, but yeah, one of the more challenging release I would work like on was in like in this in current current company, like Will, Wills Kingston and. 
 8:38: The environment where you know where we had dynamics to require solution with the like multiple database company and power power automate flows, plug-ins and the indication. 
 8:49: So the challenging part wasn't just simply simply importing the solution. 
 8:54: We had dependency and the virginal environment issue where some components in the target environment were not matching what the release package expected. 
 9:04: And there was, you know, also environment specific configuration that that had to be validated separately. 
 9:10: Instead of, you know, repeat like repeatedly retrying the deploy deployment, I passed, you know, I reviewed the solution. 
 9:19: Imports, logs and dependency information to identify exactly which component causing the problem and I, I worked with the like deployment team and with them like compare the environment and determine what needs to be corrected. 
 9:36: And once, once, once the issue was addressed, we validate, validate this solution again in the lower environment. 
 9:43: As I said earlier, this is, this is the annual steps we have followed during the during the deployment and, in the production side. 
 9:50: So yeah, this is, this is the main challenging work I have done and what made me, what made the release. 
 9:56: Challenging was number of moving part, but it's also like reinforced something I follow closely when, when release fails, understand the root cause was communicate an impact, then you'll recovered through the controlled process rather than making quick changes directly in the production. 
 10:14: So yeah, this is how I resolve, but yeah, this is the most challenging work work I've done. 
 10:21: In the department, yeah. 
 10:23: Yeah, there are multiple components, right? 
 10:25: It's not easy to, like, if the solution is large with more multiple components. 
 10:30: So if there is any plug-in deployments, right, and if there is an issue with the plug-in, like how do you, fix such kind of issue if there is a plug-in deployment? 
 10:39: OK, so if, if, if actually like when, when release includes the plug-ins, I treat plug-ins fed separately because solution input can, can succeed while the plug-in still fails at the run time. 
 10:52: Right. 
 10:52: And first, I would like identify exactly when plugins is failing and capture the plug-in's trace log detail, especially like, especially, you know, exception message, plug-in steps, except execution stages, and right, so, that, then I, that I would know determine whether the issue is actually in the plug-ins code or whether it's caused by something around it. 
 11:19: Like, such as in recover schema changes, missing dependency, this kind of, you know, small, kind of issue which is, which is causing the plug-ins failure, and, if the plug-ins was working in the UAT but failed after the production deployment, I would compare the environment complication because, because this is the most common cause, cause of this kind of situation. 
 11:42: Where we field and and I compared those environment configuration solution layer before as you assuming the code itself was wrong. 
 11:49: And if it is a code issue, I would verify, I would work with the developers to correct the plug-inst building the version and assembly and deploy the correct solution. 
 11:58: So yeah, this is how we handle the plug-ins when our releases include the plug-ins. 
 12:06: OK, so, during the deployment, right, like what is your rollback strategy? 
 12:10: Like, what is the first step or what do you do during the deployments? 
 12:14: Mhm. 
 12:14: Yeah, my rollback strategy. 
 12:17: start before, you know, deployment itself. 
 12:20: I make sure the changes request clearly define the rollback or recovery plans. 
 12:27: The current production version is known, like, like we have the required deployment artifacts and validate the evidence. 
 12:36: If, if some, sometimes something like something failed during the deployment, I first assess the assess the impact and determine whether the environment is still stable. 
 12:46: I do not, you know, I do not immediately, start making the manual changes and retire early. 
 12:52: This is the first step I would say. 
 12:55: For example, like dynamics like, manage solution deployment. 
 12:59: I, I'm careful with the word pullback and because they simply install, manage solution can be have consequences and especially, you know, if the components or dependency have changes, depending on like what fields, fails and safer option may have the correct issues. 
 13:20: So yeah, this is, this is how I, how I handle this kind of scenario. 
 13:29: Yeah, I think with me and, and then. 
 13:32: I just have one last question about the process. 
 13:37: So, I think, we have a scheduled, production release, OK, and you're already aware that, the solution has passed all the QA or pre-road, all the PVDs are successful. 
 13:47: We have successful results from all environments. 
 13:50: so during the production import, solution import, you realize that the, the import failed because of the dependency errors. 
 14:00: OK, so the, the development team says, oh wait, quickly, let, let us modify something and hand it over to you, another package or something, like, a quick solution so you could, apply it immediately during the release call because of course development team doesn't want to go through the whole, the whole process again and schedule for a new time and you know, they could sneak in such changes. 
 14:20: So how as a release engineer what you would do when you run into the scenarios? 
 14:24: Yeah, actually, yeah, this is. 
 14:27: May like, first thing like we have seen like the the government did not want to know. 
 14:33: going into that, like the last changes, right? 
 14:36: And I would not, not, I would not accept the new package and immediately, deploy in the production just because, just because, you know, we are already on the release call. 
 14:46: Even if the changes look smaller, it, it is, has, it has not gone through the same queue and pre-production validation as the original approved package. 
 14:55: And I would, you know, I would document the dependency here and confirm exactly what's missing and mis misaligned. 
 15:03: Then I would communicate with the development team, you know and release the stakeholders and package we are approved for the production is not, not deployable as is, and if, if development team provide the modified package, I would treat that as a new build. 
 15:19: Changes and not as a quick patch for the existing release. 
 15:25: I would ask them to follow the required release, required process and update the solution version, document the changes. 
 15:32: Yeah, this is, this kind of lengthy process for the the development, but yeah. 
 15:37: If, if, if we are working on the production, definitely I would, I would ask them to follow this kind of, you know, steps, and yeah, if the organization has approval emergency or expected changes process, I would use that rather than, you know, bypassing the governance depending on the severity and business impact, this kind of, you know, depending on the on the impact. 
 16:02: That's for the production, so we push back. 
 16:05: How would you react if it's, if it happens in pre-broad? 
 16:08: It's not production. 
 16:10: You don't need to change ticket in this, so, you know. 
 16:12: So how would you react to my first reaction would to be stay calm and, and you know, clearly communicate with the situation, and, I, I would, I would explain. 
 16:24: that, that the approval package failed because of dependency issue and the, the, the replacement package has not gone through the required validation. 
 16:32: So I can, I cannot treat as a same approval release and at the, at the same time, I would work with the development team and understand how to Quickly they can correct dependency whether they, we have to approved like all emergency changes courses available. 
 16:50: If, if the processs allow the fix to validate, you know, and approved within the release window we can have like evaluate that option and if it's not that, I would recommend rescheduling the production deployment rather than taking, you know, adaptic package into the production. 
 17:09: Yeah, sometimes it happens. 
 17:12: OK, yeah. 
 17:16: I think. 
 17:20: I I have like one or two more questions, but I promise to keep them short cause I wanna make sure that we leave plenty of time for you. 
 17:29: so could you walk me through when you would use an app registration versus like a service people? 
 17:39: I would, if I have to differentiate like, I think app registries as a user is application, registry site. 
 17:49: And the service principle is identity that the application automation actually uses to authenticate to resources. 
 17:57: For example, if I'm setting up, setting up the application that needs to be accessed a database or another productive service, I would register the application in the Microsoft En ID. 
 18:09: And then I use the service, service principal identity to automate, I can say, I would like like automate, like that's that is like especially useful for the ICD pattern indignation and automate and deployment because we, we don't want to depending on the individual user account. 
 18:31: The important thing for me the s like separating the application identity from the human identity, if the process is running automatically. 
 18:39: I like, I prefer a service principal with only the permission it actually needed rather than using someone's personal credentials, and I, I would, I, I would make sure like, like make sure credentials and cert certificate are stored securely and preferably like through the something like keyboards as I said earlier, and the, they have, you know, appropriate. 
 19:01: The expiration and rotation process. 
 19:04: So, so, like, practically I would use application registries to, to define application identity and, like, yeah, and so configuration files, you know, service principle, represent the application identity in the tenant and if, if, if what get assigned permission use for authentication. 
 19:25: Oh yeah. 
 19:26: Perfect. 
 19:26: Thank you. 
 19:28: you actually answered my other question when you were talking, so that works out perfectly. 
 19:32: I will hand it over to you at all. 
 19:34: Do you have questions for us? 
 19:36: How our team is set up, what kind of projects we work on, anything that you could possibly think that we're happy to. 
 19:42: Yeah, definitely. 
 19:43: We, like, previously, did a lot of things, but I would understand that day to day responsibility of the release engineering tools look like to you. 
 19:52: And since, since your team owns the peapod and production environment, how much of their role focus on the actual, deployment and troubleshooting versa governance or environment managed solution. 
 20:05: And coordinating with the development team. 
 20:08: So just I want to know what are the day to day people left us. 
 20:10: It's a great question. 
 20:12: I would say that the majority of The release engineer's time is working on. 
 20:22: Appointments that are scheduled. 
 20:24: Or deployments that are not scheduled, a lot of these applications, like I said, they are. 
 20:32: They're not, not in an ideal state and so they have very often great fixes going on. 
 20:38: in fact, we're in a high priority incident right now, and, it's a lot of fun. 
 20:44: And so a lot of it is not necessarily the troubleshooting itself, although the release engineers do support that a little bit. 
 20:51: We do have like a tier 2 and a tier 3 that take the brunt of that might be supporting them and doing the hands-on the keyboard in terms of like doing the fixes, But the majority of it, I would say is A Reviewing the documentation that's coming your way for upcoming releases. 
 21:11: Coordinating with the development team to answer any of your questions or get clarification ahead of time. 
 21:18: Verifying that you have the correct accesses and being prepared and then actually performing. 
 21:23: we do have a two-release engineer role. 
 21:26: So sometimes you might be the primary, sometimes you might be the secondary. 
 21:30: and so even if you are the secondary though, you have to be just as prepared and ready to step over if you have to. 
 21:37: The VA, their network, the laptops they give us, they're not necessarily the best either. 
 21:42: And so you never know when someone's gonna like get kicked off randomly, you might have to take over. 
 21:47: So, we jump in a lot to support the ongoing issues whenever they pop up. 
 21:55: so I would say it's fifty-fifty between planned and unplanned work, but it's never boring, I'll tell you that. 
 22:03: Yeah, I think, is there anything that I missed? 
 22:06: I guess I cleared all everything you recovered everything with you. 
 22:14: Yeah, I understand. 
 22:14: Like, yeah, you have to, you might have to coordinate with the development teams, so, you know, to get the right information what you're looking for the change to get. 
 22:23: It could be the deployment installation guidelines, you know, back, roll, rollback plans. 
 22:29: We have to just assure that we have everything right before we move on to production. 
 22:33: So yes, you have to coordinate with development teams. 
 22:36: You have to assure that, we're not, crossing our boundaries either as what it is engineers, Yeah, yeah, yeah, actually it sounds very like aligned with the kind of release I have doing in the past and I like, I like like not, not like tool is not only about the executing the deployment but also being prepared before you deployment. 
 23:01: And yeah, this kind of situation we face during the deployment process and we all, all we all that you, we all, principles and deployment and diplomas that we have. 
 23:14: Most of our releases are planned. 
 23:16: Yeah, most of our releases are planned, but if we will run into some unplanned releases depending on the fixes and emergencies we run into. 
 23:24: So we have to be all ready for those as well. 
 23:29: Good. 
 23:30: OK, and one last question, one last question I have, like, what are the like next step from here? 
 23:37: Is there any other known around? 
 23:40: So, that would be a question for showbit because we're a different company. 
 23:44: So, I'm sorry, I don't know what his company's processes are, but we have, we do have one other interview scheduled this week. 
 23:52: so we'll be passing our notes along to showbit, and then he'll be doing my steps. 
 23:56: So I, I apologize that I don't know. 
 23:58: Oh, no, no problem. 
 23:58: No, that's all I have for now. 
 24:02: And that will be in supporting the offer will release release ass as good right as well yeah definitely you're up for the offer, yeah, definitely, because, most of the release process is, you know, work on the, after and after at the different hours, yeah, right, and, yeah, definitely I also, you know, I, I have confidence with the both scheduled release and unplanned release that I like, yeah, yeah, yeah, exactly. 
 24:32: Yeah. 
 24:33: Sounds good. 
 24:33: Thank you. 
 24:35: Thank you. 
 24:36: OK. 
 24:36: Well, if you have any other questions, you can either hand them through showbi or I think you probably have our email addresses in this invite, so feel free to ask. 
 24:46: yeah, thank you so much for your time at all. 
 24:48: It's been a great, great conversation. 
 24:49: Thank you. 
 24:51: Thank, thanks guys. 
 24:53: Thank you. 
 24:53: Thank you for your time. 
 24:53: Have a good one. 
 24:55: Bye. 
 24:55: Thank you. 
