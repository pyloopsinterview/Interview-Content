0:00: . 
 0:02: Yeah, quick intro myself is Ravi, I, and, I work as a consulting partner with the Pro Limited, and, we are looking for candidates who has, full stack development experience, preferably work done, you know. 
 0:22: Security related projects where identity and access control management was involved. 
 0:28: this, this, position that we have received from one of our elite customers, so you would be, if you have found fit, you will be working for that customer, but in the roles of people. 
 0:41: OK, OK, sounds good. 
 0:44: All right, so, yeah, have you seen our job description? 
 0:48: yes. 
 0:49: OK. 
 0:50: Now go ahead and introduce yourself, and I'll cover. 
 0:55: how do you, where do you think you, you are fit for this position based on the job description that you're seeing? 
 1:01: OK, so, sure. 
 1:04: Hi, my name is Lajender Singh. 
 1:05: I have, over 11 years of experience in like software development, primarily as a Python full stack and, lead Python developer. 
 1:15: Currently, I'm working with, Selective Insurance where I am building. 
 1:20: And like modernizing cloud native applications using Python, fast API, Django, and React as well. 
 1:30: I also have a like good exposure to IAM and application security, and I have worked with OR2, OIDC, JW 2, RBAC as well. 
 1:45: And if I talk about like on the cloud and dev ops side, I have worked with AWS, Azure, Docker, etc. 
 1:55: and so overall my experience is like a combination of hands-on on Python development as well as full stacks application, microservices. 
 2:06: So yeah, this, this is much pretty much about me. 
 2:11: OK. 
 2:12: OK. 
 2:18: All right, so let's talk about, you said you are familiar with the, security, the YZ and war too and all those, security related aspects, right? 
 2:29: Yes. 
 2:30: Right. 
 2:31: OK. 
 2:34: Oh, right. 
 2:35: So you know, what's the, what, what is authentication and what is the authorization? 
 2:40: Is it the same? 
 2:42: So, no, it is not actually the same. 
 2:44: Authentication and authorization, they totally are different. 
 2:48: Authentication is basically like verifying who the user is and authorization happens like after authentication and determines what that authenticated, you know, like user is allowed to do or not. 
 3:04: Mhm, yeah, OK, so. 
 3:08: how do you implement, both? 
 3:11: What is your experience on implementing both for any, application that you have developed? 
 3:16: OK, so if I talk about like the implementation side, so I usually implement authentication like through an identity provider using OR 2.0 and OIDC. 
 3:30: And once the user logins, we receive a JW2 access token. 
 3:35: And on the back back end side, for example, like in past API, we validate the token signature as well as, issuer audience and expirations before allowing the request and like for, for authorization, part after the token is validated, I use that information like roles, scopes, and as well as groups or other user attributes like to Actually decide whether that user can perform a particular action on a resource and in that, all that cases, I have worked with both RBAC and attribute-based authorization for this. 
 4:19: So yeah. 
 4:20: What's the difference between RBAC and ABAC? 
 4:23: So the major difference between, RBAC and ABAC is like, firstly, RBAC is a role-based access control where like, permissions are assigned based on the user's roles, and AB ABAC is like actually attribute-based access control, which is more fine-grained. 
 4:44: Mhm, yeah, so like, instead of like looking only at the role, we make the decision using like attributes of the users, resource, actions, and as well as environment. 
 4:58: And if I talk about like an example like if two users may both have like a manager role, but the ABAC, but with ABAC one manager may only access insurance records belonging to like the region or department. 
 5:18: So yeah. 
 5:20: OK, OK, so where do you get those, attribute, you know, what do you attributes from? 
 5:26: So I actually get that, like from, actually that attributes mainly come from multiple sources. 
 5:35: It, it depends upon the applications. 
 5:37: Like if I talk about some of the common sources are like the identity provider, Active Directory, HR systems, database, and etc. 
 5:49: OK, yeah, How do you implement, can you, you know, you are still, hand. 
 5:58: Uncoding, right? 
 5:59: Yes, yes, yes, right. 
 6:03: Yes. 
 6:03: So, will you be writing, can you, is there a way you can quickly write a A few lines of code about. 
 6:15: Implementing a robust caching mechanism for the token caching mechanism. 
 6:21: So what, what is the strate, let's talk about the strategy, right? 
 6:24: How do you implement a robust, caching mechanism, which is Which is very resilient and in terms of the networking, network overhead transmission overhead or any failure to fetch the keys from the key provider. 
 6:44: what kind of measures you will take when you're going. 
 6:48: So if I perfectly talk about, like, yeah, the measurement is like, for token validation, like, especially, when like we are dealing with the JWTS and like remote JWKS or like a key provider. 
 7:08: I like, normally avoid calling. 
 7:11: Identity identity provider for every request and I use a like a multi-layer catching strategy so that token validation remains like, you know, fast and also continues to work during temporary network failures and at a high level like I would catch the JWKS signing fees locally with the PTN so that like when a token comes. 
 7:38: In first check the local cat using the token screen and like if the key exists, I validate the JW2 JWT locally, so like there is no network call on the normal request part. 
 7:53: And like if the, if the key is like something missing, for example, because of any key rotation, then I refresh the JWKS from the identity provider. 
 8:05: And like I would also implement timeouts and retries with exponential back off, stale catcher fallback, and also, also as a like a, as well circuit breaker too. 
 8:21: Mhm. 
 8:22: Yeah. 
 8:23: OK. 
 8:25: What method you will use to get the key. 
 8:28: So the basic, yeah, but basically that method will be called as like, for like JWD validation. 
 8:38: I would like normally get the. 
 8:41: Signing key from the like identity providers JWK's endpoint and like firstly, I read the key from the JWT header and then like I look for that kid in my local or like distributed catch. 
 8:58: OK. 
 8:59: Yeah, OK. 
 9:03: All right, Do you know what is, In terms of. 
 9:15: That's refreshing, right, right, You know what is that baseball reference is. 
 9:24: What does that stand for? 
 9:26: So, basically if I tell her a graceful refresh means like we refresh the like cach keys, without immediately throwing away the existing valid key. 
 9:39: Like for example, if my JW JWKS catch is nearing expiration. 
 9:46: I can like, you know, refresh the keys in the background like by continuing to serve requests until or using the current cache keys and also like the during K rotation, if, if I see any of the unknown kid, I Like trigger an immediate JWKS refresh and like retry the validation once with the new keyset. 
 10:12: So like the basic, the idea is to keep serving requests with the valid cache data while refreshing in the background as well. 
 10:21: So yeah. 
 10:22: Instead of blocking requests. 
 10:26: Yeah, so that's. 
 10:29: That should be one of the when we talked about robust cash me. 
 10:37: So you, you, you could have called that, call that out, right? 
 10:42: So graceful mechanism is one way where you provide more resiliency to the user experience, right? 
 10:47: You don't just cut them off, you know, and asking them to send in multiple requests until you get the new token. 
 10:57: Right, so OK, and, you, you mentioned you have worked on, you have worked on some genny projects, building the Iraq pipelines and all this stuff. 
 11:07: Do you have the experience on that? 
 11:09: Yes, yes, I have. 
 11:12: Can you walk me through, OK, a little bit about what you've done on the rack. 
 11:19: OK, so, absolutely, yes, I also have hands-on experience with like Gen AI and rack-based applications, like, particularly in my recent work at Selective Insurance, like, 11 of the use cases involved like, providing, intelligent access to enterprise information where we Like, dealing with documents such as PDF and HTML and Markdown. 
 11:48: So like we built a pipeline where we first extract and clear the content and applied appropriate chunking and metadata strategies after that generating embeddings and storing those embeddings in a like. 
 12:02: Vector store for semantic retrieval and then when I like a user submitted a question, we generated the query embedding and all performed after that vector similarity search retrieved like the most relevant chunks and passed that, you know, context along with the prompt to the LLL. 
 12:24: And I have worked with also an OpenAI and Azure OpenAI along with frameworks such as Land chain and vector technologies including Fis and APG vector, and I was also involved in like, improving, the quality of the like pipeline through, retrieval, If I talk about retrieval tuning and chunk size and overlap adjustments, metadata filtering also as like prompt engineering, so yeah, my experience is like not calling an LLM API but I have worked across the end to end rack pipeline. 
 13:07: So from document injections and embeddings to retrieval, so yeah. 
 13:12: No. 
 13:13: Look, we, that's from all the questions I have for now, OK, right? 
 13:19: So let me walk you through what is next. 
 13:21: What is, OK, what is next? 
 13:24: OK, OK, OK, OK. 
 13:27: So like I said, we are going to place you in one of our client projects, right? 
 13:32: You will be on the the pro payroll if you are selected. 
 13:35: So that client will do that, we'll do two rounds of interviews after this, OK? 
 13:44: They will be more deep dive into all those concepts that we discussed, right? 
 13:50: They will technically ask you to write down the code, pick up an old reward card, and then. 
 13:56: in our own notes and then they will ask you to write down the code on the screen. 
 14:00: Sure. 
 14:01: So be ready for that, OK? 
 14:04: be ready for to write the code, you know, whatever you do, how do you implement the cache? 
 14:08: Can you write the clause, and you call the method and all those things they'll ask you. 
 14:12: OK. 
 14:13: so, There will be an interview anytime this week. 
 14:17: Kash from our HR team will reach out to you to schedule that, right? 
 14:21: Once you clear that, technical, fully technical interview, and there will be a managerial interview, technical managerial interview from. 
 14:30: From customers, sure, sure, right, so there will be two interviews from our customer before you are, you are talking on the onboarding part. 
 14:39: Sure, that sounds good. 
 14:42: Any other questions you have for me? 
 14:44: No, no, not currently. 
 14:46: you have explained me so much for that one. 
 14:52: No problem. 
 14:54: yeah, the only thing I wouldn't, I couldn't test you was actual programming on the coding guide so that I am processing you will be asked to do a coding on the screen, and then let's, be, be ready for that. 
 15:05: Yeah, yeah, sure. 
 15:06: Sounds good, perfect. 
 15:09: All right, thank you, Linda. 
 15:10: Nice talking to you. 
 15:11: Thank you and bye. 
 15:12: Have a good day. 
 15:14: You too, man, bye. 
