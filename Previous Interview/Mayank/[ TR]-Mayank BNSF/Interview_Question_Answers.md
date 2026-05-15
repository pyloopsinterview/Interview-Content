(Transcribed by TurboScribe. Go Unlimited to remove this message.)

Awesome, so let's get started. My name is Kishore, working as a Principal Engineer for Asset Platform. I joined BNSF like 5 months ago, and I'm developing a platform for different types of assets at BNSF.

That manages the state, health, telemetry, what not, everything related to that. Prior to BNSF, I worked for Amazon for about a decade. I have an experience working for Target and Walmart too.

That's a bit about myself. My name is Mike Patel. I have around 13 years of experience working mainly as a Python Backend and Cloud Engineer.

With strong experience in distributed systems, AWS Cloud APIs, microservices, platform engineering. Currently, I'm working with Prudential Financial as a Lead AM and Python Cloud Engineer. My current work is generally focused on building scalable backend platforms and the distributed systems.

That supports high volume enterprise workflows. Most of the recent work has been around the large-scale claim processing platform. Earlier, claims were coming from different sources and formats.

Many processes were manual. The business was facing delays and inconsistencies. I led the backend architecture and development of a Python-based distributed platform that automated the entire workflow.

We designed the system using the microservices and agent-style processing. The independent services handled tasks like document classification, data extraction, validation, enrichment, and routing. All services were containerised using Docker and deployed on the Kubernetes in AWS.

I was also heavily involved in backend engineering, cloud infrastructure, CI-CD pipelines. We focus on a lot of fault tolerance. We also integrate LLM and AI capabilities into the platform using the API and also the RAG approach.

That's pretty much about it. From what I understand, this is basically a rate-limiting or fraud prevention problem for a flash open system. The requirement is that whenever a user clicks on a claim, we need to check how many successful claims the user has made within the last 60 seconds.

If the user had made fewer than 5 successful claims in the last 60 seconds, we allow the request and record the timestamp. Otherwise, we block the request and return false. For this kind of problem, I would probably use a sliding window approach using a queue or a dequeue.

Because we only care about the timestamp within the last 60 seconds. The overall time complexity would be efficient since we continuously remove expired timestamps and keep only valid entries in memory. Sure. 

That sounds reasonable to me. If you could just write some code, I would like to see if you can write some code. Yeah, sure. 

I'll write the code. I've selected Python. If you prefer any other language, please feel free to.

No, no. In Python, I have this. Yeah, good.

Should I explain this? Yeah. First, I'm importing the dequeue from collections. Because it allows efficient insertion and removal from both ends in full time complexity.

And I'm also importing the time to capture the current timestamp for each coupon claim. And after that, this dequeue will store timestamps of successful coupon claims. And only successful claims are stored.

And also, we have the 10, 20, 30, 40. These represent claims times. And also, the claim coupon function. 

These functions get called every time a user clicks on the claim button. And then we have now equals to time.times. So, these capture the current timestamp in the seconds. And the while claims and now.

So, here, I'm removing all the timestamps older than the 60 seconds. Because they are no longer part of the active sliding window. So, these are the most important parts.

And after that, also after the cleanup, if fewer than 5 successful claims exist in the last 60 seconds, we allow the new request. And after that, returning true means the coupon claim is allowed. So, if already 5 successful claims exist within the last 60 seconds, I block the request and return the false.

You are removing the claims here. And then you are adding new. Yeah, you could optimise a little bit as well, right? For optimising, what we do also.

You know, it's a month of optimising. But this is already mostly optimised. But what you could do is.

Firstly, I also remove the expired timestamp. Then I check whether the new claim can be added within the current 60 second window. And yes, this can be optimised for them depending on the scale and the traffic pattern.

Yeah, you could remove all the expired and then add. That way, there is nothing eligible or nothing, you know. Anyway, I think this is.

And how would you scale if we say that this is per user? Actually, I think it says it has to be per user. For say, per user. Exactly, since the limit is per user, we need separate tracking for each user instead of one global DQ.

So, instead of claims equals to DQ, I would maintain something like. From collections, import defaultdict to DQ. And user claims equals to.

You can import the defaultdict and pass the DQ. So, then each user gets their own sliding window queue. Can you update the code for that? Yeah, sure.

So, are you typing something? I'm not able to see here. Firstly, I go through the code and go through the logic first, then after. Okay, so you're typing now.

As per this code, since the requirement is per user, I'm maintaining the separate DQ for each user using the defaultdict. So, each DQ stores timestamp of successful coupon claims for that specific user. So, whenever a new claim request comes, I fetch that user claim history.

I remove all the expired timestamp older than 60 seconds. Then I check how many successful claims remain within the current sliding window. And if fewer than 5 claims request, I allow the request append and the current timestamp I return true.

Otherwise, I block the request and return false. Okay, that's fine. Let's say our system or our business scaled up really well.

People are interested now. So, how would I scale the system? So, let's say I scale my business. Now, instead of running this in one single server, I need to now run it in some sort of a multi-node Kubernetes maybe.

So, how would this work? If not, how would you modify this code for that? Absolutely. If the business scales and traffic increases significantly, then the current in-memory solution would start having limitations. Right now, the implementation works well for the single application instance because all claim data is stored locally in memory.

But once we move to the multiple servers or containers behind a load balancer, requests from the same user could hit different instances. And each instance would have incomplete claim history. So, to scale this properly, I would move the rate-limiting state to a centralised distributed store like Redis.

So, the architecture would look something like we have multiple application servers, shared Redis clusters, and also each user's claim timestamp is stored centrally. So, Redis is a good fit because it's very fast in memory operations, atomic operations, and also we have native expiration support and very high throughput. So, instead of storing data in local BQs, I would probably use Redis shorted sets or the sliding window like counters with TTL.

Okay, sounds good. But what if the user plays with our system, executes a bunch of requests in parallel? And how would you protect your system from that kind of attack? What about that? So, how would you protect your system, right? Now that your system is distributed, right? How would you make sure that parallel requests coming from the same, probably they may come from different regions or I don't know what it is, but if they come from the same user, probably almost at the same time, what would you consider? Firstly, I'd make sure the rate limit check is atomic across the distributed system. Because once the application is running across multiple kubernetes ports, parallel requests from the same users can hit the different ports at the exact same time.

So, if every port independently checks and updates the count, these conditions can happen. So, instead of like read count and then update count, I'd like move the whole operations into Redis as a single atomic operations. So, a common approach is like using a Redis Lua script or like atomic shorted set operations.

So, the script would like, generally, we can say remove expired timestamps, count current valid request and if count is below limit, insert the new timestamp. And after that, like return allow or block the response. So, since like Redis executes Lua scripts automatically, like atomically, so like no two requests can modify the same user's rate limited window simultaneously.

So, like even if 50 parallel requests arrives together, like from the same user across the different ports, like only they allow number success consistently. Then you can add the final line interface like that with the applications layers, state layers, like while Redis becomes the single source of truth. Yep. 

Okay. Sounds good. Okay. 

I think I got the answers for this. Let's move on to the design question. Give me one second. 

Let me just quickly do this. You can share something. Yeah. 

Give me one second. I'm pasting another link in the chat. You want to see now? Yeah.

So, this is a system design question. You don't need to code. Can I please see here? Yeah.

Sorry? Yeah. Okay. Could you run me through your thought process here? Yeah, sure. 

So, like basically like what I do, like generally overall like we can say like firstly we have like sensors, then we have like edge devices inside the train, then we have the local ML or the rule engine, and then we have like I've like done the immediate safety things. And basically the step four, we have like totally some steps, like since this is like the safety critical systems, like my first priority would be reliability and early detections, rather than only we can say prediction accuracy. So, like I probably like designed this monitoring and alerting systems.

So, firstly, as I say, like it's a data collection first, like I first place sensors like near the train wheels. And depending on engineering requirements, like we could use vibration sensors, acoustic sensors, temperature sensors, also the ultrasonic crack detection. So, these sensors like continuously generate elementary data like while the train is moving.

Then after that, step two is like edge processing, like I would not directly send all raw data to the cloud, because trains generate huge volumes of like real time data and latency, like it's like important here. So, like I need to do edge computing here, like inside the edge device would be like collect sensor streams, pre-processes data, filter noise. And after that, we have the crack detection logic.

For crack detection, there are like two possible approaches, like one is like the rule-based threshold, and the second is like ML-based anomaly detection. And like, then after we have the safety action, like if the confidence crosses the critical threshold, the edge system should immediately trigger a safety workflow. And then, yeah, so this is like the high-level diagram, like which I like to explain to you.

And we have like after that cloud architectures and reliability decision. So, overall, like I treat this as like the distributed... How would you notify so that the traffic train can stop? How would you? How would you notify someone, like is there some sort of a notification system that lets you, you know, send something to someone so that they can stop the trains? Okay, for like notifying, like I like design a multi-lane notification and also the alerting system, because this is like the safety critical use cases. So, like there are like actually two categories of notification.

They are like immediate operational alerts and monitoring and maintenance alerts. So, then continue for like immediate alerts. The like edge systems inside the train should directly communicate with the driver control panel, onboard safety systems, and the like the railway control centre.

That communication should be real-time and load at its ease. And like also like from like backend side, like I probably use the event-driven notification systems. For example, like sensor event, we use Kafka, SMS or Event Bus.

And alert service consumes the event notification services like SMS, email, push alerts. And also we have like the dashboard alerts. Then mention the reliability, like for critical alerts, like I'd also add the retry mechanism and escalations policies.

And then, yeah. And all the AWS services like SNS, EventBridge, Lambda. So, individuals can monitor.

I understand. Okay. I got the thought process.

Could you just go ahead and finish this off? Yeah, sure. Is it edge device inside the train? Oh, sorry. You mentioned the second box to be edge device inside the train.

Yeah, yeah. So, the ML is running inside the train? Yeah. Most probably, we can say.

So, where are these sensors installed? Yeah, like, yes, like exactly. Like my thought process is that the ML or anomaly detection engine should primarily run on the edge device inside the train, like instead of depending completely on the cloud. So, the main reason is like low latency and the safety reliability.

That I understand, but just trying to understand. So, the wheels, how can a train check the wheels? Is it efficient for a train to check its own wheels because there will be hundreds of such wheels? Like the train is not really looking at the wheels like a human.

(This file is longer than 30 minutes. Go Unlimited at https://turboscribe.ai/ to transcribe files up to 10 hours long.)