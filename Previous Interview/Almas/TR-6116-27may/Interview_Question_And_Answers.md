0:00: , and on such short notice. 
 0:08: do you go by, do you go by Almas? 
 0:11: What's your, what is your name Male on your resume and Almas in the meeting, right, right. 
 0:18: So, yeah, you're saying, right, so Almas Malema. 
 0:27: And then Yeah, yeah. 
 0:38: full name is like Mohammad El Basmale, so that is the exact full name. 
 0:44: OK. 
 0:47: Thank you. 
 0:50: My name is Jamie Chou. 
 0:52: I'm founder of Fusion Technology, and Steven is our senior AI engineer. 
 0:58: We both will ask you a few questions and then give you a chance to ask us any questions you may have. 
 1:06: so I will start and then I hand over to Steven. 
 1:12: Again, thank you for, quickly joining us. 
 1:15: on your resume, it was very impressive. 
 1:20: I wanted to ask you a couple of questions about the And Latin language model. 
 1:28: And have you worked with any of the larger leading large language model? 
 1:34: Of course. 
 1:36: So basically, we talk about the large language module models then, immediately I got the chance to work on like, open AI models like, JPT4 or for the like Conversational part and all and also like so there are some cloud models that I wrote on which for the which helps me a lot for the Code and coding and all and then after that, like my involvement was more on the back end integration side. 
 2:06: So building Ay APIs and streaming responses using SEC and handling concurrency orchestration, and also like integrating LLM work flows into the scalable microservices. 
 2:19: So these are the, I mean, what I got the chance to work on and I also like work. 
 2:25: You know, like promptoxication and also context handling, also, like real-time streaming responses for printing applications. 
 2:34: So these are the, We'll kind of gone through that. 
 2:40: Very good. 
 2:42: have you looked at the open source model before? 
 2:45: Open source. 
 2:50: which one you worked with? 
 2:52: OK, so yeah, if, if I talk about like which one, so like I, I worked with the drama be, especially like through hugging face integration and also like, also explore like, for I mean models for the lightweight in infants, for and faster responsive, scenarios like in one of the Implementations we evaluated like open source model for document summarization and also internal knowledge of rival workflows. 
 3:25: So my role was like mainly around integrating the models into backing services, handling interface, and like. 
 3:33: Inference, pipelines like using request processing and like optimizing the response handling. 
 3:39: So overall, so, what I found like interesting with open source models in the flexibility like. 
 3:47: Around deployments and like customization and especially when when latency and custom optimization is there so or like data privacy becomes important, then then it is very much useful for that. 
 4:02: You mentioned the customization. 
 4:03: What kind of customization you have done? 
 4:06: OK. 
 4:06: What the source. 
 4:09: Yeah, so basically, if I talk about the customization, then mostly, around the model behavior for like businesses specific, workflows like rather than, you know, training a model like completely from the scratch, we have done a custom customization. 
 4:27: regarding that, also like, in, in my project, like, we customize the prompting and the travel flow for like document based, question answering like we build, processing pipelines through, chunk documents and generated the embedding and also retrieved context dynamically. 
 4:48: Before sending it to the model that improved like responses and relevance significantly and we also customized streaming behavior and also response association and instead of waiting for the complete outputs we implement incremental token streaming using SSE or users could, you know, see responses in real time. 
 5:10: So that is the customization as we've done with that. 
 5:17: OK. 
 5:20: have you done the semantic search? 
 5:23: Of course, yeah, I have done the semantic. 
 5:28: In what kind of area you in implement the semantic search. 
 5:34: OK, OK, so like The basic idea was converting like document chunks into the embedding and storing them into a vector index. 
 5:44: Then whenever like a user is asked a query or regenerated embeddings for the query and retrieve semantically similar content like instead of doing like only. 
 5:58: Keyword research. 
 5:58: So that is, we used, that mainly for the enterprise document and healthcare operational data and also like, where exact keywords will may not always match, but the meaning is it's still related. 
 6:11: So that significantly improves the retrieval quality for summarization and question answering and like contextual, contextual LNM responses. 
 6:21: So that is the proper use of that. 
 6:26: So if I have a, a situation, a real-life situation for the medical scientific research, right, and then all the competition can be indexed and By this. 
 6:43: Term terminologies right industry, medical industry terminology, so all those things When I was looking for, trying to figure out the semantic search to figure out a solution, to find another data set to see any, more relevant cross-reference. 
 7:08: Right now it's less than 2%. 
 7:11: Those two data sets have anything in common. 
 7:15: Just, you know, purely use a foreign keys to connect those two data sets, we can only do about 2%, less than 2%. 
 7:25: So our thinking is to use a semantic search to look at the two data sets and then maybe increase the chance to get more Meaning of the two data sets and the cross-reference each other. 
 7:42: So if you are put into this project, what kind of things you, you would take? 
 7:49: What kind of technical step or technical approach you want to. 
 7:54: King Kong. 
 7:56: OK, so if I have to work on this exactly scenario, so, that's actually a very interesting, I would say, use case. 
 8:04: So especially in the healthcare and, scientific research, where exact key ways the relationships are usually. 
 8:11: like, I would say very limited. 
 8:13: So if, if I were working on this, project, then I would approach it through the multiple layers like instead of relying only on the direct relational mapping. 
 8:24: So first I would like to focus on. 
 8:27: Like understanding both data sets, semantically, like meaning not just, you know, column to column matching but understanding like the actual medial context, you know, medical or, terminology like medical, terminology and like research concepts and like. 
 8:47: You know, there are drugs, observation, observations are there, medical observation, diseases, means, for procedures, so like that, then I would, so from there like I would, probably build an embedding-based semantic indexing pipeline. 
 9:02: So that, you know, high-level approach would be something like processing the normalized, both data sets and also like a standardize the medical terminologies and also. 
 9:15: Generate the embeddings for records or you know, document charms and store them into the data, like vector database for sure and then use the semantics similarity search to identify hidden relationships between the data sets. 
 9:29: And yeah, so after that we can like, I would also introduce domain. 
 9:35: Specific models or medical embeddings because healthcare terminology is very specialized. 
 9:41: So general embedding, sometimes you miss the medical context, I would say. 
 9:46: So probably I would combine the semantic similarity or metadata filtering or so that, that is the, I mean, approach I would. 
 9:55: Take and this is exact I mean that and the system can say like these records have some higher number of contextual similarities based on, you know, medical terminology and research patterns, yeah. 
 10:11: Thank you. 
 10:14: I don't have any more questions. 
 10:16: Do you have any questions you wanna ask me? 
 10:20: Before I leave, OK, OK, let me hand over to, Steven now. 
 10:27: Steven, you go ahead, please. 
 10:28: Thank you, Steven. 
 10:31: OK. 
 10:33: yeah, so, some of these questions will be, very basic, but, so could you explain to me, what is a, pull request or burnge request? 
 10:48: OK, OK. 
 10:50: So if you talked about the, it's, it's in data environment there are some of it's basically like, code review and collaboration mechanism using, you know, it gets, based on a development workforce. 
 11:03: So typically when a developer finishes a feature boxess or enhancement. 
 11:09: They create a separate branch, and come make their changes there. 
 11:13: So then there is a request to merge those changes, into the main branch or like developing branch. 
 11:21: So the main purpose is to, you know, to review or discussion. 
 11:24: So in my project like pull request are also like tied with CICD checks like unit test or Security checks or like bill validations. 
 11:33: So before merging the pipeline ensures the code is stable and follows the project standards. 
 11:40: So yeah, so usually like during review we check code quality and performance. 
 11:46: Once reviewer like approved and all checks passed, then branch gets merged into the target branch. 
 11:53: That is the whole I mean difference on that whole scenario I would say. 
 11:59: So when you're, have you ever done, code reviews before? 
 12:07: so if, let's say you're doing a code review of, Python code, how, how would you go about doing that? 
 12:15: What sort of things would you, look for? 
 12:19: OK, so if I have to like exactly review the Python code only, then I usually look at it, like, from I, I can see multiple perspectives I have like, not just whether the code works, whether it's, production ready or maintainable, but, is the code clean, like easy to understand first of all, like our functions and classes like properly organized, or are naming conventions, meaningful, looking meaningful or not. 
 12:49: also we can say like best practices we should follow like, typing and ty hints should be there. 
 12:56: I, I would look into that. 
 12:57: And I think you just, if applicable, we, we should use that, I think, properly and also like proper exception handling should be there. 
 13:07: And also like we can, we have to like avoid the unnecessary complexity first of all. 
 13:12: And after that, I would focus on the performance and scalability from there and like unnecessary data, database calls or like inefficient loops some people. 
 13:23: Like, you know, like, and also like memory hoy processing, they are doing. 
 13:28: So I would like, look into that and also API validation or also like security councils we can look, if I'm going to review the code and also like, there are many things to look into the food like, is it resilient in production or not like timeout handling or, add impotency or like, failure recovery. 
 13:52: So the these are the, I mean, points I would try to check and after the I check testing coverage then whether unit test and integration tests are sufficient and whether the code can be deployed safely then through the CICD pipeline, then I would, that, that is the process I would say. 
 14:11: OK. 
 14:18: So, in, could you tell me what, what is a component in react? 
 14:31: So I would say like component is the basic fundamental unit of React. 
 14:35: Like, basically like component is a base reusable building block, of the UI. 
 14:41: So instead of creating an entire page as one large file, RAC breaks the UI into a smaller independent pieces called components, and each component handles its like own structure logic. 
 14:56: Also sometimes, speak, speaks also it can happen, so yeah, there are so many types of company we have, we have, we have to create in that. 
 15:05: So that it's all about something. 
 15:17: could you give me a, technical explanation of, rag, RAG, in the context of machine learning? 
 15:25: Of course. 
 15:26: So if I don't have to talk about the rags, then rag is a tribal augmentation, like, generation. 
 15:34: So, Technically it's an architecture pattern where a large language model is combined with an external knowledge of retrieval system to generate the more accurate and context aware, I would say responses and normally an LLM only answers based on its, you know, trained knowledge. 
 15:55: So if rather before like. 
 15:59: generating the response, the system first, you know, retrieves the relevant information from the external data sources like documents or rap test tools or you can say enterprise knowledge bases or PDFs and databases. 
 16:13: So many things are there, externally. 
 16:15: So, typically, rack shows and, you know, first documents are turned into, smaller sections. 
 16:22: And embeddings are generated for those chunks and stored in the active database. 
 16:27: So then, when a user ask a question, the query is also like converted into an embedding and semantic search retrieves the most relevant chunks. 
 16:37: And finally, like LLM generates an answer like grounded on the retrieved. 
 16:43: information instead of relying only on the prete knowledge. 
 16:48: So, that is the whole drag and also like we have to, properly train the system LLM model through, this process because, we, we, we generally use the word hallucination because hallucination is the case when the LNM model doesn't know the proper answer, but it is because due to of its inherent nature, it has to, it is giving the answer, I mean, according to its own understanding because it doesn't have the proper knowledge of database, of the, of question. 
 17:23: So that is the case, where that helps us a lot through the proper training of, proper data, we can. 
 17:32: And improve the responses of the L1 models. 
 17:39: OK. 
 17:40: so how do you, create the embeddings for, For that knowledge base. 
 17:48: OK, so if I have to create the embeddings, then, typically embeddings are created converting like text into a high dimensional numerical vectors. 
 17:59: So using them like, embedding model, the process is like, starts with preprocessing the. 
 18:08: knowledge-based samples, research papers, medical documents, database records, like they are first cleaned and split into like smaller chunks because, sending entire large documents directly and is not that efficient. 
 18:23: So after chunking, each chunk is, passed through an embedded model. 
 18:28: The, the model converts the, semantic meaning like, like of the text into a vector representation first of all. 
 18:36: then those vectors are stored in a vector database like Pinecon or like Chroma, open source vector data indexes, so like that, and after, user ask a question, we generate embeddings for the query as well and then perform similarity like search between the query vector and the store document vectors. 
 18:58: So yeah, so in, in practical systems, 11 important thing is like chunking strategy because chunk size directly impact the. 
 19:06: The travel quality for it. 
 19:10: OK. 
 19:15: So, how do you determine the similarity between two vectors? 
 19:23: Again, if I have to like, find a similarity between the two vectors then, usually like, like between vectors is, like it is calculated through like using matrix like, cosine similarity I know that, also like do dot product also and also like. 
 19:43: I, I know one method like, Euclidean, distance in, in semantic so it's like a cosine similarity is probably like the most, commonly used, first of all, so the idea is that, embedding representing like similar semantic meaning. 
 19:59: They will, will point in, you know, similar direction in the vector vector space. 
 20:04: So where a query embedding is generated, the vector database, compares it, like against the stored documents, document vectors and like, calculate the similarity scores like higher cosine similarity means the vectors are, semantically closed. 
 20:21: So this is the whole, I mean, I would say comparison problem. 
 20:27: Try to Yeah, so, what is, fine tuning in the context of LLMs? 
 20:36: OK, fine tuning is very, I would say important. 
 20:39: Like fine tuning is basically, the process of taking pre-trained, language model and trained it further on the domain specific for, task-specific, data so it performs, you know, better for, a particular use case. 
 20:56: So, generally, like, LLM already understands the language properly. 
 21:00: So if you fine tune it on the medical research data and healthcare terminology on or like whatever like domain you want to change, so compare it to RA and fine-tuning changes the, you know, models, Internal weights like where that keeps the base model like unchanged and and it injects the external context during the runtime. 
 21:24: So this is all like fine tuning is usually like when you want consistent and dooming behavior specialized like formatting or classification. 
 21:34: or that like task specific outputs. 
 21:37: So yeah, but the dynamic enterprise knowledge that changes like frequently, that is usually more practical because you can update the knowledge, based without, without retaining that knowledge. 
 21:47: So that is the, I would say different or, fine tuning for you. 
 21:54: OK. 
 21:55: so, did you know any, Approaches to fine tuning, Talking to them, yeah, yeah, so fine healing approaches are there if you feel I know about those like, yeah, like. 
 22:13: Depending on the use case or model size or like infrastructure constraints are there. 
 22:18: So the traditional approach, I know like where all models parameters are updated using like domain-specific training data, but for very large models like that this becomes you know expensive in terms of GPU and memory usage. 
 22:32: So, I know that in current current days like parameter efficient fine tuning approaches are more. 
 22:40: Like common, I would say like. 
 22:44: 11 popular approach I know is Luda, like, which is also like a low rank adoption, and instead of, you know, updating the entire model, it, it means like a smaller low rank, matrix on top of the adjusting. 
 22:59: It's, it's more, you know, much more efficient and widely used as well. 
 23:04: So another approach I know that PEST, which is more, like an umbrella category for lightweight tuning techniques. 
 23:12: So this is, I mean, I, I know that. 
 23:16: So yeah, these are the approaches. 
 23:20: OK. 
 23:20: Thank you. 
 23:22: do you have any, questions for me? 
 23:27: currently see, I would like to, like, know about the exact work we are going to do on this, rule, you can tell you because, I, I understand a bit about from the GD and all, but I just want to understand like on what. 
 23:42: feature or what, what you, what we are trying to achieve or what we are trying to fix, yeah. 
 23:50: yeah, so you're gonna be, Working on, OK, improving, search capabilities. 
 24:05: basically, The, historical search was a, a simple, You know, keyword, Matching the search and we'll be working on. 
 24:27: Doing, you know, AI assisted search, And The other thing is, linking together, Some, two data sets which are, Hierarchical, medical, Data sets, And, Basically, creating, Relationships between those two data sets so that if you like. 
 25:24: Look up, if you look at the term within one data set, you can get. 
 25:33: References to related entries in the other data set. 
 25:41: So OK, so, yeah. 
 25:46: Thanks a lot. 
 25:47: may I know like, Yeah, yeah, Right, so it's AWS it's on, and the front end, and, Obviously, the, you know, working with LMs and natural language processing. 
 26:17: Oh, OK, OK, OK, sounds good. 
 26:22: yeah, I'm, I'm, I'm ready to, good to go, OK, may I know like from here, like what is going to be the next process from here? 
 26:35: I will, we'll, send you an email getting back to you about. 
 26:41: this will be the final interview, so, we'll send you an email, with the next steps, shortly. 
 26:55: Thanks very much. 
 26:57: OK, thanks, thanks. 
 27:00: Have a good day. 
 27:00: Have a good day. 
 27:01: Have a nice day. 
 27:02: Bye-bye. 
