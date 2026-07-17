0:03: Hi there. 
 0:03: How are you? 
 0:04: Fine. 
 0:05: Hi, Gloriana. 
 0:06: How are you? 
 0:09: I'm good, thank you. 
 0:11: I'm getting, I'm, I'm hearing myself, not sure why. 
 0:17: Am I audible? 
 0:20: Sorry, I audible? 
 0:25: I can hear you, but I'm hearing my voice, like I'm, I'm getting the background. 
 0:29: I'm hearing myself. 
 0:32: OK, maybe. 
 0:36: There's some issue because I'm not. 
 0:42: Sorry? 
 0:43: I. 
 0:45: let's try to continue and, and see. 
 0:52: I will start the recording in 1 2nd. 
 0:55: Sure. 
 1:05: Thank you very much for joining and for your time. 
 1:11: I really appreciate it. 
 1:12: This is going to be a quick pre-screen. 
 1:17: hopefully it won't take the whole half hour. 
 1:22: I wanted to get to know you a little And just ask you. 
 1:26: A couple of questions before you meet with the, the actual hiring manager. 
 1:33: OK. 
 1:39: So, do you have any questions? 
 1:43: No, no, I don't have any questions right now. 
 1:46: Were you, were you advised about, well, a little bit, I'm sure you were advised a little bit about the position, by the partner. 
 1:55: You do know, well, I'm part of Worldwide Technologies. 
 1:58: I forgot to mention that. 
 2:02: I'm a resource manager for them, and I'll be, you know, helping them staffing this position hopefully. 
 2:11: And based on your experience in your CV, I was able to, well, you were one of the top applicants, and that's why we're here today. 
 2:25: So I did prepare, well, along with the hiring manager, some questions based on your experience and Maybe just some things that we wanna confirm, right? 
 2:42: OK. 
 2:43: So, for the first question, you described building metadata-driven masking frameworks. 
 2:52: Oh, before I continue, I'm not 100% technical as you are. 
 2:58: I'm sure you, you beat me on, on that end. 
 3:00: So my terminologies might not be, you know, the best, and I'm sure that You understand what I'm saying, but the hiring manager was the one who, who provided the question, so you guys are good on tech, so. 
 3:21: Let me start first. 
 3:23: You described building metadata driven masking frameworks with IDMC IICS. 
 3:32: So, were you primarily using Informatica native masking capabilities, or did you develop custom Python logic around them? 
 3:42: Can you explain the architecture? 
 3:45: OK, sure. 
 3:46: So, basically, yeah, in my current project, we are building that metadata-driven masking framework like also like capabilities for the actual masking techniques such as like substitution, email masking, or SSN masking, or like phone masking. 
 4:03: So, so instead of like creating and managing those masking tasks like manually, through the informatic IUI, I build, Python automation framework, like around the IDMC, and, the architecture was like meta metadata-driven, and it's, it's, it just, it started, with like Database discovery report that that, you know, contain the schemas tables and data types and columns. 
 4:27: So all, all of those database related stuff like my, my Python application read that metadata. 
 4:35: Then after that identified which column contained that sensitive information. 
 4:40: And then mapped each data type to the, you know, appropriate informatica masking technique. 
 4:46: So based on the predefined business rules. 
 4:48: So once the mapping was completed, the Python application used the, you know, Informatica IDMC. 
 4:55: APIs to automatically create the masking task and like configure them, execute them and like continuously monitor their status and after implementing after implementing those retry logic login exception handling and Report generation happens and 11, I would say like oh yeah, so this is all in short like Informatica handles the actual masking algorithm while like Python handles the orchestration and metadata processing or automation or API in integration thing. 
 5:27: So this is all about the, about your question actually. 
 5:32: OK. 
 5:33: Thank you for that. 
 5:36: this rule includes migrating masking automation from lab to non-production and production environments. 
 5:44: So, can you tell me about a masking solution migration you personally led? 
 5:50: What validation and rollback strategy did you use? 
 5:54: OK, OK. 
 5:55: So, basically, yeah, so, yeah, I have used, work on such, such kind of thing and before every migration, like, we first validated all of the Python automation components. 
 6:05: And like including like configuration files, API connectivity and all and also like authentication masking rule mappings and all like that database connections so we, we also like verify that the, the, the correct discovery reports and the environment as specific. 
 6:23: EML configuration files were being used so that no production settings were accidentally applied to lower environments and like once everything like was validated, we developed the Python automation through our Jankin CICD pipelines and after deployment like We executed a few pilot, masking jobs on a, on a like, limited data sets. 
 6:45: So instead of masking the entire database, we, we can just test that on, on the some some pilot masking jobs so, so that we can know that our services are working. 
 6:54: I mean, what. 
 6:56: I mean, we can test that. 
 6:57: So that's the proper like I mean thought about with that and we verified that all, all sensitive columns were masked correctly and then referential integrity, integrity was like Preserved through the seeded masking and the application would like still functioning and like functioning properly using that meta mask data. 
 7:23: So after successful validation we, we, we, we can execute the complete masking process and generate the execution reports. 
 7:29: So yeah, this is all implementation thing about this particular scenario. 
 7:34: OK. 
 7:35: Awesome. 
 7:36: Thank you. 
 7:38: Have you handled cases where sensitive data could not be automatically masked, such as unsupported formats, pretext fields, or unstructured data? 
 7:50: What happened in your exception workflow? 
 7:54: Yeah, so, basically I have handled such kind of scenario. 
 7:58: Obviously most structured data like names, email addresses, phone numbers, or, or like dates or date of birth, you know, so, so it could be masked automatically like using the informatic IDMC. 
 8:11: So however, we were like, there, there was something exception cases are there. 
 8:15: So especially like free text fields are there, comments or notes or or unsupported data formats are there where, where like automatic masking wasn't. 
 8:26: Reliable that much. 
 8:27: So in those situations like my Python automation first identified those columns first and during the metadata processing stage if the column didn't match any predefined masking rule or were masked or was masked like as unsupported or or the automation didn't try to mask it automatically, so instead it flagged that column as an exception it it captures the detail in. 
 8:53: The exception logs and executed in the masking report. 
 8:57: So, so that that execution report was like then shared with the data governance, compliance teams, and they reviewed that those cases and, you know, decided that appropriate actions or whether it, it's like required a custom masking rule or not or like manual handling is required or excluding that field from the masking process after business approval. 
 9:20: So yeah, that's the. 
 9:22: OK. 
 9:27: these are a little bit more soft skills questions. 
 9:31: How would you describe your communication style? 
 9:35: OK, so if I say about my communication style, then I would try to, I mean, start from the very, I, I will keep like technical discussion simple and make like sure everyone that whether it's developer or like business analyst or whatever the compliance team is there maybe or have some we, we can have the same understanding of the requirement first of all so like if I'm discussing something like technical with a non-technical person whether it can be a teammate or or some stakeholder or some someone so. 
 10:07: Avoid using too much technical jargons or like explain it in a way that, that, you know, he can or he or she can understand the easily. 
 10:17: And I also believe in communication like early whenever, like, you know, I identify like risk or the dependency, like, you know, instead of like waiting sometimes, it, it becomes a bigger issue when, when, when you wait on some, some risk or dependency. 
 10:32: issue. 
 10:33: So during agile ceremonies, I, I like, like daily standard sprint planning or demos or like, I, I just, I always like provide my concise, updates on, on, on my progress or like blockers or, or, or what are, what are the next steps I'm going to take. 
 10:52: So this is what I try to take on my communication site so that, my, my work, always go, goes smooth because of those, actions. 
 11:03: OK. 
 11:03: Awesome, great. 
 11:04: Thank you for that. 
 11:07: Well, those were all the questions I had prepared with the manager. 
 11:14: the next step, well, I will send your information to him and your answers and, and whatnot. 
 11:22: There are other candidates, right, in, in every position, right? 
 11:28: We can't only have the pos position to open for one, unfortunately, but I will be sending all the information of each in in in, in one, and he will tell me who he would like to interview after, and share that. 
 11:47: I will let you know, hopefully he's very responsive, so I will let you know hopefully no later than the end of this week. 
 11:56: And if you do receive anything, that will be coming from me, any type of invites or anything like that. 
 12:04: OK, so if you're not able to make it, how, how are you, how's your schedule for, for interview? 
 12:12: Is it open? 
 12:13: Yeah, I'm open for the interview, yeah. 
 12:17: OK. 
 12:17: Are you currently unemployed or, basically, that's my going to be the, my project, my, my contract is going to be end this week only, so I can join very soon ASAP, yeah. 
 12:29: OK. 
 12:30: So, all righty, Gloriana understood. 
 12:33: Yeah, I have a question like, may I know how many, how many rounds are going to be there, for this particular position. 
 12:41: potentially 2 more after this one, yeah, and if we're able to, I know the, the manager, if he's able to get. 
 12:51: The people in one, in only one next interview, then we will do only 1. 
 12:56: OK, OK. 
 12:58: Just that it will probably take 45 minutes instead of 30. 
 13:01: Got it, got it. 
 13:03: OK. 
 13:03: Mhm. 
 13:06: Any other question? 
 13:07: No, no, Gloria, like it's, it's, I'm, I'm comfortable from my side, yeah. 
 13:12: Awesome. 
 13:13: Well, I really appreciate your time. 
 13:14: It was great meeting you, and I hope you have a great rest of your afternoon. 
 13:19: Thank you so much. 
 13:19: Thank you so much. 
 13:20: Thank you. 
 13:20: Have a nice day. 
 13:21: Bye-bye. 
 13:22: Bye-bye. 
