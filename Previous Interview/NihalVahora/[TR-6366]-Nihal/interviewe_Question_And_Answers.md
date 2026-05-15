// Last 15 minutes transcript//


SPK_1
0:00
On my main focus is grounding that that that means the AI should respond based on only on like approved enterprise knowledge data was records and also like APIs and with the like connect connect the system business problem context as well.

SPK_1
0:16
So instead of the like generating the complete like unrestricted response typically I structure the prompt with the like clear system structure business context with that.

SPK_1
0:26
Like for example.

SPK_1
0:28
For example instead of asking us to the AI it's like answer provided by the question.

SPK_1
0:33
Like we would instruct it more like answer provide related question only using the like approved database and API information.

SPK_1
0:41
It's like confidence is low information it's unable to guide the user towards support escalation as well.

SPK_1
0:48
So yeah and like which makes the maintenance and optimization much easier.

SPK_1
0:54
So it's work closely with the business stakeholder to define like acceptable response and tone communication as well.

SPK_1
1:01
So because enterprise AI solution need governance and compliance control and then after deployment we can continuously monitor these things.

SPK_1
1:09
So overall my approach to prompt engineering is really about the balancing AI flexibility with the enterprise control governance and consistency.

SPK_2
1:20
Okay, thank you.

SPK_2
1:21
Actually can you give me an example of what I guess of why or when you chose a guided conversation versus an open ended.

SPK_2
1:28
Like what would make you choose one versus the other?

SPK_1
1:32
Yeah, for the choosing of the guided and like we actually use both approach in our project.

SPK_1
1:37
Like depending on the business scenarios how much control or flexibility was needed.

SPK_1
1:42
Like for example if guided conversation work very well structured process like like password reset or provide credential status we can say ticket creation as well.

SPK_1
1:52
So in those cases the process had like a define a flow and create the connection specific information step by step.

SPK_1
1:59
And for like instance if we provide wanted to check like credential status the board would guide the user thought.

SPK_1
2:06
And if like on the other hand like we used open ended conversation for more like for more informational like explore the scenarios.

SPK_1
2:16
For example user may ask like how do I update provider information and like what document I need to like credentialize and what should I contact to claim uses.

SPK_1
2:27
So in this cases like user ask question many different ways.

SPK_1
2:31
So allowing more natural AI driven interaction giving better experience.

SPK_1
2:36
But even for open end encompassion we still applied like prompt grounding and topic boundaries and fallback handling to keep the response control and enterprise save.

SPK_1
2:46
So overall this decision usually comes down like as a use guide conversation with the end.

SPK_1
2:53
Also the like depend on the requirement as well.

SPK_1
2:56
So use guide we can own the response structure and data collection.

SPK_1
3:00
And for the open ended conversation use need user need the flexibility.

SPK_1
3:04
So in those basis we can select the user guide and open ended conversation.

SPK_2
3:10
Gotcha.

SPK_2
3:11
Thank you.

SPK_2
3:12
Okay, can you tell me they were also mentioning low code platforms but can you tell me about a time when you hit a limitation with a no code low code solution in the power platform?

SPK_1
3:25
So yeah, in the power platform like basically we have the low code low code scenarios and one scenario involved like integrating the Chatbot internal provider management system that had a more complex auto like authentication in response like a transformation requirement.

SPK_1
3:42
Initially we try handling everything using like native power platform capabilities standard connector because we wanted to keep the solution low code and easier maintained.

SPK_1
3:52
But but as the integration become more complex we started hitting the limitation and then the APIs like required the custom token handling, dynamic request processing and like more advanced response transformation logics that that become difficult to manage cleanly inside the power automate along like along like we also the hate the like performance concern because the because the sum of flows are becoming the too large and hard to like troubleshoot.

SPK_1
4:20
So at the end point we evaluate the architecture and decide to decide not to be force everything into the low code instead.

SPK_1
4:26
So we introduced the like Azure function and custom connection connector for the like integration layers.

SPK_1
4:33
So the Azure function handle the authentication logic request transformation and validating the APIs orchestrations while power automate like continue with the managing the business business workflow side and give us a like a clean separate between the enterprise integration logic and workflow automation.

SPK_1
4:51
And also like another benefit for like was like maintainability when we move the complex processing to the Azure function that the flow has become much simple, easier to monitor and like easier for the support team to maintain.

SPK_1
5:06
So this project is really in like reinforced to import the lesson for me.

SPK_1
5:12
So like power platform is extremely powerful for rapid deployment and business automation.

SPK_1
5:17
But more are like scenario where using the like pro code component creating a much more scalable and enterprise ready solutions.

SPK_1
5:26
So this will be my approach.

SPK_2
5:29
Okay, thank you.

SPK_2
5:30
Can you like how do you actually determine whether to use a workaround when you do hit a limitation?

SPK_2
5:35
How do you determine whether to use a workaround a custom connector or even escalated to a pro code solution like.

SPK_1
5:43
To like basically to determine the where we whether we use.

SPK_1
5:47
So that's actually something we like evaluate the quite carefully during the solution design.

SPK_1
5:52
Because it's enterprise project we don't want to like over engineer simple requirement.

SPK_1
5:57
But at the but at the same time we also don't want to force complex logic into the low code tools if it is going to like create long term maintenance issue.

SPK_1
6:07
So usually my first step to understand the complexity of the requirement for from a few different angles like scalability, security and also like maintainability and performance as well.

SPK_1
6:19
So and if the requirement is like relatively simple and can be handled with the native power power platform capabilities without like without like making the solution messy and then it will usually stay with the low code and maybe we can use small workload if the management can supportable like for example if it is a simple transformation condition routing like lightweight automation logics.

SPK_1
6:45
So Power Automate can usually handle it well and but if I start seeing a single like like overly complex flow and repeated workloading patterns so so these difficulty we can use and in a like we like in a magnal health we follow the approach quite often.

SPK_1
7:03
We keep the follow architecture inside the Power Automate but moved complex integration logic into the azure function whenever the low code solution started becoming difficult to scale and maintain.

SPK_2
7:17
Thank you what types of cloud flows have you built in Power Automate?

SPK_1
7:22
Yeah I have worked on so many cloud flows in power Automates but in my project especially in Magnet I built variety of power automate cloud flows depending on the business needs and like.

SPK_1
7:35
First I build a lot of approval flow this these were mainly used to internal process like like access the request and provide the update and service service this approval and I also designed the multiple level approval which is proper like escalation reminder and tracking the taking to make sure that nothing gets stuck and like second I have worked on the integration flow these are the trigger for like for the copilot studio or we can say power apps where where follow calls the external APIs or D365 phase data and also the like.

SPK_1
8:11
The phase data is provide the credential status and send the send the response to the to the chatbot or applications.

SPK_1
8:18
These flows are like usually included authentication and building the JSON and response and the also the the the other one I case creation and service desk flow like for example when a user interact with the chatbot and request support the whole automation create in case that D365 assign and talking about the other flow like I have one more like even driven flow.

SPK_1
8:43
These are the trigger based on the data vers event and I have also like work on the schedule flow if implementing the schedule flow these run are defined on the schedule for the like things like the data sync reporting cleanup jobs and sending the like predictive notification.

SPK_1
9:02
So these kind of thing I have done with the flow and another important like error handling and monitoring flows that I have designed for the follow with like proper try cage patterns et like ETI logic And logging machine mechanism.

SPK_1
9:15
So yeah, just overall I have worked across the approval integration event and even driven schedule workflows.

SPK_1
9:21
These kind of flows I have worked.

SPK_2
9:25
Awesome.

SPK_2
9:25
Thank you.

SPK_2
9:26
So how many years overall would you say you have in it?

SPK_1
9:29
Yeah, I have 10 plus years in it.

SPK_2
9:34
Okay, and then how many years would you say you had with like Ms. Dynamics like power365 or power platform developing?

SPK_1
9:44
So I have like from the beginning of my career I start with Dynamics.

SPK_1
9:49
So I have like around the hands on experience to 9 years.

SPK_1
9:52
Approximately 9 to 10 years experience I have.

SPK_2
9:56
Okay, so primarily all in power.

SPK_2
9:59
Power Automate.

SPK_2
10:00
Correct.

SPK_2
10:01
Power platform.

SPK_2
10:03
And then how many years would you say you have with Copilot Studio for.

SPK_1
10:07
The co pilot studio?

SPK_1
10:09
Like if including my work.

SPK_1
10:10
So I have three to four years experience in that.

SPK_2
10:14
Awesome.

SPK_1
10:15
Yeah.

SPK_2
10:15
Okay.

SPK_2
10:18
If they were interested would you be interested in a contract to hire?

SPK_2
10:23
This is listed as a long term contract.

SPK_2
10:25
I don't want to mislead you either.

SPK_2
10:27
It's listed as a long term contract but a lot of all of our clients actually are open to hiring our people if all goes well.

SPK_2
10:35
And I just know that M and T often looks to retain talent.

SPK_2
10:38
Is that something that would interest you later on after a contract, a potential hire?

SPK_1
10:42
Yeah, I'm interested in.

SPK_1
10:44
Totally good with that.

SPK_1
10:45
Like if they are going to hire.

SPK_1
10:46
So I am pretty good with that and definitely open the long term contract and if things is well on both sides like I have also opened the contract to hire opportunity later.

SPK_1
10:56
For me the most important things to I have working on the right project and contributing the teams long term especially in the areas like Copilot Studio and conversation in my domain especially.

SPK_2
11:07
Perfect.

SPK_2
11:07
Perfect.

SPK_2
11:08
How many years would you say you have as a lead for the lead.

SPK_1
11:12
I have working for the last four to five years I have and last three years I'm working in the current project and previously was I also the lead.

SPK_1
11:23
So if you totally did.

SPK_1
11:25
So my total experience on aliyad is through 7 year experience I have.

SPK_2
11:34
Okay, do you have any questions for me at all?

SPK_1
11:37
Yeah, I have some few question if you could like please tell me about the like what are the next step from here as well and what like just first of all could you please let me know how many rounds are there and what are the next steps?

SPK_2
11:52
Okay, so next I mean I would like to proceed if you're interested.

SPK_2
11:55
So here's what I will do.

SPK_2
11:57
I'm going to send you an email with all of the details about the position.

SPK_2
12:01
I'm going to guess there'll be Two interviews, It's hard to say.

SPK_2
12:06
Typically they'll do one one hour video call that will likely be with Jennifer Truesdale, the hiring manager at M and T Bank.

SPK_2
12:12
Have you heard of M and T Bank?

SPK_1
12:14
Yeah, I have heard about it a little bit.

SPK_2
12:16
You can say, okay, so they're actually a very, very solid company, very strong company in terms of banking.

SPK_2
12:26
I think they're noted for slow and steady increase.

SPK_2
12:30
Not they, they just seem very always moving forward.

SPK_2
12:35
They're a large national bank.

SPK_2
12:37
They're allowed into commercial retail banking, mortgaging.

SPK_2
12:41
They're always involved with community events, sporting and fundraising, that type of thing.

SPK_2
12:45
They're very, very I think solid company.

SPK_2
12:48
Even all through Covid we had a lot of our clients pulled back through things and they did not.

SPK_2
12:52
They kept going.

SPK_2
12:53
You know they don't seem to you know open like a thousand requirements but they never seem to shut down like everybody else does.

SPK_2
12:59
They constant slow instead like we get several requirements every week after week after week.

SPK_2
13:04
So they seem to be moving forward with you know, projects, various projects.

SPK_2
13:09
And I think they're a trendy company too.

SPK_2
13:11
I think you'll, you'll find that you know they're trendy in terms of their skills, the technology tech stack that they use as well.

SPK_2
13:19
But I would, what I'll do from here is I'll email you an email.

SPK_2
13:23
I'll CC the folks at LogicQ so you know everybody's on the same page.

SPK_2
13:26
I'll include the full job description, the internal notes I have from Jen, the hiring manager.

SPK_2
13:31
I'm going to guess to answer your question about interviews.

SPK_2
13:33
I'm going to guess there'll be two interviews but I don't know because she didn't list it.

SPK_2
13:37
A lot of times the manager will list one or two interviews or whatever it's going to be.

SPK_2
13:41
My guess is it'll be two.

SPK_2
13:44
And then once I hear back from you that you're comfortable, I'll go ahead and submit you an agenda today and I'll circle back to you with any next steps or feedback as I hear.

SPK_1
13:53
Okay, that totally sounds good and really good actually.

SPK_1
13:57
Right.

SPK_1
13:57
And complete.

SPK_1
13:58
Let's continue like continuously investing in technology and like and, and for the like you are describing is also sounds like they are serious about the modernization and innovation.

SPK_1
14:11
So especially if they are.

SPK_1
14:12
I was totally like interested in that.

SPK_2
14:16
Yeah, they're definitely I think like I said a trendy organization but you know, not like not state of the art but they're never, they don't seem to be behind in anything in terms of technology leading the way.

SPK_2
14:28
They're a tech hobby here in Buffalo, New York, so they're definitely doing a lot in the technology space.

SPK_2
14:35
Okay, so let me send you an email.

SPK_2
14:37
If you read through everything, if you have any questions, let me know.

SPK_2
14:40
Even if it's more technical than I am, let me know and I'll be happy to ask the manager if it'll, you know, help make or break your interest in the position.

SPK_2
14:47
Other than that, consider this is going to be a six month assignment, they said with likely extensions.

SPK_2
14:52
They will go up to 18, possibly 20, 24 months.

SPK_2
14:56
And then like I said, you never know.

SPK_2
14:58
If you're interested in a hire, feel free to ask that if you get to an interview.

SPK_2
15:02
But like I said, for now it is listed as a long term contract.

SPK_2
15:06
And then like I said, if you have any questions, just let me know.

SPK_2
15:09
Other than that, let me know you're comfortable with everything and I'll go ahead and submit you.

SPK_1
15:12
Yeah, it's totally fine.

SPK_1
15:14
If, if I have a question, I will definitely reach out to you.

SPK_1
15:17
So that's it.

SPK_2
15:18
Okay.

SPK_2
15:19
Yeah.

SPK_2
15:20
All right, well, thank you, Nial, Very nice to meet you.

SPK_2
15:22
I'll email you shortly.

SPK_2
15:23
Other than that, have a nice afternoon.

SPK_1
15:25
Yeah, thank you.

SPK_1
15:27
Thank you as well.

SPK_1
15:27
And have a nice day.

SPK_1
15:29
Bye bye.

SPK_2
15:29
Okay, thank you.

SPK_2
15:30
Bye bye.