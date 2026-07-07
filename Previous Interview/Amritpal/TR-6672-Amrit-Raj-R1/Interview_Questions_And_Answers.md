0:01: Hi, how are you? 
 0:02: Hey, good afternoon. 
 0:08: Oh, there you are. 
 0:09: I want to make sure we saw you. 
 0:13: And I love that background again. 
 0:16: I've got to get more creative with mine. 
 0:21: Well guys, I just wanted to be here to make sure that everybody, connected without difficulty. 
 0:28: I'll drop off and let you guys get down to the important stuff. 
 0:34: Yeah, sure. 
 0:34: Thank you. 
 0:35: Thank you so much. 
 0:37: Yeah, thank you. 
 0:39: Yeah. 
 0:42: How, how do I pronounce your first name? 
 0:45: Amri. 
 0:47: Amrit, OK, so, Amrit, like, I see that you have been working with a client that is based off concert in Pennsylvania. 
 0:58: Are you located in Pennsylvania or are you working remotely from a different location? 
 1:04: I'm working remotely and I'm like located in Maryland. 
 1:08: OK, OK. 
 1:11: could you give me just a quick overview of your expertise and your most recent project? 
 1:17: Mhm, sure, like, I have 12 years of experience as a like senior Python backend and a full stack engineer, specializing in, building the scalable backend applications and, distributed systems, cloud native platforms, and, like my core expertise includes the Python, Django, class, fast API, rest APIs, in the database. 
 1:39: I know the postpa SQL, MySQL, Amongo DB, Red is Docker, and like most recently, like I worked as a lead Python, developer and architect as well at A version like, generally, where I supported. 
 1:55: And enhance the Python-based backend services like for we can say large scale pharmaceutical supply chain platform and my responsibilities included like the developing the rest APIs troubleshooting the production issues. 
 2:11: performing the root cause analysis, optimizing the database queries, improving the application performance, and also like collaborating with the QAA DevOps and the business teams like to, deliver the, like the reliable solutions and, generally, in Amesource version like my, my roles and responsibilities like included, we can say are developing and maintaining the, Python backend services using fast API class. 
 2:37: And designing the enhancing the APIs integrated with the internal and the third party systems and like the fixing bugs, implementing the enhancements. 
 2:48: So these are the things that that's pretty much all. 
 2:57: are you on mute? 
 3:03: Can you hear me? 
 3:04: Yeah, it's good. 
 3:06: Yeah, I, I hear the echo, so that's why I mute myself. 
 3:11: OK, so, just so you know that like, we are heavily invested in AI, right? 
 3:21: we generally don't write code anymore. 
 3:23: We, we have AI generated code, right? 
 3:28: as a dev team, our job is to make sure the specs are right, the requirements is the code generated that meets the requirements, right? 
 3:39: And it is secure. 
 3:41: We audit it thoroughly before we release it to production. 
 3:46: so we're looking for someone who Has experience in Python because this project is especially based on Python, that's aligned like, well, with the like way I, I, I like to work like basically also like I regularly use the tools, AI tools to accelerate the development, but, like I don't read AI generated code as the production ready by default. 
 4:11: like, my focus is on like, validating that the generated code meets the, functional requirements, follow the coding standards, and it's like a secure performance well, and it's also like the maintainable, and after that like we can say, like I, in, in my experience, like AI helps to improve the productivity. 
 4:33: But as a developer, like our responsibility is to still to evaluate the logic, handle the edge cases, perform the proper testing, and since my background is primarily in the Python with the past GPF class for Django, so I'm comfortable like reviewing debugging and improving the codes. 
 4:52: OK, so like I, I see, it looks like you have a team of multiple team members, right? 
 5:01: So let's say you want them to, one of them to implement an API where someone can like download or pull data or. 
 5:11: Stream data from a particular SD bucket and another one is from the Azure blog storage or something. 
 5:18: So just to make sure like all the developers are, following a certain set of rules or constitution, right? 
 5:28: How would you enforce it? 
 5:31: generally for enforcing, in that type of scenario, basically what I do, like the first thing I do like to make sure, like have the clear engineering standards like that everyone follows and for example, like we, we had the defined API designs guidelines, naming conventions, error handling, authentication, logging, for validation, and the security best practices and, beyond the documenting, documenting. 
 6:00: Those standards like I pose them like through the code reviews because that's where like we verify that the implementation actually follows the the agreed approach and I'd also use the automated tools like the linters formatters, static code analysis and the CICD checks so that the code meeting the standard is the requirement before it can be merged. 
 6:24: And like for APIs like S3 Azure blob access, I'd encourage creating a common abstraction for the shared services instead of like having each developer implemented like directly and that way like authentication and error handling like retrieve the logging and the remain consistent across the applications. 
 6:50: so, like, I, I know you, talked about, So, it looks like it's a platform for pharmaceuticals, right? 
 6:59: Like it's like a supply chain that you guys are maintaining for the pharmaceuticals. 
 7:04: So it's just a solution that you provide for all these pharmaceuticals. 
 7:09: We are making sure they are, integrated with their own clients, right? 
 7:15: So let's say, I, And just thinking, OK, let's say like there is a setup with you guys that you guys are trying to set up, right in between the times. 
 7:31: It's again the same thing. 
 7:33: They're trying to make sure either they're uploading stuff or they're downloading or they're requesting information from those APIs, right? 
 7:42: Did you ever run into like, resource issues? 
 7:46: Like, did you, did you guys have any mechanism in place to handle it? 
 7:51: Yes, absolutely, like scalability and the resource management were like the important considerations in our platform. 
 7:59: Like as we onboarded like more retailers and the partners, API traffic increased significantly, and, generally to handle that like we designed stateless services like so that, could scale horizontally and we, implemented the paging channels and the streaming for the large data sites instead of. 
 8:20: Like, loading everything into memory and also like, use our synchronous processing for like a long running task and apart from that, we also like optimize database queries, added the caching will be appropriate using Reddi and monitoring CPUs, memory, and the APL agencies like through our. 
 8:40: monitoring tools and, on the cloud side like we leverage the auto scaling and the road balancing like to the the handle the the traffic is like so generally these approach ensure the platform remains like responsive and reliable even like or more retailers and the client integrated with other APIs. 
 9:02: So how do you guys deploy your APIs? 
 9:05: Like, you're saying you, like you have this auto scale set up for like horizontally replicating the resources, right? 
 9:15: So how do you, like how, like what kind of process do you guys use for deploying these results? 
 9:21: Yeah, generally, we validate, API deployments at multiple levels like before, enabling the auto scaling and production. 
 9:30: first, we run unit and the integration test like to, verify the API functionality. 
 9:35: So then like we deploy to a staging environment that like. 
 9:40: closely, like closely mirrors production and, like to validate horizontal scaling, we perform load and the stress testing, using the tools like Ginter K6, and we gradually like, increase concurrent users and like monitor monitor masses such as like, response times, throughput, CPU utilizations, memory usage, and some like error rates and. 
 10:06: apart from that, like, we also verify that the application is stateless or so like any replica can handle any request and shared state and if needed, it is stored in external services like, Red or the database and, and last, like finally we test auto scaling by by generating enough load to exceed the CPU or the memory threshold and verify the new instances are like created automatically. 
 10:35: And show the load balances like distributes the traffic correctly and like confirms that when the traffic decreases it like access and chances are like terminated without like impacting the active users. 
 10:52: So, when you, when you have like a So, do you guys like use Mhm. 
 11:06: What is there? 
 11:07: I, I don't know why I hear the echo, So when you're deploying these resources, right, so you're saying that, based on your test, based on the performance benchmark, you're setting up the resources limits so that like they scale up, based on the requirements, And, do you, I mean, like, do you have experience with the, like, Kubernetes or like, function apps or any of these. 
 11:43: Yes, I have like great experience on the Cubans and the things basically, like, generally, I, I, in, I do in my recent projects like I worked with the Docker and the Kubernes for like, deploying and managing the congenized Python application and while like I, I was not the primary Kubernes administrator but like I, I worked closely with the develops teams and also on the deployment. 
 12:07: reviewing the Cubans manifests, config maps, secrets, and, monitoring the, the applications held after the releases, and also we con configured the resource request and we can say limits based on the application's behaviors. 
 12:21: And the monitors, CPUs, memory, and the response times like to make sure the services were stable and Tates handle the scaling based on the workload or we can say and we continuously monitor the applications to like fine tune those settings like whenever they needed and most recently like we have also started using like the AI to analyze the application matrices and the logs like after deployment. 
 12:49: So it helps to identify anomalies, resource bottlenecks, or like the unusual traffic pattern like much faster and or like we still validate the finding manually, but like AI significantly speeds up like the troubleshooting and the performance analysis. 
 13:06: So how do we, how are you, like what, kind of models are you using to actually analyze the logs and how are you feeding them? 
 13:15: Mhm. 
 13:16: generally in our, our team like we primarily use Gup co-pilot and the chat GPT for like the engineering task and rather than the like own AI models and also like we use the cloud, and the cursor like. 
 13:28: and also like you, you, we use it like to generate the boilerplate Python code, create the unit test, explain the existing code, and help to analyze logs or errors message like during the debugging. 
 13:42: So the important part was like that every AI generated output output was reviewed, tested, and validated before it becomes part of the applications. 
 13:52: And like 11 things like most of the AI tools like we use were powered by the the large 1 models such as like the OpenAIs GPT models would be like Chad GPT and the data copilot and from a developer's perspective my focus on like using. 
 14:10: those tools, effectively to improve the, productivity while ensuring the final implementation like me, meta like the coding standard security, requirements and the business needs. 
 14:25: So I know like you talked about like how you guys determine do some testing, right determine it and then, deploy these resources so let's say like These things are all connected like these, these are all client base, right? 
 14:46: So we are deploying this platform on the client end and they have their own customers that they connect to, right? 
 14:53: So how do you guys like, Test this. 
 14:58: Like, how do you test that connection between all of this? 
 15:01: How do you guys mark all of this information? 
 15:03: , like we try to make testing environment as close to the client's production environment as possible. 
 15:11: Like, before deployment, we evaluate the API using the like representative test data and like simulate the, we can say, like the expected workload like to understand how the application behaves like under the normal and the peak conditions and we perform the functional testing, integration testing, and the performance testing like to verify the response times, resource utilizations and the interactions like. 
 15:41: with, dependent services and, like if, if the client integrates with external systems like the storage services or, any third party API, so we also evaluate those integrations in a, staging environment and we use AI to help to, generate the realistic test scenarios and, identify the edge cases that might be missed during the manual testing, but like AI also helps to analyze the test results and the application of logs. 
 16:11: To quickly spot performance bottlenecks and like the like unexpected behavior. 
 16:20: So I the time I. 
 16:26: Sorry, I can't hear you properly. 
 16:28: No, no, no, I'm hearing the echo, so I'm trying to like gather my thoughts. 
 16:33: OK, so I don't know if I remember I mentioned we, we are, we heavily use AI, right? 
 16:41: Do you have any experience with spec-driven development? 
 16:45: Oh yeah, like, I have like like a great exposure on that basically, like I've like started using the prompt-driven development like quite a bit in my the recent work, like instead of writing everything from scratch, I used AI tools like the, cloud or the co-pilot like to generate an initial implementation like based on like the well-defined prompts. 
 17:09: So the key is writing the clear prompts with the business requirements. 
 17:13: expected behavior or like edge cases on the constant and once the code is generated, I don't assume like it's correct. 
 17:20: Like I review it carefully and validate the business logics, checks or like for the security and the performance issues and also like add or modify the unit test and like make sure like it aligns with like the coding standards before it's merged. 
 17:38: OK. 
 17:39: So, like, I know you, you, you were saying, you're looking for security, right? 
 17:45: What would be like the key points that you would look for to identify, OK, there could be an issue here, right? 
 17:52: Mhm. 
 17:53: like, for the security perspective, like, especially like the EI generated code, like I focus on security, from the beginning, like not just before deployment. 
 18:04: Like the first thing like I checked is like. 
 18:07: The input like the input validation to make sure the first thing I check is to the input validation to make sure user input is properly validated and sanitized both like then then I like verify the authentication and authorizations to ensure that users can like. 
 18:25: Only access the resources that they are permitted to, and I also look for the like the common security risks like the SQL injections, command injections, ensure the like the file handling, expose the secrets of the API keys and the sensitive information being written to the logs and if the like API communicates with external services. 
 18:49: I verify like the data is transmitted securely and the credentials are like stored in the secure secret manager rather than the code and beyond the manual review we use static security scanning tools or depending vulnerities and scans and. 
 19:05: Also some like AI assisted assisted food reviews like to, flag potential security issues like clearly like AI is like helpful because it can quickly identify common vulnerities and suggest the improvements but I always like to validate those findings like before making changes. 
 19:26: So, do like, one more question, right? 
 19:31: I like me just forget. 
 19:33: So, like I know you, you are still working at this, right? 
 19:38: So why, why are you looking for a change? 
 19:42: generally my contract was ended like in ISO but then I work as a contract-based developer, so the next, next week my contract was ended. 
 19:50: So that's why I'm looking for the new opportunities. 
 19:52: OK, OK. 
 19:55: do you have any questions for me? 
 19:57: Oh, yeah, like, apart from this round, like, is there any, other rounds, in the future? 
 20:04: Yeah, I, I, the second one will be more technical, right? 
 20:08: It will be probably a different group of, members. 
 20:10: I didn't realize it was a day off tomorrow, so I, like, not everyone is here, so there will be a definitely. 
 20:19: a second round of interview with the more technical questions. 
 20:24: Got it and I have also one more question like, an earlier say like since you mentioned the team like follows an AI first development approach, so I'm curious to know like what AI tools or the platforms like the of the team primarily uses and, throughout the development life cycle, and, like, is it like mainly for the co generations for reviews of the testing also rather than also for like the debugging and the. 
 20:55: everything is GitHub co-pilot that we use. 
 20:58: We, we're not allowed to use anything like that, and for data sensitivity that we have because it's healthcare information that we maintain. 
 21:08: So we use GitHub for private, for everything that we have to generate. 
 21:14: But other than that, like in the office, we don't use any. 
 21:20: Sounds good. 
 21:24: OK, I know, I know it's, it's been only 20 minutes, but I think I'm good on this. 
 21:33: and I will let Mary know, I like we have a few more candidates early next week. 
 21:40: After that, I will let Mary know so that we can, if, if needed, we can set up the second interview. 
 21:46: Sure, sure, Charlene. 
 21:48: OK, yeah, thank you. 
 21:49: Thank you so much. 
 21:50: Have a good weekend. 
 21:51: Yeah, same to you. 
