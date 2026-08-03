0:03: Hello. 
 0:09: Hello. 
 0:13: hi, good afternoon. 
 0:22: It's OK. 
 1:22: OK, let's, let's start. 
 1:25: Yeah, sure. 
 1:47: Yeah, well, so one year, I'm part of the digital consulting team at Itech, group within consultant. 
 1:58: So for today's interview, right, and we'll start with the introductions. 
 2:02: Then we'll do some coding exercise. 
 2:05: Yeah, sure, OK, OK. 
 2:07: So Mala, I see I have your resume and went through it quickly. 
 2:11: So so right now you're at Nova Health, yeah, yeah, is that correct? 
 2:15: Yeah, OK. 
 2:18: And before that, the truest, lowest, yeah. 
 2:22: OK, I like, so, and what about education? 
 2:30: one second where is it? 
 2:31: Yeah, I like done bachelor's of Engineering Computer Science. 
 2:35: OK, where, where from? 
 2:38: MIT. 
 2:43: And where is this? 
 2:44: it's in India. 
 2:47: Oh, OK. 
 2:49: Yeah, you may want to put that in the bracket because there are multiple institutions called MIT so it's not clear where from. 
 3:01: And it will, it will. 
 3:04: You understand me OK. 
 3:07: OK. 
 3:10: Like, basically it's an Indo, like India. 
 3:14: And so, so when you say, you know, formality in, in brackets, you should say in the India because someone else may be a different institution. 
 3:26: And basically it's a stands for like Malwafields of Technology. 
 3:31: Oh, I think you can write the full name and, but still I would say just, you know, add the, especially because you, this is like when you are in West India is like a foreign country, right, so you shouldn't expect people to know MIT you what it is, where is it, so. 
 3:52: Yeah, so let's start with your experiences and then we'll probably, you know, do a coding exercise first and then we'll follow up. 
 3:59: So let, let, let's start with your latest. 
 4:03: What is your responsibility? 
 4:04: What is your day to day job? 
 4:06: OK, so what kind of development are you doing? 
 4:09: What kind of project is it? 
 4:10: Mhm. 
 4:11: currently, like, I'm working as a lead Python developer at no one's else, like, generally where I'm building the clinical analytics and the AI powered, PI platform on the Microsoft Azure and like my primary responsibilities include like. 
 4:25: Or designing and developing the fast GPI, microservices, building the secure S APIs, processing healthcare data from sources like CSV, Excel, HL 7, FHIR, and like storing the transform data in post SQL and using SQL alchemy. 
 4:45: apart from that, I also work with, extensively on the database design, query optimization, indexing, and like this schema management using alembic and for like long running operations such as like file imports and, report generations I like developed as synchronous background processing services, with retryal logic and item potencies to ensure the reliable executions and productions and. 
 5:10: From a like a deployment perspective, like our applications are, canonized like with the Docker deployed on the Azure human services, like delivered through the Azure DevOps, CICD pipelines and, like along with the development like I'm actively involved in the production. 
 5:28: Support, performance tuning, debugging code reviews, and, colla collaborating with different front-end developers and product owners to define like, AP contracts and, design the scalable solutions. 
 5:40: And before no one that I worked with organization like to LE so where, where, where like I gained the deve strong experience in path and backend development interest APIs, relational databases and cloud-based applications. 
 5:54: So that's a pretty much about me. 
 5:57: OK. 
 6:00: So let's do this, right? 
 6:01: do you have access to any online? 
 6:04: Python editor, if you don't, then I can recommend something. 
 6:08: Yeah, yeah, I have, I have. 
 6:15: should I share my screen? 
 6:17: Yeah, please, yeah. 
 6:40: Yeah, even the first one is OK. 
 6:44: But let me see which one. 
 6:46: Which one that do people use one compiler.com I think this this is what this should be. 
 6:56: I think this is OK. 
 6:57: I also use it previously. 
 7:00: Look, So, we'll do a coding exercise depending upon the time we will do. 
 7:06: Mhm. 
 7:06: What's that thing. 
 7:08: Oh, I think. 
 7:20: I use that one compiler.com, I think that that one. 
 7:24: When I saw someone use it, it was good. 
 7:36: Just save one come by living one word. 
 7:42: You No, that's OK. 
 7:47: That's, it's Yeah, is that fine? 
 7:51: Yeah. 
 7:54: it had those, you know, autocomplete and other things. 
 8:12: Oh, it's loading. 
 8:13: It's taking too much time. 
 8:14: Should I open other one? 
 8:17: That's right. 
 8:18: I mean, anyone who doesn't have a hand for the virus and all these things. 
 8:24: I just opened the first one which I should have done. 
 8:40: Yeah. 
 8:50: OK, so what we are doing here, right, is creating a synthetic data set first, and once that is done, then we'll do some coding, some, you know, analysis of that data set, right? 
 9:03: So it's a totally random data set, right? 
 9:05: Nothing, It doesn't have to be repeatable so it doesn't mean that you know if you run it again it could result in a totally different data set so it's perfectly fine, It's, so, so let me tell you, right, what it is, right? 
 9:23: So it's a clinical data set, right? 
 9:25: So let's suppose there is a clinic, right, like you have Max in India or something, right, and there are different locations throughout the country, and there are patients, right, and they visit these clinics, or they could visit in Delhi, they could visit in Mumbai, and so, and there is a date associated, right, on which date they visited, right. 
 9:46: So let's suppose there are. 
 9:48: 1000 patients, right? 
 9:50: And then you're visiting. 
 9:53: These max clinics at different locations, since let's say January 1st, 2026, right, so seven months they have visited one or more clinics on a certain date, right, so we want to create, create this kind of a data set. 
 10:11: Got it. 
 10:18: Yeah, I see the, I don't see the editor actually, yeah. 
 10:22: Yeah, no, it's. 
 12:08: Firstly, I'm importing conducts like to create a manipulate the data set and as a data frame and like random to generate random patient IDs, locations and visit dates, OK. 
 12:20: Mhm. 
 12:21: OK. 
 12:38: And basically this, this list contains all the clinic locations. 
 12:42: later, like I will randomly assign like one of these locations at every patient visit. 
 12:51: OK. 
 14:01: And now I'm defining like the start and end dates like for the data sets like every patient visits the for for like within the this date range. 
 14:13: Mhm. 
 15:07: like, this is the empty list. 
 15:09: Like I will store like every generated patient visit as a dictionary inside this list and later like, I will convert this into like, into a data frame. 
 15:48: I'm reading through all the 1000 patients and assuming like each patient's, a patient a unique ID. 
 15:57: Mhm, mhm. 
 17:23: He, like, I first calculate the total numbers of days between the start and the end dates. 
 17:29: then I randomly select, one of those days and add it to the start date. 
 17:33: So normally these insurances, every, every, visit date falls, within the required range. 
 17:42: Mhm Yeah, like for every visit, I create a dictionary, containing the patient ID and, randomly, selected clinic location and the visit date. 
 19:41: Then I like append it to the record list and after that, like, I convert the list of dictionaries into the pandas data frame like which makes it easy to perform filtering aggregations and analysis. 
 19:56: Mhm. 
 19:56: Mhm. 
 20:13: like printing the first few to verify that the data set has been generated correctly. 
 21:57: Yeah, it's basically I first, I define the number of patients, clinic locations, and the valid date range. 
 22:03: Then for like each patient, like I ran I randomly generated the, like between 1 or 5 visits and like for each visit, I selected a random clinic locations and the random random date like, within the specified range and like. 
 22:18: stored each, visit as a dictionary in a list and like finally converted that into the pandas data frame for analysis of these basically this is approach is simple, efficient and scalable for like generating the synthetic, synthetic, data sets. 
 22:38: Hello? 
 22:41: Yeah, so total cost is 3030, right, yeah. 
 22:46: OK. 
 22:51: Patient ID clinic location. 
 22:55: OK, so you don't have name, right? 
 22:56: What patient name. 
 23:08: How would you add names so that each ID is like a, a unique name. 
 23:13: Oh, see, like, generally for adding the, unique, names, like, like, right now I'm only generating unique patient IDs like to make the data set more realistic. 
 23:26: I would like create the patient name once and maintain, mapping between the patient ID and the patient name, like, then like whenever the same patient has multiple visits, I would reuse the same name instead of like generating the new one. 
 23:55: OK, so now that we have this, right. 
 23:58: Now I want to do a very simple manipulation. 
 24:02: I want to print the, so these locations are there, right? 
 24:06: You have Texas, Mumbai, Delhi. 
 24:09: So for each location, I want to print how many unique visitors of patients were there, you know, each month. 
 24:17: So January. 
 24:19: You know how many unique visitors were there for each location? 
 24:23: February, like how many unique visitors were there? 
 24:27: OK. 
 24:29: So for 7 months and And for each month, you have to print. 
 24:37: How many visitors that, since like each patient can like visit multiple times in a month, so we need to count only unique patients. 
 24:49: first, like I will extract the month from the visit date, then group the data by like clinic locations and month, and finally count the unique patient ID ID using the N unique function. 
 25:04: and unique method, should I write the code? 
 25:09: Yeah, it is, yeah. 
 26:18: Like first I convert the visit date column like to a date time, data type. 
 26:22: So this allows me to use Panda's data, date function like accepting the month year already. 
 26:33: after that I create a new column for like month by like expecting the month name from the visit date and using percentage bill returns like the full month name such as like January, February or March. 
 28:06: Like here I'm grouping the data by month and clinic location because the requirement is to find the number of unique patterns like for each clinic and every month. 
 28:24: After grouping, I select the patient ID column because that, that's the field like I want to, I want to count. 
 29:38: I can use any unique method instead of count because the requirement is to count like unique patients. 
 29:46: So if the same patient visits the same clinic multiple times in a month, they should like only be the counted once. 
 31:43: Group by basically runs a group project like with a hierarchical index converts like back into the normal data frame. 
 33:13: Yeah, that's fine. 
 33:15: basically, first I convert the visit date into the date time so that I can work with the date function. 
 33:23: Then I expect the month from the visit date, into a new column, OK? 
 33:27: And, next, I group the data like by a month and the clinic location because the requirement is, to calculate the number of, unique, patient for like each clinic every month and. 
 33:37: and last, like, finally, I use a unique method on the patient ID, to count the distinct patients, like, reset, the index to get the clean data print and print the result. 
 33:50: Mhm. 
 33:55: I think we're done with this exercise, Will you be able to write in this, you know, this editor or new editorial. 
 34:03: A very basic fast API, you know, endpoint. 
 34:07: Just give me one or two examples, right? 
 34:10: So let's suppose this is what you have built, right? 
 34:13: So this data set that you're creating here, let's suppose that was the response to a request from the client. 
 34:21: The client leaves a web front end, right, makes a request, to the back end. 
 34:27: And in your fast API you have to expose this particular data set that you just created and give it to the client and it will display in a table. 
 34:37: You understand what I'm saying. 
 34:38: You go to the dashboard. 
 34:40: The dashboard is calling your fastest pay point, and you're returning this particular table that you have just printed. 
 34:47: Got it. 
 34:47: Got it. 
 34:50: should I use, this compiler or, other one? 
 34:55: OK, I mean, whatever, whatever works best for you. 
 35:59: Like first I create the first DP application, instance. 
 36:02: This is the entry point for like defending the rest APIs. 
 36:26: And basically this defines get endpoint name like patient like whenever the front end call this endpoint fast I will execute the functions below it. 
 38:11: basically, this online compiler does not have the fast GPI, library installed, so it cannot execute the work, Yeah, just write, should I just write the code for like the basic implementation of the code, yeah. 
 38:42: like, also I'm, assuming that the data frame like we generated in the, like previous exercise like already exist, OK? 
 38:53: Mhm, you know. 
 39:12: and this, like, basically says, the data comes from the pandas data FM, and in the real world application the endpoint like, would fetch the data from the database, such as post SQ or using SQ alchemy, and also apply any required filters or paging nation and then return the result as a like adjacent to the end. 
 39:37: Mhm It's done, basically it's done. 
 39:50: So I think I'm good. 
 39:51: I just wanted to see your hands on coding and what kind of code you write, what kind of design content, and everything else. 
 39:58: So it looks good so far. 
 40:00: So the next step then, I'll provide my feedback at some point, you know. 
 40:04: So it's Friday, so. 
 40:06: But I'm hoping by Monday someone will connect with you and guide you to the next steps, provide you feedback and so on. 
 40:14: like, apart from this one, is there any other one for this, like any technical, I think 2 technicals. 
 40:22: This is your 2nd, I believe, right? 
 40:23: Yeah, yeah. 
 40:25: So normally it is too technical terms. 
 40:27: So that's, I think the other two, and I will tell you the next steps. 
 40:35: OK. 
 40:35: Yeah, sure. 
 40:37: Thanks. 
 40:38: Thank you. 
 40:38: Have a good weekend. 
 40:39: Bye-bye. 
