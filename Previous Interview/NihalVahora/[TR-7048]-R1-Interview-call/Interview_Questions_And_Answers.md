0:00: How's your day going? 
 0:02: Good. 
 0:03: And how, how is your day going so far? 
 0:05: Yeah it's really good. 
 0:09: On some, on something else, Yeah, let's get started, you know, so, a quick self-introduction by myself, you know, I work as a, consulting partner with the Pro Limited, and I look after, And cybersecurity, Consulting and and and and that service delivery and we have a a huge one of the Fortune 500 customers who is giving us a project that includes doing a full start development for one of their Security control project that largely related to the identity and access management. 
 0:57: So yeah, I'm doing a bit of a screening. 
 1:01: It's not a wholesome interview as such. 
 1:04: It is a bit of a screening and then, based on my assessment, we would recommend you to the direct our customer interview. 
 1:15: Sounds good. 
 1:16: Does that sound good? 
 1:19: All right, so have you seen the job description of this role? 
 1:24: Yeah, yeah, I have gone through the job description. 
 1:26: OK, now. 
 1:29: Let's go ahead and kind of do a brief introduction about yourself and what you have been doing in the last two years with that. 
 1:38: Do you think, You know, that arrange with our requirement. 
 1:43: Yeah, absolutely. 
 1:43: So, like, I have around 10 years of experience in software development, primarily focused on Python, to stack development, cloud native applications, and also data engineering, and currently I'm working with like Corewell Health on a healthcare modernizing application platform. 
 2:00: Like, where I develop Python-based microservices using Fas API and Django, and I build rest to APIs and work with Post SQL and Redi and like for data management and performance, and I'm also involved in Docker, Kubernets, AWS, and alsoerraform. 
 2:17: And I have, I also with CICD pipelines and monitoring tools like CloudWatch and Open telemetry. 
 2:24: And like a significant part of my recent work has been around like G AI and rack solutions I can say like where I have worked with document processing, chunking, and embeddings, vector search using FAISS and PC vector and LLM integrations using like Lang chain and yeah, so like. 
 2:44: And that that that's pretty much about me. 
 2:49: Oh, OK. 
 2:51: And, what is your exposure to, you know, have you done any development project in, in any security, cybersecurity oriented, You know, projects such as identity and access management. 
 3:09: What is your, what is your exposure to identity and access management part of the, the development, and what, what kind of development work you have done on that line? 
 3:20: Sure, sure. 
 3:21: So see, like, in development, like I have done, like I have had some experience in like authentication. 
 3:28: So my primary work has mainly been around authentication, authorization, and like policy-based access control for Python migration services and APIs and like we used OR 2 and OIDC for authentication and JW JWT tokens to like securely pass under like identity and claims between services and like I, I also implement. 
 3:49: I go with access controls like their permissions like were validated before allowing users to access specific APIs or like healthcare resources and from the development side, I integrated this security mechanism into like fast API and Django rest API including token validation, authorization checks, and also protected endpoints. 
 4:10: So yeah, like my IM experience is friendly application level and identity and access investment and also like API security. 
 4:17: So yeah. 
 4:18: Oh, OK. 
 4:19: that sounds good. 
 4:22: So you mentioned about your experience, you have worked on authentication and authorization, part of the identity and access control. 
 4:33: can you explain what are the modern protocols that are used. 
 4:37: For, achieving, OK, so, authentication, so yeah, like, in my experience, like the main modern protocols and standards I have worked like with OSS 2.0 and like Open ID Connect or YDC. 
 4:52: So like if I talk about OO 2.0, so it is like primarily used for authorization actually. 
 4:58: So it allows an application to access a protocol resource without like directly handling the user's credentials. 
 5:04: And for example, like in our APIs an access token is issued and the API validates that token before align like access of protected endpoint and another side like open ID so it is it connects you, it is like connect it's built on open top of 2.0 and it's focused on like more on authentication side basically. 
 5:24: So like confirming with who the user is and it provides identity information through like ID token. 
 5:30: I can see and I have also worked with JWT like which securely like I mean it's a it also like it used in like our faster pay and general services like we validate the JWT signature and claims such as expiration, issuer and audience before processing the request and like for enterprise IM I can say like I have exposure to role-based access and also like IEM policies. 
 5:57: So yeah, that's my experience. 
 6:01: Oh, OK. 
 6:02: OK. 
 6:08: yeah, so do you? 
 6:11: What is the construct of a jar token? 
 6:14: OK, so, basically, a constructor of a jar token is like, see, there are like 3, 1st, JWT implements, the contents so they can become like relatively large. 
 6:27: So if we put too many claims or permissions into the, into them, so like since they The token is sent with API request and that can add a network overhead. 
 6:37: So like, second revocation, I, I can say like it is more difficult than with a server-side system and like once a JWTH is issued, it normally remains and valid until it expires. 
 6:50: So like for sensitive applications, I can say like I prefer short-lived access tokens and use refresh token mechanism or then when like immediate revocation is required. 
 7:01: And another important point is that JWT is signed and like not necessarily encrypted, so I never put sensitive information such as like passwords or confidential healthcare data inside the claims. 
 7:13: So yeah, like from a security perspective, I also make sure the application validates the signature, issuer audience and like also expiration like rather than just decoding the token and trusting the claims. 
 7:26: So yeah, that's the. 
 7:29: Oh, OK. 
 7:30: Yeah. 
 7:32: So, how do you set the expiry of the to? 
 7:37: OK, for setting the expiry of token, I can say like, like for example, in a fast TP application when I, when I create the JWT, I add an EXP claim based on the current UTC time plus the configured lifetime and something like, 15 or 30 minute access token. 
 7:55: like, depending on the application security requirement, I can say, then on every API request, the authentication layer where it gets the JWT signature and checks the EXP claim. 
 8:07: And if the token is expired, like, so if the token is expired, the client needs to obtain a new access token. 
 8:14: And for longer user section, I generally use a refresh token mechanism like rather than making the access token valid for hours or days I can see. 
 8:24: OK. 
 8:26: OK. 
 8:30: Yeah. 
 8:33: I said So you know, so it's quicker scenario, right, so if you are building an APA gateway, right, that kind of validates the job tokens, now you must for that I, I'm sure you must be fetching this, keys, such as, you know, from the store, right, from the way ADC provided, you know, jockski store, right, yeah. 
 9:02: So fetching these keys over the network kind of sometimes is slow, right? 
 9:08: And then, like I think you also mentioned that adding like crypto. 
 9:14: OK. 
 9:16: Oh I think your sound is breaking actually. 
 9:23: Am I audible? 
 9:29: Hello Bolawa. 
 9:34: Your, your voice is breaking. 
 9:36: You're, you're not audible. 
 9:37: hello. 
 9:41: Hello, Ravi. 
 9:47: Are you there? 
0:02: Hey, hi Ravi. 
 0:03: Am I audible? 
 0:05: Yes, yes, you are. 
 0:09: Yes, I think I had some, network issue at my. 
 0:13: you are able to hear me. 
 0:14: Yeah, now I can hear you. 
 0:18: All right, yeah, so we were talking about, you know, so all the overheads, right, like for example, doing the signature verification, you know, fetching the keys, and, now how do we, how do share that, the caching mechanism, you know, you need to ensure that caching, caching mechanism, kind of. 
 0:47: Create, you know, allows us to. 
 0:52: To reduce this downtime, you know, doing the key rotation, you know, all those things, you know, how do we ensure that that what kind of a caching mechanism that you will use that reduces this network overhead. 
 1:06: OK. 
 1:07: Are there any downtimes specific to the key rotations? 
 1:10: So yeah, exactly. 
 1:11: Like I would design the, like I would design the caching and key rotation flow so that a key rotation doesn't cause authentication value. 
 1:19: Like, in this scenario, like first I, first thing is like I would use the cash. 
 1:24: As the JWS keys without a controlled TDL, but, I wouldn't simply like delete the old key, old keys when the cash expires and like during normal rotation, the identity provider may publish the new key like while still keeping the old key available for the tokens that we were already using. 
 1:42: So like my approach would be like to keep the current and like to keep the current and recently retired signing keys available for like transition period and generated uses the JWT key to select the correct cache public key. 
 1:58: So like I can say like if a request comes in with a feed the like that isn't currently cached, I would refresh the JW cases and asynchronous asynchronously or on demand. 
 2:09: Like rather than making every request for the identity or adding to the cash and the token is validated again. 
 2:15: So like, I would also use the stale key for that carefully and if the like JWKS provider has a like temporary network outage, we can continue validating tokens with already like I can say with already trusted and non-expired cash fee, I, which I can say like that prevents some temporary identity provider outrage from like immediately taking down authentication. 
 2:40: So, like, overall, I can see the design is like cache keys locally and use key for lookups and also like refresh on unknown key ID and retain the old keys during the rotation and like this keeps signature verification local and like fast while still handling key rotation safely. 
 2:58: So yeah, this will be my approach. 
 3:09: Are you there? 
 3:13: Yes, my birthday again it's it's just another system now it should be OK. 
 3:17: No, yeah, so yeah, we were talking about. 
 3:22: The Yeah, was that that, the store token stuff, right? 
 3:27: Yeah. 
 3:29: Yeah, so, can you repeat your answer for that? 
 3:31: Just. 
 3:32: Like, yeah, like I was saying for like the, I was telling you my approach for like currently, recently retired signing is available like for a transition period. 
 3:45: like, the gateway use the JWTK to select the correct cash publicly. 
 3:51: And like if a request comes in with a kid that isn't currently cashed, I would rephrase the JWKS as synchronously or on demand, I can say, rather than making every request for the identity provider. 
 4:03: And like I would also use stale key for that carefully and like if the GWKS provider has a temporary network outage like we can continue validating tokens and like so like overall I was saying that the design is cast keys locally use kid for lookup and refresh on unknown key IDs and also retain OPs during the rotation. 
 4:25: And also like I, I, I mean like that keeps signature verification local and fast while handling the key rotation safely, safely. 
 4:36: OK, great. 
 4:38: OK, Are you, are you? 
 4:43: Are you still hands on with your coding work? 
 4:47: Yeah, I'm still handsome. 
 4:49: Yeah, OK. 
 4:50: OK. 
 4:52: All right, so, Yeah, so. 
 4:58: Yeah, that would be a, that would be a scenario where you will be asked, so this is like, you know. 
 5:07: You, you will be joining our company and then we would be deploying you for one of our client projects, right? 
 5:13: that client is one of the first kind of client, so they would do a thorough, more technical interview, like I mentioned, right? 
 5:21: So in that interview they will, will definitely ask you to do some on the screen coding. 
 5:27: Yeah, that's OK, they, they're gonna ask you, and can you write this mechanism, for example, can, what kind of a coding you will write if you have to implement, this cash in a, in, you know, look, shows for me that how the class would look like, right, you know, what functions you would call, what methods you would call, all those stuff they would literally ask you to do that, right, which I'm not going to do now, OK, so, so you'll have to be more clear. 
 5:58: It, it's a more of a screening and preparing you for the actual customer interview, you know, right, so. 
 6:05: they are going to be prepared for, be able to write all those, you know, queries, you know, the calls and methods and functions, all those stuff, OK, yeah, I'm comfortable with coding. 
 6:19: OK, OK, great, yeah, so again, the concepts that you mentioned of, ODC what to, and, there is, you know, the, in the in the authorization there is a concept called, fine-grained authorization. 
 6:38: Are you familiar with this, I'm familiar. 
 6:42: what does that mean? 
 6:44: see, like, basically, if, if I say, I can say that. 
 6:50: This, let me, like, yeah, let's see. 
 6:54: The fine-grained, the, the fine-grained authorization means we don't like just decide, whether a user can access an application on a like broad resource. 
 7:03: we make authorization decision at much more detailed level, I can say, but like based on things like the user role and resource and excel and context also. 
 7:12: So yeah, I'm familiar with it. 
 7:16: OK, yeah, do more, do more research on that, you know, you, you, you, you are, Yeah, your answer is still at 10,000 ft, but yeah, just, you know, I, I think you more or less you said, you know, based on, you know, certain policies based on user attributes, based on asset attributes also, that's a good call, right? 
 7:42: You, you kind of, further restricting, you know, can, you know, putting a lot of conditions and restricting, yeah, you can enter into a building, but you. 
 7:51: You cannot access into this particular room, or you can probably enter into this room, but you cannot access this portion of it, right? 
 7:59: And so, so that kind of restricting based on the distance requirement, that's fine grind lot of authorization right so this is again it's it's a security project for one of our fortune 50 customer and they definitely need a lot of AA based genuinely based projects are requirements are out there, so. 
 8:22: So briefly, so, you know, that they will touch up on that part also. 
 8:27: I see you have a, you were on some rat pipelines and all those things, isn't it? 
 8:33: Yeah, thanks for giving me all the insights. 
 8:35: I will make sure that. 
 8:37: I mentioned all yeah. 
 8:39: Right, so, so I think at my high level screening, you should, you are good. 
 8:44: We'll, go ahead and, place you for the customer interview in, it could happen any time this week. 
 8:52: That sounds good. 
 8:53: anytime in this, yeah, any time in this sense, of course, they will, they will discuss with you on the timing and then they'll schedule it. 
 9:02: yeah, so that's pretty much it. 
 9:04: yeah, do you have any questions about anything? 
 9:08: No, I think right now, not. 
 9:11: you already told me like, OK. 
 9:13: Well, can I know one thing, like how many rounds gonna be happen? 
 9:18: yes, so there will be, the next level would be the 100% technical interview. 
 9:24: there will be another interview with the client manager would do that, right? 
 9:29: so there will be tech, there will be technical plus managerial interview, two more interviews after this. 
 9:38: then, you know, if they select you, then, the obvious HR interview would be there, right? 
 9:45: Other, other aspects, onboarding aspects. 
 9:48: OK, so yeah, technically you can expect, 2 more interviews. 
 9:54: OK, that's good. 
 9:56: All right, thank you, Neal. 
 9:58: Your, profile looks good, but, even though you could answer some of the technical related questions, not much entries are there, in your profile if I look at, the IAM related, concepts, right, So you have not even talked about what in your profile. 
 10:25: Yeah, that is one or what it is you see if you can kind of, oh yeah, you have it, OK, I'm back here back. 
 10:33: I'm familiar with that. 
 10:36: Yeah, you can, you, you know what is the back, right? 
 10:39: Yeah, yeah. 
 10:41: What is that, OK, so like, I'm familiar with that concept. 
 10:46: Like, if I mean if I, you talk about like authorization or access control side, like I have worked with the this part as part of my API security implementation and authentication. 
 10:58: So like EAC stands for. 
 11:00: Like attribute based access control and in it instead of making an authorization decision only based on the user's role, we evaluate multiple attributes before like allowing or denying access and those attributes can come from the user resources and requested action and environment also like for example, if I can say in my healthcare project like a request to check whether the user is clinician or not, like which organization or department they belong to. 
 11:28: So yeah, I'm familiar with that. 
 11:31: Yeah, we, yeah, so we talked about fine grain authorization, you know, right, maybe there is, there is a product called, the dedicated product and commercially available product that. 
 11:46: That is used to implement this, pancre. 
 11:49: One of the products is, plain ID. 
 11:53: Just if you want to take a note. 
 11:54: OK. 
 11:55: Right? 
 11:55: Yeah. 
 11:56: Plain, P L A I N I D, OK? 
 12:00: OK. 
 12:01: just browse this product on the public website, on their website. 
 12:05: So, to, I mean, all the things that you, About our back a bag and all those things, they, they literally made a product for that, right? 
 12:13: You don't have to at the coding level you don't have to go fetch the users attributes from ADHR and blah blah blah. 
 12:20: They, they kind of made it a product where you can just do a configuration, not coding, right? 
 12:25: So that, that is one of the products that customer is using it, right? 
 12:29: So. 
 12:31: When you introduce yourself, you can probably talk about it, you know, I'm familiar with the, you know, they will definitely ask you like me, you know, have you done any, what are the, what is your exposure to the security projects and all those things you can talk about you're familiar with authentication authorization, find the authorization, and there is a like a auto back, there is something called a PBAC, P, P as in Poland. 
 12:54: So it's a policy-based access control, where you write a policy, hey, this user has, this attribute, if the, if the asset has this attribute, you kind of mix everything and boom. 
 13:07: When a user logs in, then you like it's a GPU like you put apology and then it. 
 13:13: It becomes easy, right? 
 13:15: So this product client ID you can, you can search www.cli ID. 
 13:20: So you can do a little bit of research, familiarize yourself. 
 13:23: That will be icing on the cake, when you face these guys. 
 13:28: Yeah, sure, I'll do research about ID. 
 13:32: Yeah. 
 13:33: All right, But we, so that's pretty much it. 
 13:38: Neil, nice talking to you. 
 13:41: you know, I'll set you up, last night I tried to set you up with a client, our client, for the technical interview. 
 13:47: Yeah, it's really great to talking with you. 
 13:50: Have a great day. 
 13:51: Oh, same to you. 
 13:52: You too. 
 13:54: Bye. 
 13:54: Thank you so much. 
 13:55: Bye bye. 
