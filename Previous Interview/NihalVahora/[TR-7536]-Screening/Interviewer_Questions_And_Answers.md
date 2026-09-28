0:00: Good. 
 0:01: Hey, hi, good afternoon. 
 0:03: How are you? 
 0:03: Yeah, I'm good. 
 0:04: I'm good. 
 0:04: How's your day going? 
 0:07: It's going good so far. 
 0:10: So the son may be joining the the maid, OK, he just joined. 
 0:22: Hey. 
 0:22: Good afternoon. 
 0:24: Hi, good afternoon. 
 0:26: So, how are you doing? 
 0:29: Yeah, I'm good. 
 0:30: How about you? 
 0:31: Yeah, I'm good too. 
 0:32: Thanks for asking. 
 0:37: Yeah, they come from. 
 0:41: The So, anyhow, I am just checking your CV and it's also good actually, have good experiences and, a good technical background as well, but we share that one. 
 1:05: So how about your recent projects? 
 1:08: So what exactly you guys are doing on the technical side and, how are the things? 
 1:14: So, yeah, like recently, I was working with Cowell Health Lifeline Hospitals and like in my recent role, like my, I'm responsible for developing and maintaining Python-based banking services and also rest APIs using fast API and Flask. 
 1:30: And like in this like I can say we, we have a significant data like I have also data, significant data engineering component like since we deal with large volumes of healthcare data, so I use P Spark and Apache Spark for the distributed processing. 
 1:45: Like we do things like data cleansing, transforming, validation, and also the standard digestion because like data coming from different sources, sources in our system. 
 1:56: And like on the cloud and deployment side like using the AWAs Docker and also Quinnates like we can generalize our Python services using the Docker and deploy them to the Quates like I'm also involved in the troubleshooting things like failed ports and application errors. 
 2:17: So yeah, like and also like I use CIC practices for building. 
 2:21: And testing and also like deploying our services and recently like I have been using cloud as an AI assisted development tool for understanding the existing code, generating case scenarios, troubleshooting, and also for writing the unit test cases. 
 2:36: So yeah, but I always validate the generated output through like testing and normal code reviews and security processes. 
 2:43: So yeah, that's my recent experience with Corwell Health. 
 2:47: Got it, got it. 
 2:48: Yeah, yeah, that's all good to know. 
 2:51: so in the Python, you have a good experience, right? 
 2:54: So, what could be the main differences between threading and the multi-crossing in a Python? 
 3:02: OK, got it. 
 3:03: So, the main difference between threading and like, it, basically depends on like the handle, how they handle the education. 
 3:12: So, basically, like, with the thread, with the threading, like multiple threads done within the same process and share like the same memory space. 
 3:21: Like in Python, like because the, because of the GIL I can say like shredding is generally more useful for input output bound work, like calling the APIs, reading from the databases, or also like, waiting for network responses. 
 3:37: While like one thread is waiting for an input output, another thread is waiting for like that can continue working. 
 3:44: So yeah, and also like multi-processing. 
 3:47: So like multi-processing on the other hand, creates like separate processes and each process has like its own memory, own memory space and like Python interpreter. 
 3:57: So that makes it, I can say like useful for CQU intensive task like because that can actually execute CPQU work in parallel across the multiple CPU cores. 
 4:07: So yeah, this is the main difference. 
 4:10: Got it. 
 4:10: Got it. 
 4:12: suppose in the Python now, right, I have an AWS, screen. 
 4:17: in the meantime, give me one second, Santos, can you give us the screen frame, please? 
 4:22: Screen, sure. 
 4:24: Yeah, they have, in the meantime, so I have, AWSSC budget, OK, and, my team is asking me to upload some of the files, and they want me to create one, automation file for that in the Python. 
 4:40: So how and what the independencies I need and how we can, and I in the cold. 
 4:49: OK, OK. 
 4:51: So, like we have the 3 and we have to retri the code. 
 4:54: OK. 
 4:55: So for this like uploading files from a Python application to an AWS S3 bucket, like I would typically use the AWS SDK for Python which is like Boto 3. 
 5:06: So, the main dependency I need is the Boto 3. 
 5:10: Like I would install it with the PIP install Bodo 3 and like then I would configure and like. 
 5:18: if I can say like if the requirement is to read files from the S3, I can use like I already told the Boto 3 I will use, like I will connect to a bucket list, like list objects or download a specific file or read the object directly into the memory. 
 5:34: And like in our project like a similar pattern can be used when like healthcare data files are like received in the cloud storage and need to be picked by a Python data processing pipeline. 
 5:46: And from there like. 
 5:48: The application can validate the file processes and like it like process using the Python or PySpark depending on the size and then it would either store the transform data back into the stream or pass it to the downstream applications and also for the security like for security I wouldn't hard put the AWS access these into the Python code. 
 6:09: So yeah. 
 6:12: OK, OK, do you mind, can you check on the screen, the, I can. 
 6:19: Yeah, see the complete screen and stuff or just something, yeah. 
 6:33: OK, you can open any online Python or something. 
 6:47: OK. 
 6:49: So, let me write, let me give you one simple thing, OK. 
 7:08: Well, is, is a little bit slow. 
 7:11: Is there any other others that, it is keep on loading. 
 7:15: It won't, it won't even talk to you. 
 7:20: OK. 
 7:23: I'm trying to take the go back to this place. 
 7:25: Maybe on Netflix. 
 7:30: OK. 
 7:34: No, the, the site itself is won't open. 
 7:37: Can you go back? 
 7:39: yeah, all right, another one. 
 7:43: I like. 
 7:45: The second one, yeah, this is much, much better. 
 7:47: No, yeah, OK, yeah. 
 7:50: Yeah, this is much, much better this this won't upload any. 
 7:58: Anything, so I'm, I'm just typing you something. 
 8:02: don't read this. 
 8:04: by the way, this is, is this meeting is a recording, I don't know. 
 8:09: No, I'm not recording this meeting. 
 8:14: no, no question. 
 8:15: OK, OK, OK, got it, got it. 
 8:19: so let me. 
 8:22: Send you this, so please don't read this out, OK? 
 8:25: you can copy and I think that what I have is copied here, you can copy and paste it somewhere. 
 8:38: Whatever you understood, right, you can, write a code for this. 
 9:04: OK, so I have to write the repeated values. 
 9:08: And if they are not repeated, I don't have to pin them. 
 9:18: The frequency view for storing the. 
 11:22: Oh yeah. 
 11:25: Where is the output. 
 11:31: So basically, Can you see it? 
 11:36: Yeah, yeah, I think, 6, it is showing up 3 times, right? 
 11:45: 66 is 3 times. 
 11:47: OK, OK, OK. 
 11:50: OK, yeah, you know, yeah, yeah, you can keep it, safe, and, in the meantime, right, so, suppose I have a few that this, application is, running as of now, but all of a sudden, some of the parts are delayed and then. 
 12:10: if I delete it, it is creating a new part and it is working fine, but after some time again it is also deleting, so what might be the issue. 
 12:24: OK, so the issue I can think is like, basically, if a Kubernes like pot keep dying and like deleting the pot temporarily fixes it, but the replacement pod like eventually dies again, I can say like I would, I would treat that as a symptom rather than like the actual problem. 
 12:42: Like Kubernes is like recreating the pod because the deployment or replica state wants to like maintain the desired number of replicas. 
 12:51: And the first thing like I would do is to check the pod status and events like with tube CTL like get pods or like pod and like here the described pod will like actually tell me about the status of the like the current Kuberne pod and like it is important like because it can tell me whether the pod is being filled because of like health pro or resource issue likes doing problem or like something else. 
 13:21: And then if the container has like already restarted, like I would also check the previous container instance with the two detail logs or like by giving the pod name and like these are like several common possibilities that I could use like if I see like OOMK or like that usually means the container exceeds its memory limit. 
 13:44: And in that case, like I would also check the port CPU and memory request and limits also, and I'll also look at the actual resource consumption. 
 13:52: And if I like another thing I would like, I would can check is like failing, failing the probe like Litus probe, for example, like, if the application is running but the litmus and quant is continuously failing or taking too long to respond. 
 14:09: So, but is it a liveness or is it a readiness? 
 14:13: well, can you come again? 
 14:15: Is it aliveness or is it a readiness. 
 14:20: OK, OK, OK. 
 14:22: So, OK, but, readiness won't impact anything there. 
 14:28: readiness, like, readiness won't impact in the like status. 
 14:36: Like, see, readiness by itself normally doesn't restart or kill the pod. 
 14:40: Like if the readiness probe fails, tubernates like considered the pod not ready to receive the traffic. 
 14:48: So it removes that pod from the server service endpoints, and that container can continue running. 
 14:55: Got it. 
 14:55: Got it. 
 14:56: So, so how come, we, is there any chance of, services down if this is the case? 
 15:06: if service is like down, like, I can say like, yes, there is a possibility of the service becoming unavailable, but it depends on like how many like healthy replicas you have. 
 15:17: Like for example, suppose I have 3 ports behind the Kuberne services like, is, will the pot again will like it. 
 15:28: Like if the service is down, the pod will, like, basically, it will not recreated just because of readiness probe failure. 
 15:36: Like if the readiness probe fail fails, the pod stays running, like Kubernes makes it not ready, and the pod is removed from the service endpoint, so it stops receiving the traffic. 
 15:49: OK, and, in Cuban it is itself, right, I have, my monitoring tool is the keep on saying that one pod is not available, but actually when I go to this, cubo is cluster, the pod is up and running, OK. 
 16:12: OK, what might be the issue if that is the case? 
 16:16: OK, if that is the case, like, as I can, like that can definitely happen, like a pod can be like running but still not be available to receive traffic. 
 16:27: So like I would first check the difference between like the pod's running status and its ready condition. 
 16:32: For example, like I would run the two CTL g pods, and if I see something like, the pod stats like name already or running, the status. 
 16:42: So that means the container is like running but the pod is not ready. 
 16:46: Then I would check the Troops CT, I can say describe pod. 
 16:50: So I would specifically like not, I, I would specifically look at the conditions and the events sections to see like why the readiness probe is failing. 
 16:59: Like I would also check the troop retail get endpoints depending on the Kuberness version, like, and that, that tells me like where, whether the pod is actually registered as a healthy endpoint or like behind the service. 
 17:13: And another thing like, another thing like I would check is the readiness probe like itself. 
 17:20: For example, like if the application exposed get help or like the endpoint. 
 17:24: So but that endpoint is returning 500 timing out or I can say taking too long. 
 17:30: So Kernes can like keep the poll in running straight while making it not ready. 
 17:35: And and last like I would also check, like I would also check the monitoring tools configuration. 
 17:41: Sometimes the monitoring system is checking out different metrics or like I can say name space services or endpoint. 
 17:49: So my, I can say like my troubleshooting flow would be like for if the pod is first port is running, then check ready column, then check the readiness for, then check the QCTL endpoints and I, I can, and then check application health endpoint and then check the monitoring configurations. 
 18:09: So yeah. 
 18:10: OK, OK, yeah, nehal, I'm good here actually, I'm good with this call, Santos will, let you know for the next person down, OK, so. 
 18:25: Yeah, so he, he will be ready for the next steps. 
 18:28: OK. 
 18:29: Yeah, awesome, man. 
 18:31: Thank you. 
 18:32: Thank you so much. 
 18:33: Have a great weekend bye you too bye bye. 
