# Frequently Asked Questions
This FAQ gathers many of the questions asked on https://learn.cantrill.io/ so there is a permanent record of the advice given. 
You can add questions by replacing the "Question x" with your question and writing the anchor replacing spaces with -. Then just add the answer underneath. 
Please submit a PR to add or improve upon this FAQ.

- [How many hours do Adrians videos take?](#how-many-hours-do-videos-take)
- [How long does it take to complete SAA-C02 course?](#how-long-does-it-take-to-complete-saa-c02-course)
- [Whats an aggressive but reasonable timeframe to complete all 3 associates?](#whats-an-aggressive-but-reasonable-timeframe-to-complete-all-3-associates)
- [Why do I get an error creating accounts?](#why-do-i-get-an-error-creating-accounts)
- [Whats Adrians Roadmap for new courses?](#whats-adrians-roadmap-for-new-courses)
- [What is the best path to take through the AWS certifications?](#what-is-the-best-path-to-take-through-the-aws-certifications)
- [Do I need to create new accounts for the course?](#do-i-need-to-create-new-accounts-for-the-course)
- [Are my associate certifications renewed when I pass a professional certification?](#are-my-associate-certifications-renewed-when-i-pass-a-professional-certification)
- [Can i download sessions for offline view?](#can-i-download-sessions-for-offline-view)
- [Why are only 4 layers are covered in the network starter fundamentals?](#why-are-only-4-layers-are-covered-in-the-network-starter-fundamentals)
- [Are the slides of the course available?](#are-the-slides-of-the-course-available)
- [Any ideas as to what applications should I write to help me learn?](#any-ideas-as-to-what-applications-should-i-write-to-help-me-learn)
- [Do these courses help you get real jobs at the end?](#do-these-courses-help-you-get-real-jobs-at-the-end)
- [Resetting course progress?](#resetting-course-progress)
- [Is there a PDFF of the course?](#is-there-a-pdf-of-the-course)


## How many hours do videos take?

This question has been asked numerous times on [TechStudySlack](https://techstudyslack.com/). So much so, that a student Sherif Fanous created a Webapp, and also
charts showing the overlap between courses. Check it out.
You can find it here: https://cantrill.io.i-aws.cloud/

## How long does it take to complete SAA-C02 course?

For most people you should budget 6-8 weeks with 1-2 hours study per day. Take all the fundamental lessons to get understanding of the basics in place before 
continuing with the course. The videos are specifically put in an order to help you get the understanding and knowledge of the course.

## What's an aggressive but reasonable timeframe to complete all 3 associates?
The average is 6-8 weeks given 1-2 hours a day per exam. It all depends on your skill level and how much you are focussing on learning versus passing. The setup
in Adrian's courses starts with an organisational configuration as this is what people see in their workplaces also. Adrians courses are also designed to 
overlap, so after completing the first associate that is cut down by 60% for the other courses as he has designed for this overlap, 

## Why do I get an error creating accounts in an Organization

An error "You have exceeded the allowed number of AWS accounts" is sometimes seen even though you are way below the quota maximum. There is a bug. It's been 
around for some time now. It shows "10", but for new accounts the quota is actually set to "2". From discussions on [TechStudySlack](https://techstudyslack.com/)
this error can resolve itself after some unknown/unspecified period. It grows to the displayed value of 10. Logging a ticket with AWS can help expedite this.

## What's Adrian's Roadmap for new courses?

Adrian has put a notion site together which he keeps updated. 
You can find it here: https://www.notion.so/96fc88a739dc45a59174f1acd8a96776?v=604d7bc7ed9744e1982ef257273d44f9 

## What is the best path to take through the AWS certifications?

Best answer is "It depends" on the role you are going for :-) The certs are divided into Associate and Professional. The specialities are also considered 
Professional. For most people wanting to work with AWS, it's best to take the Solutions Architect - Associate (SAA-C02) first to give you the broadest knowledge 
of AWS. Then you can take the other associates; Developer (DVA-01) and SysOps (SOA-C02) or go directly to the Solutions Architect - Professional (SAP-C01) if you
have worked with AWS and feel comfortable moving on to the SAP. Remember: The SAP certification is broad and deep across all AWS services and takes a serious 
focus on study. 

If you do get the SAP-C01, its also a good idea to take the AWS Certified Security - Specialty soon after the SAP-C01 as many of the topics are 
covered already in Adrian's SAP-C01 course (with extra reading on AWS KMS). Then the rest of the specialties can be taken in any order. 

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

Layers 5 (SESSION), 6 (PRESENTATION) and 7 (APPLICATION). The application layer is something you organically learn (HTTP/S etc) and the presentation and session
layers are covered intrinsically throughout the course. The 1-4 layers are the ones that need to be covered in isolation and you get to understand the rest as
you go through the course.  

## Are the slides of the course available?

Short answer "no". The reasoning behind this is that you need to learn and understand the architecture by going though the course material understanding bit by
bit on all visuals. On the associated github under https://github.com/acantril you will find a 00_LearningAids folder under some of the topics where a png
version of the visuals is available. 

## Any ideas as to what applications should I write to help me learn?
You should choose a project that solves some problem or helps you (or your friends/family) in some way. You’ll be more productive and more motivated that way.
Can really be anything, here are some ideas:
* Cryptocurrency tracking application of some kind
* Personal cloud storage (OneDrive/Dropbox clone, but YOURS!)
* VPN for you and all your devices
* Blog/website of your own

I’ll use one example, and illustrate what you can do for a personal project that you can showcase on Linkedin, and I’ll take personal cloud storage as an
example. For this, I’ll be using Nextcloud https://nextcloud.com/:
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

You can do a lot more, and use a lot more AWS services and make this more complicated. Just bear in mind that this example can be expensive if you
upload/download a lot of data from/to AWS. You should use it as a project and proof of concept. But you can go even further and cost optimize your project
architecture.

## Do these courses help you get real jobs at the end?
Certifications get you interviews but not jobs. It gets you to the table. Experience gets you jobs (on the job, personal projects or stuff learned while 
studying). Adrian's courses are very skill focussed. It's a "by-product" getting the certifications. He is preparing you for real work experience. 

## Resetting course progress?
Technically, from what Teachable have said, it is possible with a loooooooot of work for Adrian to reset the course progress. But he has to delete the whole
profile for every single person who asks, 1 at a time. And then we'd never get new lessons or updates!
So very reasonably, Adrian has said "no". You could possibly log a support request with Teachable to ask for students to be able to reset their own progress.

## Is there a PDF of the course?
Qucik answer is "NO". The best way to learn anything is to take your own notes. This makes sure you understand the material in the course. All studies show that taking
your own notes helps you understand what you are learning. See: https://www.lifehack.org/articles/featured/writing-and-remembering-why-we-remember-what-we-write.html
There are learning aids in the Github repo but that is specific details and not a PDF of whats said in the course material. See README.md for how best to take notes. 
