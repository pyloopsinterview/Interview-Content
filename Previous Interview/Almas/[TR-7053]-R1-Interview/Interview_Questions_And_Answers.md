0:00: Hi, Kylie. 
 0:05: I'm Elizabeth, all of you. 
 0:09: How are you? 
 0:11: hey, good afternoon. 
 0:13: Good afternoon. 
 0:16: Right, when you, I'll turn it over to you. 
 0:17: I'll drop and we'll connect after. 
 0:19: Sounds great. 
 0:20: Thanks. 
 0:21: Thanks. 
 0:24: We might have one more joining us, so I'll probably give it just a couple more seconds if that's OK. 
 0:30: There we go, perfect timing. 
 0:34: OK, well, thank you for joining. 
 0:36: Especially I know it's on the lunch hour, so I apologize for that, but thank you. 
 0:42: I'll do, can I have some quick introductions with the team, and then, let you introduce yourself, of course. 
 0:50: I'll provide an overview of the project and specifically our team and the role, and, then we'll probably dig into asking you some questions, but we'll make sure to save plenty of time for you at the end as well. 
 1:01: Yeah, sounds good. 
 1:03: Awesome. 
 1:04: Well, my name is Whitney Hayes. 
 1:06: I'm the deputy program manager for this project. 
 1:10: I've been at the VA for I think I counted it up the other day as 12 years, and on this project in particular for the past 6, so it's a lot of fun. 
 1:24: I really, really love getting to support the veterans, in any way that we can. 
 1:28: It's great, very filling, and I kind of run around and do a lot of different things, but I act as the deputy for the program. 
 1:40: I'm gonna toss it over to Depeka next. 
 1:44: Hey, I'm Vitika, the release manager supporting, the portfolio application portfolios we have here at, Veteran Affairs, primarily with CRM, which is D365 environment, so I basically manage the overall release planning, scheduling, coordination, some change management, deployment readiness across other environments, a team supports, which is, which is reproduction and production. 
 2:12: Yeah, so, yeah, that's about me. 
 2:14: it hasn't been very long that I've joined Veteran Affairs. 
 2:17: So it's almost 3 months now. 
 2:22: Yeah, so. 
 2:24: Yeah, I would let Kli go next and, and then we can get started. 
 2:29: Sure, thank you, Deepika. 
 2:31: hi, I'm Kali Devinini. 
 2:33: I'm a D365 platform technical architect, so I just joined Lendipika a few months back. 
 2:40: So I'll be doing architecture reviews and providing best practices and thank you. 
 2:47: It's my turn. 
 2:48: So, hey, I'm, I have like 11 years of experience with the Dynamics 365 and Microsoft Technologies and like a, a major part of like like my recent experience has been like focused on release management and deployment engineering. 
 3:03: like in my current project at the Legend Biotech, like, like I manage the end to end release life cycle from the Dynamics 365 and the Power Platform applications and like I use Azure DevOps for like the, source control branching for request and like build and the release pipelines, version management approvals and the CIAD automations and like my responsibility is to make sure. 
 3:28: Like approved changes, like move safely from like development to the QA, UAT and the productions and, like before every release like I evaluate the solutions package dependencies, deployment sequence, and, like apart from that, like, I have also hands on experience with the datawa solutions for automated C plugins, JavaScript like integration solutions, environment specific configurations, and so yeah, like that's pretty much about me. 
 3:59: Awesome. 
 4:00: OK, so I'm gonna give now an overview of kind of the project and What I would consider to be some interesting things about it that you might not have experienced on other projects. 
 4:11: So we are at the VA, of course, we're part of what's called the Digital Transformation Center, DTC. 
 4:18: essentially it's the VA's attempt to Modernize the VA. 
 4:23: Everybody at the VA is still stuck a little bit in the Stone Ages for the most part. 
 4:28: And so VTC is there to help them get either their SASS or pass solutions available to them. 
 4:35: so that's where our team kind of fits in. 
 4:37: We manage the platform for both power platform and dynamics, although this role is specific to dynamics, We act as not only like the platform owners, but also as governance where Hallie comes in quite often, and then also. 
 4:54: We are kind of like the The layer of protection for the VA. 
 5:00: So VA has a zero trust policy, which means that in the upper environments for pre-production and production, they drastically limit who has access to that. 
 5:11: and so that's where our team comes and we own and manage those upper environments. 
 5:15: In the lower environments though, there are development teams from various companies, various contracts. 
 5:23: They do the development. 
 5:24: They own the lower environments, the testing, etc. 
 5:27: etc. 
 5:28: And so they are doing everything and then handing it over to us essentially, and so a lot of times we will be. 
 5:36: Implementing things that we did not make and so it's, it's always a that adds a layer of fun, and so. 
 5:45: Some of these are really old legacy applications as well. 
 5:49: They don't necessarily, none of them, in fact, are using an automated CICD pipeline, something that we're hoping to start working to push them towards, And some of them are even using managed solutions. 
 6:06: So it, it gets very fun. 
 6:09: everyone's a little bit different. 
 6:10: Everyone, every single of the applications has like, you know, their own intricacies that you have to learn. 
 6:17: It's a lot of fun. 
 6:19: but overall it is dynamic CRM, specifically customer relationship, customer service is what I meant to say, sorry, CE, and so. 
 6:33: yes, yes, sorry, no, no, I say like it's definitely makes the like the release process like more challenging, like especially like when you are dealing with the legacy application unmanaged solution and the like manual deployment. 
 6:46: Mhm it's very true. 
 6:49: And so this project in particular, all of these development companies, they kind of inherit what whatever company came last, right? 
 6:58: And so there's been people, you know, lose information, It's not necessarily coherent. 
 7:06: The next person, the next company that comes in to do the development, maybe they're tasked to do something very specific, even though there's a lot of things wrong with the application, it's just, it's just a lot of fun, I think it's the best way to describe it. 
 7:19: There's never a boring moment for sure, the. 
 7:24: Other aspect of this role in particular is that it is specifically for a set of the applications that require after-hour support. 
 7:35: and so they are all basically call centers for veterans and veterans' family members to be able to receive service any time of day. 
 7:46: some of them only have late hours, so maybe until like. 
 7:51: 678 o'clock. 
 7:52: Some of them are 24/7 and so, coordinating with them to do things in the low volume hours is always what, we're gonna be having to do for production releases. 
 8:04: And other than that though, I think that's, I think that's a good summary. 
 8:10: But I'll, I'll stop for now. 
 8:12: feel free to ask us questions as we go along. 
 8:14: That's perfectly fine, but I'm going to hand it over to Depeka to start with some questions and I'll probably pepper some throughout. 
 8:22: Thank you. 
 8:24: Well, Marlene, so you mentioned that you had some development experience in the past on the CRM. 
 8:29: So what, so have you worked as a release engineer in the past, or was it on the development and what you have experience, like I was like in my work, like the like. 
 8:43: I've been like heavily involved in the release life cycle like like I work with Dezure DevOps like for source control like as I told you earlier like the branching the pull request and like the for example like when D365 releases like ready like I review the work items like make sure like the changes are like coming. 
 9:03: To the correct branch, review the PR and validation results, build up like package and the, dynamic solutions and verify the solution was an dependencies and then like, coordinate the deployments like through the QA UAT and the productions and, apart from that I also handle the deployment failures like. 
 9:23: In some cases like like a cured deployment field because like of we can say of like missing solution dependency. 
 9:30: So like I reviewed the Azure DevOps and like the dynamics deployments logs also like identified like the missing components, corrected it in like on development, like increase the solution versions, rebuild the package, and like redeployed it like successfully. 
 9:51: That's through CICD pipelines, I'm assuming. 
 9:56: OK. 
 9:57: How are you with the manual deployments because we don't do any deployments using CICD pipelines here as far as I see. 
 10:04: Mhm. 
 10:04: Like, I, I, I have like also have experience on like the manual, like, basically like my CICD experience is like definitely something like that can bring to the team, but I have like, like, assuming that everything needs to be, needs to be like, automated. 
 10:20: Immediately, like, I 1st, 1st like like the existing deployment processes, governments and requirements and like approval flow solution architects and like also like in my current dynamics application requires like the manual deployment like I can work within that the process giving the solution package and the versionsvaing the dependency. 
 10:41: conforming environments, especially contributions and approvals, importing into the target environment and like the, correct sequence and like then performing post-deployment validation and in fact, like, with legacy application and unmanned solution, I would like to be even more careful about like. 
 11:01: Documenting and like exactly like what was deployed like due to like what changed and then over time like if the team decides to introduce automations like my major major DevOps experience can help with that transitions and also but I I've like also done the like manual or all of the stuff. 
 11:25: So our engineers here are involved in reviewing the deployment instructions, executing the deployment instructions we received from the development teams itself, based on what they have gone through on QuA and the death implementations, so. 
 11:42: Yeah, so our job is to execute, review the deployment instructions, make sure we have everything, with respect to access, and you have to go through the instructions that, make sure that we have everything required for our release so we don't get interrupted during the release. 
 12:00: executing the releases, of course, based on the instructions, troubleshooting the deployment issues when required, and of course, secrets and certificates is another aspect which we also support here. 
 12:14: So, so like Whitney already said, we support both planned releases and of course the unplanned ones which we get often like hot fixes and emergency changes. 
 12:27: So troubleshooting ability, ownership, communication, and, and, you know, being, Able to work under pressure are very important for this role. 
 12:36: Yeah, yeah, like talking to or like firstly during the deployment, like, like I follow the, like the approved instructions, but if like something fails like I'm comfortable like troubleshooting like it rather than like. 
 12:50: Simply like stopping at the error like I review like the deployment logs, dynamics, and the database errors, solution dependencies, plug-in trays, and like also like for the secrets and certificates, like I understand those are like sensitive operational, components and like generally my approach is like to first, verify like that the required secrets or like the certificates exist and it's like valid and not expired. 
 13:16: I like that the application or integration has like the correct access and like have like we can say configurations and generally I would always, always like follow the organization's approved security and change management processes like rather than exposing credentials or like making undocumented changes. 
 13:36: In your current or previous organization, how did you guys track, the sequence and certificates which are coming to and expiry? 
 13:46: not so, we, we don't want, to check whether the secrets are, up to the date before the release, anytime before the release. 
 13:58: How, how, how did you guys, Do this way ahead of the time, I mean, independent to the releases, generally we track deployment sequencing as like part of release document, documentations and the Azure develops work items. 
 14:12: Like for each release we document which component needs to be deployed first, for example, like, database solutions components, like the plug-ins and the configuration changes, power automa flow. 
 14:25: I'm asking about the secrets and search, right? 
 14:29: How did you guys track. 
 14:32: Mhm. 
 14:33: Which ones are coming for expiry? 
 14:34: How did you keep track of the secrets and certificates which are coming to expire? 
 14:38: like, basically, like in my previous, like we treated expiration as a part of like the pre-release readiness check. 
 14:47: Like we would review the relevant secrets and the services before the release and verify the, expiration. 
 14:53: dates make sure like nothing critical was like approaching inspirations and like for the items we are like responsible for like we maintain the required information of coordinating with the appropriate teams and like totally when when something needed renewal during the release preparations like I would especially. 
 15:13: Especially check that the credentials or we can say required like or certificates required by the applications and integrations are like still valid and apart from that like I should mention that like I will not claim like we had like this specific automated expiration monitoring tool and in my previous project unless like. 
 15:35: it was a part of that environment. 
 15:37: My approach is like to make, make it a part of the release readiness checklist and like operations, tracking and like if a VA team has like a, a specific tool or like a process of tracking installation, I'm like completely comfortable following that process. 
 15:54: OK, have you ever used, any specific tool for certain secret management, for security purposes? 
 16:02: Mhm, yeah, basically, like I worked with the, like, like management and the enterprise applications and the deployment support, but, like I want to be transparent that generally, like I've used a dedicated secret management product extensively enough like to claim deep expertise like the Azure key vault. 
 16:22: Like my experiences, like me being around making sure the dates and certificates like required by the, applications are available, valid properly, configured and not exposed like during the deployment process. 
 16:36: OK, thank you. 
 16:39: Can you tell me the most complex production release you personally handled, and also explain me what made it difficult and how did you get through the release? 
 16:50: I remember like, one of the, like the most challenging was basically. 
 16:55: Like I've handled was that Lesion Biotech. 
 16:59: Like it involved the multiple, dynamics 365 and the, power platform components like going into the same tree like, database customization, C plugins, JavaScript, Per automate flows and the configuration changes. 
 17:13: So like. 
 17:14: Here, like I was responsible for like coordinating the release from, like as I told you earlier, like deployment to the QA UAT and the final productions. 
 17:23: So before deployment, like I validate the solutions versions dependencies, deployment sequence environment specific configurations and the approval so. 
 17:33: like the biggest challenge happening during the Qo development is like the solution import failed because of like the missing dependencies, and I renewed the Azure DevOps and the dynamics deployment information identified like the missing components and It's traced it like back to the source solutions and like instead of manually fixing QA or the bypassing the process like like I work like basically work with the deployment side to correct correct the like dependencies incremented the solution version, rebuild the package and deployed it. 
 18:09: And once like the QA passed, we promoted the same validated package to the UAT, completed the business validations and approvals, and then like scheduled the production deployments and before production I did another readiness check including the deployment sequences, configurations, dependencies, and the rollback, the contradiction and. 
 18:33: after that, the production deployment completed successfully, and we performed the post deployment validations and, like monitored the environment, like afterward. 
 18:43: Did you guys use any tool to check the dependencies or, like, generally at the at the legend at the flows work flows, yeah, is there a tool which you used to check the dependency way before or like we primarily use the D365 deployment information and logs along with, like the Azure Devops deployment history like where the applicable. 
 19:08: And like for dependencies related issues, like I would check like the basically the dynamic solution informations and like identify which components were like missing, causing, and I, I like use plug-in trace locks and the power like automatron history so it dependent, it depends on like where the problem is. 
 19:31: OK So tell me if pre deployment is successful, does it automatically mean you're comfortable proceeding with the production? 
 19:48: like, generally. 
 19:51: When it's happened, like, basically, like it's not automatically like a successful production deployment is like a strong indicator, but for me, like it's not the only go, no growth, no grow like criterion. 
 20:06: Like before production, I would like still confirm that we are like deploying the exact same validated package and the version. 
 20:15: That like QA and UAT testing has passed and like required approvals are like complete and the production is specific items like such as the configuration values of security access integrations or dependencies and like we can say security access integrations dependencies, you know like secrets or certificates and like deployment like sequence have like been verified and apart from that, like I will also reviewed the rollback plan and any like non issue like from pre fraud and Environment difference are like important because something can deploy successfully in UAT and still fail in the production because of like the configuration access or like the integration difference. 
 21:02: So generally, like my approach is like, successful prero give, gives like the confidence, but production readiness requires a separate final go or like the no go check. 
 21:16: I, I, I just have a question on the certificates, Mhm. 
 21:22: So after rotating a secret, right, the application, say suppose the application stops authenticating, how would you troubleshoot? 
 21:31: generally in these types of, scenario, like, what I do, like, firstly, if an application stops authenticate, authenticating immediately like, like after a secret of the certificate, rotation, like I would first confirm that the timing is like actually related to the rotation and Understand the impact. 
 21:53: Then like I'd walk through, it's like a systematic like first I like verify that the new certificates or secret is valid, but not expired or Correctly installed like but you just, you, you just rotated a new secret. 
 22:07: You just added a new secret. 
 22:10: And you restarted the app. 
 22:12: OK, like, when like I added the new secrets, like I have like just basically I checked the application for like integration logs to confirm that exact authentication error. 
 22:25: Then I verify that the new secrets were like created correctly, that is active, has not expired, and then the value application is like, actually using and I'd also check whether the application is like still referencing the old secret or whether like. 
 22:40: there's like there's some, configurations or like the permission issues and with the like new one and like if the application requires a restart or the configuration refresh or like pick up like new secret, I like verify that as well and like if new secret itself look correct like I. 
 22:59: Check the associated accounts permissions and points and like the environment specific configuration to make sure like nothing has changed and like if the production authentic authentication is down, then like we have an Approved rollback procedure like I use that to restore service like while continuing the root cause investigation. 
 23:23: So like I would not immediately assume the secret is like bad like I'd compare what changed, what the application is consuming and what the laws like are telling me and that like then narrow it down from there. 
 23:42: Oh, I like Carli Gomez. 
 23:45: OK, thanks. 
 23:47: Thank you, Rebecca. 
 23:47: Hi Melin. 
 23:51: let's assume there's a secret key in power automate flow. 
 23:57: While you're deploying, you'll see a secret key in the power automate flow. 
 24:01: So what do you do? 
 24:02: What are the next steps? 
 24:05: generally for this type of situation, like my, like, like I would identify the weird secret is being used and whether it is like. 
 24:15: Actually required by the flow, then like I would check the organization's like approved, like approach like form. 
 24:23: Handling the sensitive configurations and ideally like the secret should be like stored in the approved secure like mechanism or like a configuration approach and then like the flow should like reference that value rather than like hard coding it. 
 24:40: And like for deployment like I would make sure like the seated value itself is like not committed into the solutions, source control or like the deployment documentation and I would like also coordinate with the development or the security team like to replace the hardwooded value with the approved configurations like before promoting it and like if the secret has already been exposed like I would treat it like a Potentially comprise and follow the organization's security processes like, which could include the rotating and revoking the secret and updating the flow like with the new value. 
 25:22: So like generally my priority would be Protect the secret. 
 25:27: Don't propagate it through the deployment and move the configurations to the approved, like secure mechanism and like rotate it like if it has been exposed. 
 25:40: OK. 
 25:43: OK, and have you done any data imports? 
 25:46: Like what are the tools that you used for data inputs? 
 25:51: generally data importing tools, mhm, yeah, like generally for the, like the data import like for power automated like. 
 25:58: I use the flow run history like to check the field runs or like for dynamics 365 and data like I, I use the solution information dependency information and deployment and the import details and for like plugging like the plug-in related issues I use the plug-in trace lock. 
 26:21: And for release tracking depending on the environment like I, I also work with the Azure DevOps like for the source control and the deployment history but I understand like like your like environment may be handling deployments manually and so like like. 
 26:42: like, I would choose the tool based on the issues like power auto meter and history for flows, dynamics, database information for solutions and dependencies, and plug-in trace locks for like the lugging errors. 
 27:00: Hello. 
 27:01: yeah, OK, it's better now. 
 27:05: we did not hear any of your answer. 
 27:07: I'm so sorry. 
 27:08: basically, the second you started answering, it cut out. 
 27:12: Oh, I think there was some network issue. 
 27:15: Can I tell you again? 
 27:17: Yeah, yeah, sure, yeah, like, basically the tool is like removed for troubleshooting and, like deployment and power automate child like, like, like I mainly work with the, DH when the power platform tools themselves. 
 27:31: So like for power automate like I tell you, like I use the flow and history to check the, like the field runs and, like the inputs and outputs and like the identify like the. 
 27:43: Where the flow is breaking and for 365 and data like I use solution information dependency information and the deployment info like import details and for plug-in issue I use the plug-in trace log and also like I would choose the tool like based on the issue, like power automated history for flows, dynamic data was information like for solutions and dependencies and like plug-in trace locks for like the plugin errors. 
 28:10: OK, what about for the data inputs, if you want to import bulk data, can you please come again? 
 28:17: Bulk data. 
 28:17: If you want to import the bulk data, how do you import them? 
 28:21: OK, like, generally for data imports, like, bulk, like for data work, like I would first like understand the volume and the relationship between the records like for like, straightforward bulk import, like I would prepare the data like in a supported format like such as CSV and use the D365 data import capabilities and I'll also make sure the required fields, data types, look up values and relationships are like correct before like starting the import and for like a larger migration I would use an appropriate bulk data integration of migration approach, like especially when we have like the multiple related entities and needed to control the order loading and, after the import like I would, validate the report report counts, field reports, look up relationships and, apart from that, I will also review the, like the import errors and the addresses then like rather than assuming the bulk load was successfully just because the job completed. 
 29:28: OK, OK, what, what, what is the difference between managed and unmanaged solutions? 
 29:35: Oh, OK, like, basically. 
 29:37: Like an unmanaged solution is like typically used in the like the deployment environment like and and they like developers can add or we can say modify components directly and those components remain editable and we use unmanaged like solutions while building and maintaining customizations and like on the other side like a managed solution is generally used for QA UAT and the production like it's a package for deployment and the components like like. 
0:00: Solution then make that the release process like more consistent. 
 0:05: OK, so let's assume we are doing, we are using only unmanaged solutions in all the environments. 
 0:10: OK, so if the, if the client asks or if the, if the team asks to do the changes, customization directly in production, so what do you do? 
 0:23: basically. 
 0:26: Well, then Yeah, because Sunman is solution, right? 
 0:29: They can direct, we can edit in the production. 
 0:32: So what do you do? 
 0:33: So like, I would first they ask, they just ask to change some small field or update a field, required field or some small update. 
 0:42: So what do you do? 
 0:43: So because it's an. 
 0:45: Yeah, like I would first understand why the change needs to be made directly in the production. 
 0:50: And whether like it is an approved like emergency or like the hot fix and like even if we are like using unmanned solution across environments like I would not make an ad hoc production change like without following the organization's change management and the approval processes and if it's like the normal change, like I would prefer to make the change in development and like. 
 1:16: Validate it through the QA or UAT and then like move like approved change like into the production and it's a general production emergency so like I would follow the emergency change processes, get the required approval documents exactly like what is being changed and make the smallest possible change and afterward like I will make sure the same changes like properly captured back in the development environment so we don't create like environmental. 
 1:47: OK. 
 1:49: how do you manage versions, conversion control in different environments? 
 1:54: like, generally for the different environment, like I make sure, like, for example, like before I release, basically I use the source control like where the pro project has like your works in place, and, like, like before I release I make sure the solution has like the correct major, minor, build, and like the, like the revision versions and like that the versions. 
 2:17: clearly I I identifies the disease we are like deploying and when changes are like made, I update the solution versions before creating the deployment package. 
 2:26: So like in a major des environment, like I also track the corresponding commits, branches, PR, and build the releases so like we can trace exactly like the changes like went into the like the particular release and also like for the manual deployment environment like I would still like maintain the solution versions and Like, release documentations carefully that the way like, if there is like issue in production we can identify like exactly which versions was deployed and what changed and like which previous versions or like packages was like approved. 
 3:03: OK. 
 3:05: so can you give me one, example where the, where you had a challenging issue, production issue. 
 3:14: Like challenging issue, like just one example. 
 3:18: any project. 
 3:21: one challenging production related issue like I handle was like around the D 365 deployment where like, like the multiple components like being released together like including the C plugins, data was components for automate tools and the like the configuration changes. 
 3:39: So the like the challenging part was after deployment we had issue that. 
 3:45: Initially, like, it was not obvious whether it was like related to the code, configurations and like solution dependencies, so like I started by Understanding the business impact and then check the dynamic deployment information, solutions dependencies, plugging trace logs, and then the power on histories and depending on like the company involved. 
 4:11: You know, like, a related release, like we actually found that the missing solution dependency was like causing the, deployment failure. 
 4:19: So I traced the error back to the source solutions, identify like the missing components and like instead of making a manual workaround in like a target environment like I corrected the dependencies in the, development, increased the solution versions, release the package and move it like through the validation, process again. 
 4:42: OK, so let's assume there is a plug-in issue. 
 4:45: So let's assume there is something related to the plug-in. 
 4:48: You required only the plug-in code and something related to the plug-in. 
 4:51: So how do you troubleshoot the plug-in issue? 
 4:54: like, generally for the plug-in issues, like, basically, I would first, reproduce or identify the exact operation like where the plug-in is failing and understand the business first. 
 5:07: Then like I had to start with the lugging tree slots. 
 5:09: Like I had to look at the exception message, state trees, lugging step, entity message, and like the like the execution context so they understand like exactly where the failure is happening and like after that like I had totermined where, where it's the actual code issue or something around environment, for example. 
 5:30: like, I would check like the plugin, registrations, execution, execution stage, filtering attributes, or like the configuration values or any dependencies. 
 5:40: So the plugin is like, using and like if the plugin is calling dataverse or like another integration, I would like first verify like whether the like related record permissions or like the external services available and Once like I, I identify the root cause, I would work with the, with the development team or like the correct the code or like the configuration, and I make sure like the fix is tested in development and the QA first and then like move it to the approved release process rather than like the directly changing the production. 
 6:19: OK, thank you. 
 6:23: yeah, with me, I'm good. 
 6:24: I'm done. 
 6:25: Thank you, thank you, Marie. 
 6:27: Thank you, and they covered a lot of the questions that I probably would ask. 
 6:31: So let me try and see if what might be last. 
 6:35: thank you guys. 
 6:36: I appreciate all, all the questions and your answers only right? 
 6:40: with you the One of the questions that I do have is, Part of us being governance is also providing recommendations. 
 6:51: And so if you are reviewing an upcoming deployment and you see. 
 6:58: Something that doesn't quite make sense. 
 7:01: Would you feel comfortable bringing that up either to Topeka or maybe even the architects to bring back to the development team, Generally, for this, like, absolutely, like I would be comfortable, bringing that up and I think that's like an important part of the government and the lease rule. 
 7:22: And yeah, like if I'm reviewing the deployment and something does not look right, like, like, like for example, like a missing dependencies and the deployment steps, so I will not just proceed because it's already in the deployment instruction. 
 7:34: So I would like first. 
 7:36: Validate like what I am seeing and understand the potential impact, then like I bring it up like all the team or like the architects, yeah. 
 7:48: Perfect. 
 7:49: And kind of along the same lines, I think this is something that we've run into. 
 7:53: Can you kind of, from your perspective, when would be the best Use this case for using a an app registration versus like a service principal. 
 8:05: like the best use cases, like an app registration is like essential, like where we define the actually identifying its authentication configuration, like the service principal is like the identifier of that application is like a specific tenant and like that what the typically grant permissions to, for example. 
 8:24: like, if, if we have the details justify for the power platform integrations that needs to authenticate to the another system like without using a personal account. 
 8:33: So like I have used an application identifier like identifier and the like the corresponding service principle with like only the permissions that like integrations actually need. 
 8:45: So this gives like the non-interactive identify identity that is not tied to then the individual like employee. 
 8:57: OK. 
 8:58: And then this last question, I promise it will be last and we'll save time for you. 
 9:03: It's more of just I like to ask this question to anybody I interview for any role, which is how do you, you have a list of things that you have to get done in a day, how do you self-organize? 
 9:15: I just like to see how people's brains work. 
 9:17: -huh, generally for that, like, Basically I usually organize my day based on priority, priority like, or the business and impact and the deadlines rather than just like working through a list from like top to the bottom, like for example, like if I have a production deployment schedule or like a deployment issue and some like regular development task, so I will like first prioritize the production activity and anything that Could impact the release first and also like look ahead to the upcoming deployments and make sure the prerequisites like the access, approvals, dependencies, configurations, certificates, or like the other required items are like ready before the release window. 
 10:05: Awesome. 
 10:06: Thank you. 
 10:07: I don't think I have any other questions. 
 10:10: I will open the open the floor to you. 
 10:14: Do you have questions? 
 10:15: It can be about the role, the project, the team, whatever you'd like. 
 10:19: Oh yeah, like, like, basically. 
 10:23: First, like, I like to understand what the, like the day to day responsibilities is like would you like for this role, like would it like would the primary focus on reviewing the, like the executing deployments, troubleshooting the release, or like, or anything else. 
 10:39: No, great question. 
 10:41: so I'll probably let Topeka answer this a little bit more in detail, but at a high level we do have a tier 2 and tier 3 team that does a lot of the troubleshooting piece of it. 
 10:50: However, we would coordinate with them if there was an issue. 
 10:53: So if they needed to make a configuration change or if there was an. 
 10:58: Expired secret that didn't get caught, you'd be the hands on the keyboard, to do the fix essentially, and so you'd be helping with the troubleshooting, but you wouldn't necessarily be the responsible one if that makes sense. 
 11:13: I would say the majority of the team's days are filled with reviewing and preparing for any upcoming deployments and then. 
 11:22: Like Topeka mentioned earlier, because we are dealing with a lot of legacy applications, that are kind of Frankenstein together, there ends up being fairly regularly something pop up and so we try to keep our team's capacity lowered in the expectation that some of our time is gonna be taken up with helping and supporting something that was not planned for. 
 11:45: So I would say it's about fifty-fifty of planned work and unplanned work, Hopefully that will start decreasing the more infrastructure and the more guidance that we provide, but yeah, Tapika, do you wanna add anything to that? 
 12:01: I think you answered everything with me. 
 12:04: our daily duties are mostly on like witness of planning and planned releases, but our main goal is to for the planned releases we have to be proactive. 
 12:14: And see if we have the change tickets created for the change process, right? 
 12:18: We have to make sure the change tickets are created ahead of the time we receive all the approvals, whether all the documentation that is required is attached to the tickets, basically take ownership of the complete release from the change to implementing that until the smoke testing which we do, the post implementation and then hand it over back to the development team or the business to do the rest of the testing, so. 
 12:43: Having the ownership of, of from beginning to end, which includes the change process, which includes the release readiness. 
 12:51: Yeah, it's fine. 
 12:52: Like basically that type of work like I do in my like, in my current organization it's like I'm comfortable with that. 
 13:04: Yeah. 
 13:08: Any other questions for us? 
 13:09: like, any other, like another, round for this room, apart from this? 
 13:18: No, I don't think so. 
 13:19: typically how it happens ishobit from continuum, he, I don't know what the interview process is before us, to be honest, but it's. 
 13:29: Once it gets to us, this is the final round. 
 13:31: And so, thank you for, you know, speaking with us. 
 13:35: I know it's, it's fun to go through multiple, multiple rounds of interviews, I'm sure, so what we do is we provide our notes to showbiz and then showbit will reach out with next steps. 
 13:45: Yeah. 
 13:47: Thank you, thank you to all. 
 13:50: You're welcome. 
 13:51: Thanks. 
 13:52: Thank you for your time. 
 13:52: Thank you for your time. 
 13:56: Bye. 
