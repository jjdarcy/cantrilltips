# Frequently Asked Questions
This FAQ gathers many of the questions asked on https://learn.cantrill.io/ so there is a permanent record of the advice given. 
You can add questions by replacing the "Question x" with your question and writing the anchor replacing spaces with -. Then just add the answer underneath. 
Please submit a PR to add or improve upon this FAQ.

## The Course
<!-- no toc -->
- [Why do I get a 403 forbidden error when accessing?](#why-do-i-get-a-403-forbidden-error-when-accessing)
- [How many hours do videos take?](#how-many-hours-do-videos-take)
- [How long does it take to complete the SAA-C02 course?](#how-long-does-it-take-to-complete-the-saa-c02-course)
- [What's an aggressive, but reasonable timeframe to complete all 3 associates?](#whats-an-aggressive-but-reasonable-timeframe-to-complete-all-3-associates)
- [What's Adrian's Roadmap for new courses?](#whats-adrians-roadmap-for-new-courses)
- [Do I need to create new accounts for the course?](#do-i-need-to-create-new-accounts-for-the-course)
- [Are the slides of the course available?](#are-the-slides-of-the-course-available)
- [Can I download sessions for offline view?](#can-i-download-sessions-for-offline-view)
- [Resetting course progress?](#resetting-course-progress)
- [Is there a PDF of the course?](#is-there-a-pdf-of-the-course)
- [Why is the answer 177 IPs in a slash 24 network](#why-is-the-answer-177-ips-in-a-slash-24-network)
- [Is there a discount or bundle discount for the courses?](#is-there-a-discount-or-bundle-discount-for-the-courses)
- [What is the difference between a management account and an organisation root?](#what-is-the-difference-between-a-management-account-and-an-organisation-root)

## Study
- [Whats the best study technique?](#whats-the-best-study-technique)
- [Are there any problems with Architecture Evolution demo?](#are-there-any-problems-with-architecture-evolution-demo)
- [Any ideas as to what applications I should write to help me learn?](#any-ideas-as-to-what-applications-i-should-write-to-help-me-learn)
- [Do these courses help you get real jobs at the end?](#do-these-courses-help-you-get-real-jobs-at-the-end)

## Certifications
- [What is the best path to take through the AWS certifications?](#what-is-the-best-path-to-take-through-the-aws-certifications)
- [Are my associate certifications renewed when I pass a professional certification?](#are-my-associate-certifications-renewed-when-i-pass-a-professional-certification)

## Miscellaenous
- [Why do I get an error creating accounts in an AWS Organization?](#why-do-i-get-an-error-creating-accounts-in-an-aws-organization)
- [Why are only 4 layers covered in the network starter fundamentals?](#why-are-only-4-layers-covered-in-the-network-starter-fundamentals)
- [How do I populate my shortcuts bar in the AWS Console?](#how-do-i-populate-my-shortcuts-bar-in-the-aws-console)
- [Cross account permissions on buckets - Why is the answer not denied?](#why-is-the-answer-not-denied)
- [What are the AWS IAM permissions on a ConsoleSignIn event?](#what-are-the-aws-iam-permissions-on-a-consolelogin-event)
- [Any good Linux courses?](#any-good-linux-courses)
- [Any good resources to use when coding CloudFormation?](#any-good-resources-to-use-when-coding-cloudformation)


## Why do I get a 403 forbidden error when accessing?
Teachable have made some changes. If you get this error please check the following:
* If you are using a browser with tracking protection ... do you have it enabled, standard, strict 
* are you using private tabs or normal tabs
* are you using a VPN
* what OS, what browser
* any workplace restrictions
* the new player is designed to make ripping videos harder which is why it reacts badly to some stuff you can be running
* do you have an ad blocker turned on  
Most of the time is the browser tracking protection that is the issue. 

## How many hours do videos take?
This question has been asked numerous times on [TechStudySlack](https://techstudyslack.com/). So much so, that a student Sherif Fanous created a Webapp, and also charts showing the overlap between courses. Check it out.

You can find it here: https://cantrill.io.i-aws.cloud/

## How long does it take to complete the SAA-C02 course?
For most people you should budget 6-8 weeks of your time with around 1-2 hours study per day. 

> ⚠️ Make sure **not** to skip any of the fundamental lessons to get a good understanding of the basics! See Adrian's linkedin post about [focusing on fundamentals](https://www.linkedin.com/posts/adriancantrill_a-friend-of-mine-derek-morgan-just-wrote-activity-6922425127859077120-Od7z?utm_source=linkedin_share&utm_medium=member_desktop_web).

The videos were specifically put in an order that will help ease you into the more complicated topics as you go through the course.


## What's an aggressive, but reasonable timeframe to complete all 3 associates?
The average is 6-8 weeks given 1-2 hours a day per exam. It all depends on your skill level and whether you're focusing on *learning* rather than *passing*.

The setup in Adrian's courses starts with setting up an [AWS Organization](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_introduction.html), as this is the kind of environment most companies using AWS have implemented in their workplace. 

Adrian's courses are also designed to overlap, so after completing the first associate you can complete the other Associates in a short time. See [here](#how-long-does-it-take-to-complete-the-saa-c02-course)
 for more details.


## Why do I get an error creating accounts in an AWS Organization?
> ❌ **You have exceeded the allowed number of AWS accounts**

This error can occur even though you are below the [quota maximum](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_reference_limits.html). **This is a bug.**

It's been around for some time now. It shows "10", but for new accounts the quota is actually set to "2". From discussions on [TechStudySlack](https://techstudyslack.com/) this error *can resolve itself* after some unknown/unspecified period.

Logging a ticket with AWS can help expedite this.

## What's Adrian's Roadmap for new courses?
Adrian has put a notion site together which he keeps updated. 
You can find it [here](https://www.notion.so/96fc88a739dc45a59174f1acd8a96776?v=604d7bc7ed9744e1982ef257273d44f9). 

## What is the best path to take through the AWS certifications?
Best answer is "It depends" on the role you are going for :-) The certs are divided into **Associate** and **Professional**. The speciality exams are also considered Professional. 

No matter what your chosen role is, it's usually best to take the `Solutions Architect - Associate (SAA-C02)` first to give you broad knowledge of AWS. Afterwards, you can go for the other associates; `Developer (DVA-01)` and `SysOps (SOA-C02)` or go directly to the `Solutions Architect - Professional (SAP-C01)` if you have worked with AWS and feel comfortable moving on to the `SAP-C01`. Remember: The `SAP-C01` certification is very broad and deep across all AWS services and will require a serious effort on study and focus. 

If you do get the `SAP-C01`, it can be a good idea to take the `AWS Certified DevOps Engineer - Professional (DOP-C01)` immediately afterwards, because there is significant overlap.

The `AWS Certified Security - Specialty (SCS-C01)` is also a very good target after the `SAP-C01`, as it's considered the easiest AWS Speciality Exam and many topics are already covered in Adrian's `SAP-C01` course (with some extra reading on AWS KMS).

The rest of the Speciality Exams can be taken in any order. 

## Do I need to create new accounts for the course?
Yes. Create new accounts for each course you take. THIS IS VERY IMPORTANT. 
Accounts in AWS are disposable and give you the permission boundary needed to contain your labs, etc. Don't use sandbox accounts or
existing accounts either as they might have password policies and other contraints that will give you problems during the course. Take the time to create new 
accounts. It will make your life easier :-)

## Are my associate certifications renewed when I pass a professional certification?
As soon as you pass a Professional exam, the relevant **ACTIVE** associate certifications are automatically renewed. If you pass the DevOps Professional 
certification, then both Dev Associate and SysOps Associate are renewed instantly. If you pass the Architect Professional certification, then Architect 
Associate is renewed. 

## Can I download sessions for offline view?
There is no "offline" or download function available as such. However, if you use the Teachable IOS app from the Apple App Store you can download videos and
listen/see them offline. I use it when travelling or when out walking/running to refresh some courses. The Teachable setup is not very user friendly, so patience
is required :-) You need to create a teachable account and link your cantrill.io account to it to be able to access it. See this link for details:
https://support.teachable.com/hc/en-us/articles/236078487-Teachable-Accounts 
At the time of writing, there is no Android equivalent. 

## Why are only 4 layers covered in the network starter fundamentals?
Layers 5 (SESSION), 6 (PRESENTATION) and 7 (APPLICATION). The application layer is something you organically learn (HTTP/S etc) and the presentation and session layers are covered intrinsically throughout the course. The 1-4 layers are the ones that need to be covered in isolation and you get to understand the rest as you go through the course.  

## Are the slides of the course available?
Short answer "no". The reasoning behind this is that you need to learn and understand the architecture by going though the course material understanding bit by bit on all visuals. On the associated github under https://github.com/acantril you will find a 00_LearningAids folder under some of the topics where a png version of the visuals is available. 

## Any ideas as to what applications I should write to help me learn?
You should choose a project that solves some problem or helps you (or your friends/family) in some way. You’ll be more productive and more motivated this way.

Can really be anything, here are some ideas:
* Cryptocurrency tracking application of some kind
* Personal cloud storage (OneDrive/Dropbox clone, but YOURS!)
* VPN for you and all your devices
* Blog/website of your own

I’ll use one example, and illustrate what you can do for a personal project that you can showcase on Linkedin, and I’ll take personal cloud storage as an example. For this, I’ll be using [Nextcloud](https://nextcloud.com/):
- Deploy NextCloud locally on your computer and test it out, see how it works.
- Deploy NextCloud on an EC2 instance, install the NextCloud client on both your phone and computer and make sure you can upload/download files.
- Migrate the database to RDS and make NextCloud work with it. Migrate the storage to S3 (or EFS/EBS, whatever you want).
- Put CloudFront in front of your NextCloud instance, add an ACM certificate and make sure it’s HTTPS-only (redirect from HTTP->HTTPS)
- Migrate your application from EC2 to ECS, deploy NextCloud as a Fargate container. If you want, migrate your database to a container as well.
- Put a load balancer in front of ECS
- Now define everything that you did in code using CloudFormation/Terraform/Pulumi, whatever you want.
- Put it all in a git repository (Github/Gitlab). Make sure not to commit any secrets to your repo!
- Use CI/CD to automatically deploy everything.
- Create an architecture diagram in the README.md and make sure to provide detailed instructions so anyone can deploy what you just did
- Once your repo is ready, publish to Linkedin, along with a blog post telling about your journey and what you learned.

You can do a lot more, and use a lot more AWS services and make this more complicated. Just bear in mind that this example can be expensive if you upload/download a lot of data from/to AWS. You should use it as a project and proof of concept. But you can go even further and cost optimize your project architecture.

## Do these courses help you get real jobs at the end?
Certifications get you interviews but not jobs. It gets you to the table. Experience gets you jobs (on the job, personal projects or stuff learned while studying). Adrian's courses are very skill focussed. It's a "by-product" getting the certifications. He is preparing you for real work experience.

## Resetting course progress?
Technically, from what Teachable have said, it is possible with a loooooooot of work for Adrian to reset the course progress. But he has to delete the whole profile for every single person who asks, 1 at a time. And then we'd never get new lessons or updates! So very reasonably, Adrian has said "no". You could possibly log a support request with Teachable to ask for students to be able to reset their own progress.

## Is there a PDF of the course?
Quick answer is "NO". The best way to learn anything is to take your own notes. This makes sure you understand the material in the course. All studies show that taking your own notes helps you understand what you are learning. See: https://www.lifehack.org/articles/featured/writing-and-remembering-why-we-remember-what-we-write.html

There are learning aids in the Github repo but that is specific details and not a PDF of whats said in the course material. See README.md for how best to take notes. 

## How do I populate my shortcuts bar in the AWS Console?
AWS have recently released a shortcut bare at the top of the console. If you want to create a shortcut to your most used services follow the below instructions:
- Press services to list the most recently used services
![Services](./images/services.png?raw=true "Services")
- Click on the "star" beside the service and there you go. The services will be listed on your shortcut bar.
![Star](./images/listoservices.png?raw=true "List of Services")

## Are there any problems with Architecture Evolution demo?
Directly from the slack channel from a student: 

> *I am trying to **manually** follow this demo ([AdvancedDemo] Architecture Evolution) in another AWS account and another zone. 
I've created manualy the VPC, subnets, security groups, role (InstanceProfile) and parameter store variables, but is always failing at the first Launch Template from Stage 2 and Wordpress is not getting installed. Stage 1 with the manual Wodpress installation is going well. I've spent a couple of days on this one now :) and everything is pointing me to the 1-Click deployment from STEP1 that creates the base infrastructure and is hardcoded in that 1-Click deployment. I wonder what am I am missing here? I saw that 1-Click deployment has some fixes related to IPV6 but I don't think that is the problem. It is possible to modify the Cloud Formation 1-Click deployment to run in another region? I couldn't find anything in yaml file that set the region.*

Snippets of the discussion (Adrians comments in bold, student in italics)

- Adrian: **Did you check the logs - they are in /var/log there will be cloud-init logs files**
- Adrian: **Remember just because the instance is provisioned doesn't mean the userdata has finished**
- Student: *logs shows that php install is still running...*
- Student: *took 3-5 more minute to finish after the instance was actually up*
- Adrian: **thats normal**
- Adrian: **thats why we use CFN creation policies/signals**
- Student: *but I learned so many things just trying to figure out the issue:)*
- Student: *it is easy to modify that 1-clik deployment to use another region or is more than that Yaml file ?*
- Adrian: **its easy if you know what to change**
- Adrian: **I stick to us-east-1 for a ton of reasons though**
- Adrian: **its the region which is always guarenteed to have all services**
- Adrian: **its the region all global services log to/bill to**
- Adrian: **so its the perfect one to use for study/non production workloads**

## Whats the best study technique?
There is really no "one size fits all" here, but probably the best study technique is: 
* `read/watch => understand => compress => write => revisit`

This is the key to storing information in your long term memory. And write here means `take your own notes`. Some students like flash cards. These are good as long as you create them yourself and not use other peoples'. Using other peoples means you only remember things - creating them means you go through a process which encourages understanding.

## Why is the answer not denied?
![Star](./images/crossaccpol.png?raw=true "TutDoJo Question")

Remember SCPs only affect identities in that account. The identity is not in the same account as the SCP. The resource policy on the bucket allows the account the identity is in to access. The identity policy allows access to S3, so access is allowed. 

## What are the AWS IAM permissions on a ConsoleLogin event?
You can't deny a `ConsoleSignIn` event. For example if you put a deny all policy on an IAM user they can still login. They can't see or do anything.

So how does AWS SSO work in the backend? AWS SSO drops you into a role in an Account. AWS SSO manages SAML providers that get auto-provisioned in your AWS accounts. AWS SSO also auto-provisions service-roles that match your Permission Sets that you have configured within AWS SSO.

In AWS SSO you may see a `signin:UserAuthentication` event in your Management AWS account. Within the Management AWS Account you will also see a `sso:Authenticate` event entering the SSO system. Then there will be an `sso:Federate` call leaving SSO environment. In the member account you will then see a `sts:AssumeRoleWithSAML` (likely logged to both Management and member accounts). The role that is assumed is one of the provisioned roles that the assigned PermissionSets within AWS SSO grants access to. Following this you will see a `signin:ConsoleLogin` event with an `userIdentity` type of AssumedRole (the role is the AWS SSO service-role matching the PermissionSet).

You may also see `sso:GetRoleCredentials` instead of `sso:Federate`. This is the mechanism that generates the short-lived API tokens from the SSO portal.

Also see https://aws.amazon.com/blogs/security/aws-cloudtrail-now-logs-aws-management-console-sign-in-events/ 

## Any good Linux courses?
* Free
  * https://www.youtube.com/c/LearnLinuxtv/playlists
  * https://blog.feedspot.com/linux_blogs/
  * https://linux-training.be/
  * https://www.server-world.info/en/
* Non-Free
  * Udemy: Linux Administration: The Complete Linux Bootcamp for 2022, Andrei Dimitrescu
  * LinkedIn Learning - All from Grant McWilliams
  * Cisco’s -  NDG Linux Essentials, and NDG Linux I, and II which indeed covers LPIC
  * https://www.edx.org/search?q=linux

## Any good resources to use when coding CloudFormation?
Going through Adrians course and examining the templates he uses is a great wy to understand CloudFormation. Also there are some good places to get sample templates and of course the referance pages. Some good sites to bookmark:
* https://github.com/aws-cloudformation/aws-cloudformation-samples
* https://github.com/awslabs/aws-cloudformation-templates
* https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/CHAP_TemplateQuickRef.html
* https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html

## Why is the answer 177 IPs in a slash 24 network
This a question that turns up a lot on the slack channel. Finally, got around to getting it in here :-).  

The question is:
* *You have a VPC which uses the CIDR of `10.0.0.0/24`. This is split into 3 subnets, 1 in each Availability zone. How many total usable IPs are available in the three subnets in total?*

I'll try to get you thinking, so that you can work it out and understand yourself. Understanding subnetting and CIDRs is essential for moving forward.     

Think how to determine the start point of a CIDR range. Take the IP 10.0.0.0 as in the question. What are all the valid subnets and ranges from this IP. Take this diagram:  
![Ranges](./images/ranges.png?raw=true "Ranges")
As you can see from the diagram, that a /24 can not be broken into 3 even parts as the start and end ranges wont work. It would have to go into 4 /26s with 1 spare or a /25 and 2 /26s and put up with uneven sizes.  

Have a look at the illustration Adrian has in the course:  
![Subnetting](./images/subnetting.png?raw=true "Subnetting")

> ⚠️ Remember there are [5 reserved AWS IPs](https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html#subnet-sizing) in any subnet. 

## Is there a discount or bundle discount for the courses?
Quote from Adrian:  
>"I want to make sure you're getting maximum value from https://learn.cantrill.io.  
>Whatever you've enrolled in, you can always upgrade to a bundle or a larger bundle by paying the difference.  
>Just use our support form ( https://learncantrill.zendesk.com/hc/en-us/requests/new ).  
>Let us know the email you registered with, what content you own, and what bundle you want, and we'll get you a personal upgrade link sent ASAP."

## What is the difference between a management account and an organisation root?
Think of the organisational root as a container. An Organisational Unit (OU) at the top of the organisation at the top most point where other OU's or accounts are located. The management account is the AWS account which created the ORGANISATION. Its an AWS account, and it's special in a few ways.  

An AWS account (member or management) cannot BE an organisation root, because the organisational root is not an AWS account, its the top most point as above. 
