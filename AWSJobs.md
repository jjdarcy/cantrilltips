# What is a Solution Architect and what do they do?
This text was taken from a discussion on the TechStudySlack community. The text is taken "as is":

> @JohnOgdan:
> There are often posts about requirements for “entry level SA” jobs. Would be interested to understand what people think an entry level SA job is?
> 
> To me entry level SA requirement are going to look like:
> * 5 years professional IT, where you've done dev/engineering, had management/team leadership responsibility
> * Be confident leading design, review and requirements gathering workshops with engineers and senior customers, 
> * have done delivery, operations/support, consulting, - including leading the fixing of complex incidents
> * understand something of the sales process, P&L, project management,
> * know a bit about software, infra, security, network, database, monitoring, backup/recovery, scalability, UI, compliance & be an expert in at least one
> * Have done recruitment/interviews & been a line/review manager
> * generally be seen as a leader by engineers/managers (ie when brown stuff hits the skinny thing, people look at you for guidance)
>
> Clearly not everyone will have all of that, but I'd be looking for someone with at least 80%
>
> Why all that stuff? Because the architect is supposed to be the peer of the project manager. The PM owns the money side of the solution, and you own the technical side of it & you can't do that without a broad base of skills
> 
> I'll caveat the above, by adding you will work as per of a team, and as a junior you are likely to own one aspect/stream of the whole. But still: this is not a first job, unless you are an exceptional candidate to have gotten thru an interview for a rare company rich enough to put you through an 18 month dedicated training programme
> 
> The above also being the reason I consistently say don't go for a SA role as fist job. Pick any one bullet above and go do that job first. Learn that, then do another   
> 
> From Adrian   
> - i've actually had a few people me (2 ex students and 1 new one) who are looking to hire SA's as a 1st job ... fully train up. There is a huge demand for it   
> - and people are struggling to find good people   
> - most experienced people, have experience of more legacy sides of IT (which has value).. but there are a ton of project demands which needs more cloud focussed SA's and there are outfits willing to train people up   
> - so im not saying you're wrong  @John Ogden in general, but its not clear cut either (edited)    
> - theres a lot of people who think that an SA role is a senior thing, like people develop in IT, move through support, then ops , then project roles and then become an SA   
> - they are all diff streams   
> - you can start as a junior SA .. and develop within that stream   
> - at least in my experience   
> - i have a few students who've hopped into junior SA roles as their first IT role   
> - and yeah generally this means shadowing a Senior SA for a while.... but it's good development   

> @JohnOgdan: As a a side post to the above - other common question I get via DM “what does an SA do, day to day” hard to say cos every day is different, but here are examples
> * lead a bid response: describe how you would migrate 30 years of legacy (1000 servers and 500 apps) to cloud. Produce a 3 year project plan, and fixed cost proposal that is commercially acceptable
> * Design a new system that speaks to 10 other things and does xyz, ensure it's implemented per design
> * write a design then oversee its implementation to make (system you've never worked on) process messages 10x faster and at 10x the scale
> * Find out why (some system) is (doing something weird) and stop it
> * Write a report describing how our system meets the needs of sp800r53 (Google it, download the spreadsheet, weep)
> * Talk to (random vendor) find out what their thing does, whether we could use it and what it would cost
> * Customer wants a price/delivery estimate for x, produce a 3 year roadmap and costing with ROI
> * Engineers want to do (thing) determine if it's good idea
> * Customer got a massive bill. Work out how to make it cheaper, oversee implementation of any changes
> * Customer wants to replace (some random product eg the database, monitoring tool, cloud provider) with (equivalent product from Gartner magic quadrant) - work out how we could do it, how long, what costs, what payback, oversee its delivery
> * Review project/system/design, produce recommendations for making it better (eg perform a well architected review, listen to concerns from users, devs, support, etc) cost and plan fixes

> @JohnOgdan One more example - let's look at the difference between a real scenario and a pro level question. A pro question will have a 3 line answer and boil down to “use aurora” or something
>
> Real world scenario:
> * you need a database to support (some product) running in AWS
> * The product is only certified on oracle & currently uses data guard over 2 AZs
> * The product is hyper chatty creating 30,000+ transactions per second requirements are zero data loss, so data guard must run max avail (ie commit to 2 AZs before acking the transaction)
> * App uses 2 phase commit and there are triggers
> * App is hugely sensitive to commit latency and will cascade fail if commit latency exceeds 100ms
> * App can't support shards of eventual consistency 
> * Db is running in biggest/fastest ex2 available
> * There is very little time/money to fix this
>
> What do you do - produce detailed cost/benefit, pricing, delivery plans for:
> * rewrite the app to be nicer to the db (support shards, be less sensitive to latency, use eventual consistency)
> * Migrate the lot to OCI and run it on exadata/logic
> * Migrate to on-prem and run it all on BFG10k mainframe
> * rewrite the app to be less chatty (solve cascade failure, live with other problems)
> * Run the db single AZ on instance store to mitigate latency & convince client active data guard works well enough
> * Migrate the app to azure and use the interconnect to run the db in OCI on exadata (+ consider impact of MS and Oracle funding, pissing off AWS, and how many things the app talks to (about 50) also move to azure
>
> Also: how would different context change your recommendation. Eg if the app was certified on MySQL,
> 
> @JohnOgdan Last one / disclaimer: Am absolutely not saying “don't do the AWS architect course”
> 
> Am saying do them to help land *cloud infra engineering* jobs & when you have that job, learn more stuff, do other roles, over 3..7 years, so you can land the SA style jobs with the right experience
> 
> I don't think you can answer challenges like the above without detailed understanding of AWS, applications, databases, and internal politics

# Tips and tricks with getting a JOB in AWS
Information here is gathered from discussions on TechStudyslack. Thanx to John O, Sameer, Adrian (ofc) and many others for contributing. 

Also, read up on the STAR method when you are describing situations you have been involved in: https://interviewsteps.com/blogs/news/amazon-star-method

## Getting a job with your AWS experience
* Length of your CV should be 2 or 3 pages max. Font size 10 minimum. Normal margins. Do not do “wall of text” or death by bullet points. Always better to land 3 messages than 20. Nobody is reading 20 page CVs
* Use the https://resumeworded.com/ to improve your CV
* Content should say what you did, including a so what or a “who cares”. What impact did your work have on the end customer/user. What difference did you make, what were you responsible for, what did you take accountability for, what innovation did you bring or what risks did you mitigate - this is more interesting than listing 200 technologies. Consider numbers: budget managed, people you led, money saved, number of users serves, number of transactions per second - whatever helps people understand scale
* Try to say what makes you tick / what you are looking for - is it quality or innovation, or helping customers or developing others, or learning new things, working on certain things
* Attitude & alignment to company values > skill and knowledge. You can teach skill but not attitude. So if you are interviewing at AWS know what their leadership principles are and make sure they come across in your cv. Same concept every employer. You want to ensure the recruiter you will fit in, that you're one of them. Same if you're going for leadership jobs. Describe your leadership style
* Sell yourself.  But Be honest. You can emphasise skills and shape your image a bit. But claiming stuff you can't back up at interview is a major no no. I interviewed a guy claiming to had designed loads of VPNs. He couldn't answer any questions in VPNs so that immediately undermined everything else he claimed
* Make it stand out and be memorable - some how 
* Cover your ambitions. Where you want to be or what you want from your next role
* How do you keep up with trends - mention certs you have/want, blogs you write, talks you've given -value you add, what extra curricular stuff they can expect from you
* Use the STAR method to explain your experience. Situation, Task, Actions, Results. Describe the situation, list the task involved and the actions you took to improve the situation and the results you achieved.

## Some interview questions
Go through these and think about situations that you encountered and how you handled them; write it down. If you didn't encounter it think about how you would handle it if you ever came across such a situation.
* Tell me about a time when you handled a challenging situation.
* Tell me about a time when you made a mistake. What did you do to correct it? Tell about a project that failed. How did you handle it? Can you give an example of a time when you wish you’d handled a situation differently? What was it and how do you wish you’d handled it instead? Why?
* Tell me about a time when you were in conflict with a peer and how the situation was resolved.
* Tell me about how you work under pressure. Remain calm in stressful situations. Tell about a particularly stressful event or situation and how you dealt with it.
* Give me an example of how you set goals. Tell me about a goal you set and reached and how you achieved it.
* Give me an example of a time you made a decision that was unpopular and explain how you handled implementing it. Tell me about a time you had to persuade someone else to see your point-of-view or change someone’s mind. How did you go about it? Difficult or unpopular to say and you went ahead and said it./Take risk on a new solution.
* Share an example of how you were able to motivate a coworker, your peers or your team. How you provided good and constructive feedback. Sub-ordinate had a developmental issue and how you helped him.
* Share an example of how you had a disagreement/conflict with a superior Have you ever worked with a difficult boss? In what way was the boss difficult, and how did you handle it? Tell about a time when you knew your boss was wrong. How did you handle the situation?
* Tell me about the last time your workday ended before you were able to get everything done.
* Tell me about a project that you managed
* Most successful project. What made it so successful?
* What’s the largest number of projects you’ve had at the same time? Did you find it challenging? Why or why not?
* How do you approach newly assigned projects? What do you do when a project is first assigned to you?
* Learnings from your past project.
* How do you handle an uncooperative team member?
* Tell about a challenging stakeholder you had on a project. How did you handle it? Have you worked with a customer or team member who was unresponsive? How did you handle it?
* Tell how you demonstrate leadership to the team. How would you develop a high performing team.
* Give an example of a time when you went beyond your normal responsibilities.
* Tell about a difficult decision you had to make. What made it difficult? How did you handle it? What was the outcome.
* Have you ever been given an urgent project that conflicted with other projects you’re working on? How did you handle the situation?/Tell me about a time when you had to change course of action mid-way. Have you ever had to deal with a project with unrealistic timelines?
* Tell me about a goal you failed to achieve.
* Describe how you were accesible to others because they needed your input or advice.
* How do you build relationships in order to ahieve your goals.
* What do you think are the skills required for this role?

## Other stuff
Tech wise. You might get stuff like:
* Can you design from scratch an AWS account? Think org structure
* Lay out VPCs. Zone subnets. Public and private. Add IGW, natGW, DX back to on prem. dns. Ad. Monitoring, logging, config
* Can you put a three tier app into that account? How do you scale it, secure it, make it resilient, add operations features - basically work thru the well architected framework
* Then how do you do other stuff like private link to a SaaS service, or setup redshift for analytics, or migrate data from a legacy thing (these are all scenarios you know super well from SAP) (edited) 
* What happenes when you type Amazon.com into a web browser (tcp, dns, TLS, webserver)
* What is the cloud (maybe sell the benefits of cloud to me)
* What is a container & why would I use one
* What is kubernetes
* Explain CICD to me in much detail
* What's risk management / how do you do it. Tell me about a big risk you took.
* How do you learn things
* What's your biggest failure / what have you learnt / what would you do differently
* What happened to Facebook & how would you have debugged or prevented it
* How would you let a client down / give them bad news like missing a release
* How do you deal with uncertainty or uncertain requirements or change
* How do you deal with conflict (or difficult clients) (edited) 
