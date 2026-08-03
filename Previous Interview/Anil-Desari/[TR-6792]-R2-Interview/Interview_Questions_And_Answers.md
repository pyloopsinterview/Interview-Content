0:02: And. 
 0:03: Hi Ganesh. 
 0:04: Good morning. 
 0:07: Good morning. 
 0:09: How are you? 
 0:12: I'm good. 
 0:12: How are you? 
 0:13: Oh, I'm good, thanks for asking. 
 0:17: All right. 
 0:17: And so, let me just introduce myself for Then maybe we can go forward with your introduction and the the interview. 
 0:26: So myself Janice this side I'm currently I'm working as a senior software engineer, at an IQ, and, I've been associated for around 3, 3.5 years with this company and currently I'm leading a tenure initiative here, where we are trying to develop, various AI capabilities for our NIQ products, and, these are the customer facing products, and there's another JA initiative which is Yeah, in engineering, that is an internal initiative where we're trying to automate various engineering processes like and then SDLC development flow. 
 1:02: So that is one of the other initiatives that we have been working on from the technology stack side. 
 1:07: So, we have been using line graft Nightchain, MCP servers and we have created our own MCP servers. 
 1:14: We have MCP client and A2A for agent to agent communication and fast APX a microsurface layer and databases that uses Snowflake postgrace Mongo DB. 
 1:27: we have been working with DG vectors, for the severity result as of now, and one of our, we have not implemented that rack thing, but RAC is actually implemented by another team, and, it is working on the SGRAI search. 
 1:38: So that is a pretty much a very high level text stack that we use, and this is where we are currently committed to the deliverables that is a high level. 
 1:46: Overview from my side. 
 1:47: Let's let's go forward with your introduction. 
 1:50: Sure, sure. 
 1:50: Like, I'm Anil Kumari. 
 1:53: Like I earned 12 years of experience in, software development, like with a strong focus on, Python API, Django, microservices, and the solution architecture. 
 2:03: currently, like, I'm working as a lead Python developer and architect, like. 
 2:07: At Eleance Health, where like I design and develop the scalable backend services, for the healthcare text platform, and I work extensively with the, fast API, REST APIs, postpay as well, Mongo DB, Reddi, React, and AWS and Azure both, and also CICD. 
 2:28: And recently, like I've been involving the AI enabled applications including the vector databases and the rack-based solutions. 
 2:36: before this, like, I worked with, Fitch Ratings, Modicare, Lemonade, and the Jazz Pharmaceuticals, like, building the, enterprise applications across healthcare, finance, insurance, and the pharmaceuticals domains. 
 2:49: So that's pretty much about me. 
 2:55: Sorry, I was speaking on mute. 
 2:56: You got it. 
 2:56: thanks for providing the background and, so from the AA experience, we are more interested in your A experience. 
 3:03: So we would like to know, I mean, what kind of project you have been trying to develop in your current or or the past or, what, what is your assignment there? 
 3:12: Yeah, like talking toward my project, like, basically in, at, elements Health, my AI, AI work has been focused on integrating the AI enabled capabilities like into our healthcare platforms, rather than, building foundations models from scratch, and one of my recent assignments was the like support, support semantic search and intelligent document, retrieval like for, internal healthcare applications and, we integrated vector databases to store the documents. 
 3:42: Weddings and implemented rack approaches so users could like ask natural language questions and retrieve relevant healthcare documents and the information and generally my role was mainly on engineering side like I design and develop like a Python and the past Gail services that connects the applications with the vector to expose the SDPIs, handle the document retrieval, and integrate the AI services into our existing microservices architecture. 
 4:12: also worked on the API designs, performance optimization, security, and deployment, and Generally, the objective was to make it like we can say easier for internal users to find the relevant information quickly without like mainly searching through the large volumes of documents or this improved like the search experiences while fitting into other existing healthcare platforms. 
 4:41: OK, so when, so you mentioned about, easy, quick searches, so this was all a semantic search with the better database that you were trying to do a kind of a rag approach, right. 
 4:52: Yeah, right. 
 4:54: So, basically, can you just explain your rag architecture, like how you approach it and what was the flow, the rag architecture. 
 5:02: Yes, let's see, in this application, basically, the rack flow was implemented like fairly straightforward, like, first, like we collected the internal healthcare documents, like basically that needed to be searchable, and those documents like were, processed, split into smaller chunks, and converted into the vector embeddings like which were stored in the vector databases and when a user. 
 5:27: Submitted the questions. 
 5:28: Our fast DPS services received the request and converted the user's query into the embeddings, and we then perform a similarity search like against the vector databases to retrieve the most relevant document chunks, and those retrieved documents were like passed as context to the LLM. 
 5:49: Along with the like a user's question, so instead of answering only from the model's knowledge, the LLM generate a response, based on the retrieved documents like. 
 5:59: Which helped improve the accuracy and like reduce the hallucinations and my responsibility was to build the API integrate the vector database with all the microservices, implement the retrieval pipeline, optimize response time and like expose the service like securely for like the other applications. 
 6:24: OK, so let's suppose so in your case, so all these documents were textual documents, right, consisting of the text. 
 6:31: What do you think? 
 6:32: Like, what kind of, documents that actually struggles in those kind of? 
 6:37: What, what are those documents where the rag actually struggles to come up with embeddings or, come up with the appropriate responses? 
 6:44: What kind of documents are these? 
 6:46: talking to like documents like rag generally works very well for the plain text documents, but like it can struggle with documents. 
 6:54: That have a like a lot of structure of or like a visual content. 
 6:59: For example, like a scanned PDFs or like a handwritten documents complex table charts, diagrams, and images are like more challenging because the information is not just like simple text and another challenge is when information is basically we can say. 
 7:18: like, like, spread across, like we can say multiple sections of the document, and when the document contain, domain-specific terminology that is not captured well during. 
 7:30: So in those cases, like the retrieval quality can drop, like they generally affect the final answers generated by the model. 
 7:37: So that's why like reprocessing a good chunking strategies, metadata, and high quality embeddings like become very important. 
 7:48: Yeah, and, and what about the, apologies which is like because see your, LLM or any embedding or this you know the public data, right? 
 7:57: I mean, but I suppose your company is trying to use some jargonic, keywords or the words. 
 8:02: So how it will come up with an appropriate embedding because it does not know, right, that kind of a word because it was not publicly available. 
 8:10: So how your embedding will be proper for this kind of, textual content, like generally. 
 8:17: For the embeddings, what we did like. 
 8:20: since, like, basically a general amending model may not represent company specific terminology or like a domain specific, acronomous well, especially in those like terms are not part of it like it's training data and in that case, like, like there are like the few approaches like, basically one is to build the vector indexes using the organization's own documents. 
 8:44: So, those domain specific terms like, become a part of the searchable knowledge base. 
 8:50: And another approach is like use the domain specific embedding model or like we can say a fine tune the embedding model like if the use case requires it and metadata and preprocessing also helps, for example, we can say expanding agronomous and or like maintaining a business glossary or like we can say. 
 9:11: Adding like additional context like before generating the embedding scanning like improve the retrieval quality and in my project, my responsibility is on the integration side like connecting the back end services with the vector DB and the AI services. 
 9:29: OK. 
 9:30: So, I mean, but, but what see my fine tuning is another example that you're not a reader in the, the wedding model, the internet model, whatever you're using, but what is the quickest approach to it? 
 9:42: Maybe let's see your dictionary of a few words which your which is only private to your company and, I'm a bedding model model actually struggles with that, because it does not, it's not trained on it. 
 9:54: So what is the quickest, solution to it. 
 9:57: let's see, basically, the quickest solution is, like we can say like. 
 10:03: like, I would not, basically retrain the Manning model as the first option because like that's a time consuming and expensive also, like, so the quickest and the most practical solution is to maintain a domain glossary and the synonym, dictionary before like we can say, generating the me links and I would like, pre-process the user's query and expand any company specific terms, for example, like. 
 10:27: we can say if a user search for ABC internally, ABC means like automated benefit calculator. 
 10:35: So the preprocessing layer can rewrite the query to ABC or like simply replace it like with the expanded business terms like before sending it to the amending model. 
 10:47: So this way like the amending model receive like the richest amending context without any of the retraining and retrieval accuracy improved significantly. 
 10:56: So. 
 10:57: If required, the same grocery can also be applied during the document indexing, so that like both the index document and the incoming queries like use consistent terminology. 
 11:08: So that's usually the fastest and most maintainable solutions like in an enterprise environment. 
 11:17: OK, and, let's suppose you have a chat session going on, or do you want to maintain the contextual memory as well because there can be multiple follow-up questions by the user follow-up query. 
 11:29: So what kind of memory is this being called? 
 11:32: What, what is the term that we, what is that term actually called when we try to maintain the context related responses within a particular chat session? 
 11:41: What is that memory? 
 11:43: like to maintain context, across the multiple follow-up questions like, multiple terms within a particular chat session, same, chat session. 
 11:53: So generally like if we use conversations memory also called the session memory or like a chat history memory. 
 12:00: So it, it, it is stores previous users and assistant messages so the LLM can understand references like it, and that document or the like the previous results. 
 12:10: So in framework like Langin or Lang graph like this is typically implemented as like a message history or that like passed back. 
 12:19: to the model on like each request and depending on the application we may use like the buffer memory like which is like stores the complete conversations, window memory like keeps only the last 10 messages like to control token usage and summary and the vector memory as well. 
 12:40: What is summary vector? 
 12:42: summary is basically summarize older conversations like while, retaining important context and, vector is like we can say. 
 12:52: like, generally, vector, is, what we say. 
 12:57: Around it. 
 13:00: Works basically periodically summarizing like the older parts of the conversation instead of like keeping the every messages and as the chat grows, an LLM generates the concise summary of the previous decisions and the summary is like basically stored. 
 13:18: So this is the summary memory that says conversation summary summarization memory, but what is vector mean? 
 13:22: vector is basically retrieves relevant past interactions, semantically when conversations become like very long. 
 13:34: OK. 
 13:37: And I suppose I want to retain some information like there was multiple chat sessions and what, what we will do user preferences, let's say I have a preference to be called myself as a So it is for as a certain name with a certain name, certain name. 
 13:51: So how can we implement this kind of user preference system. 
 13:56: like, generally for retaining the information across, multiple chat sessions, we use, persistent memory or a long-term memory like, unlike, we can say session memory which is like clear. 
 14:10: when the chat ends and persistent memory is like stored in the DB or like a vector store is like associated with the with the user's identity. 
 14:19: For example, like, we can say after the session ends, we can store important users' preferences or the conversation summaries like in the DB, like such as post as well or Mongo DB or like store embeddings in a vector database. 
 14:34: And like when the users basically starts a new session we retrieve the relevant information based on the user ID and inject it into the prompt before like sending it to the LLM. 
 14:45: So generally these allow the assistant to remember things like user preferences previously like discussed topics or like a project context like across the multiple sessions. 
 14:58: OK, I And, and, and when we, when we, when we talk about rack, so we, we re try when we do a similarity search and, on the documents chunks and then we retrieve the most relevant chunks for it. 
 15:15: so how this actually happens very quickly because let's say you have a, I mean thousands of chunks, millions of chunks available. 
 15:23: Our we are actually able to quickly retrieve the most relevant, chunks based on the user query. 
 15:29: Yeah, like, see if we compare the, query embeddings like with every document embedding, so one by one, like it would be too slow, like for millions of documents. 
 15:40: So instead, like, vector databases are like services, like. 
 15:44: your AI search using like the approximate nearest number, the ENN search algorithms like during the indexing, so the embeddings are like organized into the efficient data structure. 
 15:55: So like we can say at like query time the search does not scan every vector. 
 16:01: So instead like it quickly navigates the index to like find the vectors that are like closest to the query embeddings and, after generating the query embeddings, the vector databases performs, ANL search and, returns the top, most similar document chunks like based on the similarity chunks and, also like, similarity matrices, such as like the cosine similarity or the dot product and in many systems this is like. 
 16:28: Combined with the keyword search like a BM 25 as like a hybrid search or the improved accuracy. 
 16:33: So, and because of these specialized indexing techniques and the the ENL algorithms, retrieval remains fast, even when the corpus contains millions of document chunks like typically returning results in milliseconds. 
 16:50: No, but let's say you, we're mentioning about keywords right. 
 16:52: So how keyword combining it with keyword search will make it faster. 
 16:55: There should be some internal, technology link lying behind that which actually optimizes your similarity search across multiples because we are not going to search one by one, each and every, so you mentioned about ANN. 
 17:11: It is one of the way, but, what these vector DPs are actually trying to use. 
 17:18: Enterprise vector I would say, AN is for very internal level of implementation for it. 
 17:24: Have you heard about HNSW indexing, HNS? 
 17:29: Doing,, yeah, like I hear about it basically we can say HNS is like, like we can say a hierarchical, like, navigable, like a smaller like it's, we can say one of like the most commonly used indexing techniques in the enterprise like, we can say, vector databases because like it makes, similarity search extremely fast like instead of like comparing the like query vector or like every stored, vector. 
 17:58: So how it works actually as an index, basically, when a query comes in, the search like starts from the top layer and quickly moves through the graph, towards basically the reason containing the most similar vectors, and once, once it reaches that reason, it performs a more detailed, we can say search in the lower layers and returns the nearest matches. 
 18:22: And because it's like only explores a smaller portion of the graph graph instead of like scanning like the millions of vector retrieval is like a very fast like while still maintaining vector databases like using the edges HNSW as the like the default indexing. 
 18:40: OK. 
 18:41: And when we have, when we do similarity, so there are multiple algorithms like cosine similarity, Euclidean. 
 18:45: So when should we use, cosine or when should we go for Euclidean or our product? 
 18:50: Why always cosine? 
 18:51: Mostly we use cosine, but why we do cosine similarity most of the time? 
 18:57: generally the choice depends on how the model, represents, the basically we can say. 
 19:04: The vectors cosine similarity is like the most commonly used metrics in the rack system because it compares the direction of two vectors rather than their magnitude. 
 19:16: And in semantic search we are usually interested in whether the two pieces of text have the similar meaning. 
 19:22: And regardless of the of the length or the size of the embedding values, that's why I like the cosine similarity, like the default choice like for many embedding models and the vector databases and talking to like Euclidean distance measures, like the actual straight line distance like between the two vectors like generally useful when the magnitude of the vectors also carries meaningful information. 
 19:48: So if the bending model produces vectors. 
 19:52: generally where both distance are like scale are like important. 
 19:57: So if linear distance can be a better choice. 
 19:59: However, like for most can be, like, text embedding, like for most text embeddings used in rack, magnitude is, usually less important than the semantic directions. 
 20:11: Also, cosine similarity like, generally, performs better. 
 20:19: OK. 
 20:23: How do you manage prompts in your current application? 
 20:26: So, like any multiple system prompts, right, or an agent or a a particular node. 
 20:31: So how do you manage the prompts? 
 20:35: talking to our like prompts like in a production rack application we don't have hardcore prompts inside the code like instead we manage them using the reusable templates and the version them separately like. 
 20:50: typically we have a system prompt that defines the assistant roles, behaviors for the library and a user prompt containing the user's query, and a context query basically, context sections like, we, we inject the retrieve retrieve rack documents and optionally the conversation history from the, session memory, we can say to maintain the context and. 
 21:13: We built, we build the final prompt dynamically using the template engines such as the lang changes, chant prompt template or similar prompt, management framework, and we also version prompts like. 
 21:27: Test different prompt variations and monitor metrics like answers quality hallucination rates and the user's feedback. 
 21:34: So generally these allow us to are you using any framework to evaluate this multiple problems. 
 21:39: What, what framework are you using for the evaluation, like, generally in my previous project like, we use, I think, not remember basically, but, like in previous like we usually from using the automated and the human evaluation like first like we created the benchmark and basically the model depends on the use case and we can consider the deployment requirements in our application. 
 22:09: The LLM was traced behind the service layer, so we could not, like we could switch models without changing the application logic. 
 22:18: The focus was like, providing the right context, like we can say through the rack and prompt engineering and the drive rather than the tight coupling of the application to a specific model. 
 22:31: So this approach like give us the flexibility to evaluate different models based on the response quality and latency and the cost. 
 22:43: Yeah, but still the response quality. 
 22:45: So, can you, if you are not using any anything like that, I want, I want to just with the multiple version of long show. 
 22:53: I want to actually use multiple metrics to evaluate the response quality, so. 
 22:59: What is the appropriate way of doing it? 
 23:02: like, see, like, basically if I don't have a dedicated, like evaluation framework, I would create a representative, test data set, containing typical users' queries. 
 23:15: Then, I would run all the prompt version against the same data set and compare the outputs like side by side. 
 23:21: I'd evaluate them based on the correctness of the answers, relevance, to the like the user's questions, groundness, like whether the answer is supported by the retraced, hallucination rates, and if possible, like I'd also have the subject matter experts or like the business users, review the responses and the score them. 
 23:41: OK, and let's say we want to do a token by token, basically on the front end up just like how charge GB or any other mobile pilot is able to do, right, as the execution starts from there and then we start showing it on the screen. 
 23:56: We want to implement the same kind of, feature in our with our back end. 
 24:02: So how you will implement this. 
 24:06: see, like, basically implementation and in this type of scenario like token by token streaming like the GPT, like I would, like use, the streaming capability like provided by the LLM API and on the back end, like back end, like, if we are using the fast GPI I'd, like exposes streaming, endpoint using the streaming, response for the server, server and emails, the SSE, like when the LLM starts generating tokens instead of like. 
 24:34: waiting for the complete response, the back end forwards each token to the client as soon as it's received, and on the front end, React listens to the stream and the app like appends each incoming tokens to the UI, so the user sees the response being generated in the real time. 
 24:53: So basically the overall flow is like user sends a query. 
 24:58: Fast TP calls the LLM with the stream equals to true, and then the LLM returns the token incrementally. 
 25:05: Then after like fast API forwards those tokens immediately using the SSE or like we can see or web sockets. 
 25:11: So, and then like in last the react and updates the display text as like each token arrives. 
 25:18: So, so you implemented SSC API now suppose your blood workflow needs a human input or a human approval in between. 
 25:27: So how you will handle this with SSC API. 
 25:32: like I can implement that. 
 25:34: Like in this scenario, the workflow needs to pause and wait for the human input like before continuing. 
 25:41: I would like to design the workflow as a like we can say, stateful process. 
 25:47: When the like agent reach the step like, requiring human approval, it saves the current workflow instead using the checkpoint or we can say a persistent storage and, returns like a response to the front end indicating that approval is required, and the front end basically displays the approval UI to the users and once the user is approved or like provides we can say additional input. 
 26:13: So it sends another request with the like a workflow ID or a session ID so the back end restores the safe state and, resumes executions from the point of when it was paused, and if we are like using the land graph, this is the naturally supported like through the checkpoints or the interrupt or the resume functionality and if they're like building it ourselves like with the fast API, we had processed the workflow state in the database, all the IDs and the resume processing like when the approval like request arrives. 
 26:48: And what if the user is not providing approval now? 
 26:52: Oh, see, in, in that type of scenario, like, I would not keep the request thread open and waiting. 
 27:00: Like instead I would make the workflow asynchronous and assess the current, state. 
 27:04: And when the workflow reaches the like human approval state like we store the workflow ID or the execution ID, current state pending a details, then the workflow is marked as like waiting for like the human input, the back end can send a notification or the update the UI like that approval is pending and we can define the time of policy like for example. 
 27:28: If approval is received within the configured time, resume executions, and if it expires, either like cancel the workflow, move it to like escalation queue or like we can say execute a predefined fallback actions like, depending on the business rules. 
 27:50: OK. 
 27:51: OK. 
 27:52: I suppose you're trying to Love on an orchestral agent because you love you're working in architecture and you want to know the queries. 
 28:03: From one regime to another or maybe. 
 28:05: Plan a particular flow of the agent execution. 
 28:08: So your orchestra of agent is something which needs to do all this. 
 28:13: So for your designs of this for a moment. 
 28:16: for like, designing an orchestrator. 
 28:21: Basically, I would like to design it as like a central, decisions making area responsible like for understanding the user's intent, like planning the workflow and like, delegating tasks to specialized agents. 
 28:34: So the high-level architecture, would be like, it's like, we can say user request injections and then the request comes to the an API layer such as the fast API. 
 28:44: Then, we capture the user's query, session information and the conversation history. 
 28:49: Then, intent understanding and planning like the orchestrator uses an LLM to understand the user's intent. 
 28:57: It decides like whether the task can be handled directly or like needed, needs one or more like specialized agents and it creates an execution plan for the workforce. 
 29:08: And, like, for example, like document questions like the rag agents, data analyst requests, the analytics agents, security validations, and we have the compliance agents and we have the agent registry. 
 29:21: Like I would like to maintain a registry of available agents with their like capabilities, input output, contracts, and the tools, and the orchestrator uses the metadata to select the right agents and after that, the orchestrator involves the agent. 
 29:39: through like the well-defined interfaces such as, rest APIs and MCP tools and the internal function for complex workflows, it manages the sequences and dependencies between the agents and then after we have the state management and it last like the response aggregations. 
 29:58: OK, so, even when it comes to the altitude, so the accuracy is something which matters the most, how to, how accurately it is able to come up with a plan and the specialized agent execution. 
 30:12: So let's restrict ourselves into the accuracy part of it. 
 30:16: So how you will make sure your orchestrator agent is able to accurately route the request to the right agent. 
 30:26: like accuracy in our, like orchestrator is like, is critical because like a wrong, routing decisions can, like the incorrect results even if the specialist agents themselves are good. 
 30:39: So, generally, first, like I would address some, levels like basically, clear agent definitions and the boundaries. 
 30:47: Like first. 
 30:48: Like I would like to maintain a well defined agent registry where each agent has a clear description of its capabilities, supported task, input outro schema, and the available tools. 
 31:00: So these reduce the ambiguity when the orchestror selects an agent. 
 31:05: And after that, rather than allowing the LLM to generate an arbitrary plan, like I would enforce a structured plan format using schemas. 
 31:27: Hello? 
 31:31: Sorry, I'm speaking again on mute again. 
 31:33: No, so you will be trying to, further enhance your agent skill sets capability and more plan clear description so that our agent understands it. 
 31:43: Apart from tuning this, what else we can do? 
 31:48: apart from tuning, basically improving the agent descriptions like, and the prompt tuning is like definitely one way to increase the accuracy, but I don't think that's like the only solutions. 
 32:00: Like, another important thing is like, like is to give each agent as like a very clear and the narrowest responsibilities like. 
 32:09: when agents have overlapping capabilities, the orchestrator can get confused about like which one, should handle the request and keeping each agent focused on the specific task like improves the, routing accuracy. 
 32:23: apart from that, like I would also use the structured input and the output within the agents, and instead of like passing free form text, I would pass the structured data, whenever possible, so that reduces the ambiguity and makes the next agent job like much easier. 
 32:39: And another thing I believe is like very important is maintaining the context throughout the workflow. 
 32:46: So the orchestrator should pass the relevant conversation history, users and. 
 32:51: , like intermediate results, like the next agent, so every agent has enough information to make the right, like right decisions. 
 33:03: OK, understood. 
 33:05: OK, that's all I have, for myself right now. 
 33:07: Do you have any questions for me? 
 33:09: yes, like, like, basically, like, first I'd like to understand like how the like AI platform and, and, in our organization is currently structured. 
 33:19: Like, are you already using a multi-agent architecture in production or is this is something like, you are actively building and evolving. 
 33:29: It's a multi architecture which is currently serving in production, it's already built and we are continuously evolving it because of the new requirements that keep on coming up on the side, but yeah, in short, yeah, it is something which is already serving production. 
 33:45: OK, apart from like this round, like, is there any round in the, future? 
 33:54: No, this is the, you'll be one more round after this with the director, so that is the that yeah. 
 34:04: OK, yeah, thank you. 
 34:06: Thanks for your time. 
 34:07: Yeah, thank you, thank you. 
 34:08: Have a nice. 
