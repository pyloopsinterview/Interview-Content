# AWS Screening Interview Conversation

**Participants:**

- **Interviewer (Marvin)**
- **Candidate (Vineet)**
- **Recruiter (Suman)**

---

### Introduction

**Marvin:**  
Hey, hey, I'm Marvin.

**Suman:**  
Hi, Vineet.

**Vineet:**  
Hi, Suman. Hi, Marvin.

**Marvin:**  
How are you guys doing now? Everything good?

**Vineet:**  
Yep. I'm doing well, thanks.

---

### Screening Call Introduction

**Marvin:**  
Okay. So few things I'd like to say right before I start any of the screening calls.  
The first thing is, this is a _screening call_.

If we feel that you're the right candidate, then we'll put you in front of the customer.  
Let's make this interactive — if you have any questions, we can clear your doubts and ensure that you have everything you need and I understand your skill set.

**Vineet:**  
Sure, sounds good.

**Marvin:**  
Okay. The other thing I would like to say is this is an **AWS role**.  
There is no GCP, no Azure, no OnPrem — it’s all AWS.

And the focus is **Infrastructure as Code**, okay?

**Vineet:**  
Yeah, sure. Just wanted to check — in the JD I saw something about PowerShell along with Microsoft 365, Entra IDs, Graph APIs, etc. Is that part of AWS tools?

**Marvin:**  
Good question. That’s actually the very last thing — maybe 70-80% of the time you’ll be working with AWS tools like CloudFormation, SSM Documents, Config Rules, Step Functions, etc.  
So the major part of the role starts with **CloudFormation**.  
Without CloudFormation, we cannot proceed. So let’s start there.

---

### CloudFormation Discussion

**Marvin:**  
Have you worked on CloudFormation?

**Vineet:**  
Yes, I have opened CloudFormation.

**Marvin:**  
Okay. So when you open up a CloudFormation template, what categories do you see?

**Vineet:**  
Uh, so there is a version, the format version, description, metadata, parameters, mappings, conditions... and of course, resources.

**Marvin:**  
Perfect. The **resources** section is the most important one — that’s mandatory.

---

### Parameters Section

**Marvin:**  
What is the purpose of having the _parameters_ section?

**Vineet:**  
Parameters basically define values that change between environments — like instance type or VPC IDs. They help make templates reusable and dynamic.

**Marvin:**  
Good. And how do you call that within the template?

**Vineet:**  
Inside sections like _Resources_, _Conditions_, or _Outputs_, we can reference parameters using the `Ref` function.

**Marvin:**  
Excellent. For example?

**Vineet:**  
In a resource definition — say an EC2 instance — I can refer to the parameter in the `Properties` section using `Ref`.

**Marvin:**  
Correct.

---

### Referencing Other Resources

**Marvin:**  
Now let’s say I created a Role in the same CFT and want to use its ARN elsewhere — how would you call that?

**Vineet:**  
I can use `GetAtt` to reference its attributes like ARN.

**Marvin:**  
Correct — `Fn::GetAtt`.

---

### Using Secrets Manager

**Marvin:**  
Now, let’s say I want to call the **Secrets Manager** in a CloudFormation template.  
How would you do that?

**Vineet:**  
I can reference the secret ARN or use a function to resolve it… maybe `GetAtt`?

**Marvin:**  
Not exactly — you use the **`resolve`** function to fetch secrets dynamically.

---

### Exporting and Importing Outputs

**Marvin:**  
Let’s say I want to use the output of this stack in another stack. How do you do that?

**Vineet:**  
We can use **Exports** — export a value in the first stack and then import it in the second stack using the `Fn::ImportValue` function.

**Marvin:**  
Correct. And under which section do you export?

**Vineet:**  
In the **Outputs** section.

**Marvin:**  
Right.

---

### ECS Cluster Creation

**Marvin:**  
Let’s say you have a CFT that already has VPCs, subnets, and security groups created.  
Now your lead asks you to create an **ECS target cluster** with services and tasks.  
What would you do?

**Vineet:**  
Since infra is already there, I’ll first copy the current stack, add ECS target resources — like a cluster and services — then validate the template.

**Marvin:**  
Okay, but what resources exactly need to be created?

**Vineet:**  
ECS cluster, ECS service...

**Marvin:**  
So actually, you first create **roles**, then **target groups**, **listeners**, **load balancers**, then **cluster**, **services**, **tasks**, and possibly **sidecars**.

**Vineet:**  
Oh, I see. What’s a sidecar?

**Marvin:**  
A sidecar is an additional container running alongside the main task container, often for logging or monitoring.

**Vineet:**  
Got it.

---

### ECS Fargate Auto Scaling

**Marvin:**  
What are your thoughts on **ECS Fargate Auto Scaling**?

**Vineet:**  
We can set up Auto Scaling horizontally based on CPU usage.  
It automatically scales out when utilization exceeds a threshold and scales in when it drops.

**Marvin:**  
Okay, but explain completely — how it’s triggered and where it’s set.

**Vineet:**  
Sure.  
We first set up **CloudWatch Alarms** to trigger scaling actions.  
For example, if average CPU utilization exceeds 70%, ECS can launch more tasks; if it goes below 30%, it scales in.

These thresholds are defined in **CloudWatch alarms** as part of the Auto Scaling configuration in CloudFormation.  
We can use metrics like `ECSServiceAverageCPUUtilization` or `ECSServiceAverageMemoryUtilization` and set the target values accordingly.

**Marvin:**  
Good. That’s better.

---

### Wrap-up

**Marvin:**  
Okay, Vineet, that’s all I had. Do you have any questions for me?

**Vineet:**  
Yes — just wanted to know about the next steps.

**Marvin:**  
I’ll discuss with Suman what the customer needs, and then he will get back to you.

**Vineet:**  
Sure, sounds good.

**Marvin:**  
Thank you, Vineet.

**Vineet:**  
Thank you.

---
