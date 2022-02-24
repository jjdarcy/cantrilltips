# Frequently Asked Questions
This FAQ gathers many of the questions asked on https://learn.cantrill.io/ so there is a permanent record of the advice given. 
You can add questions by replacing the "Question x" with your question and writing the anchor replacing spaces with -. Then just add the answer underneath. 
Please submit a PR to add or improve upon this FAQ.

- [How many hours do Adrians videos take?](#how-many-hours-do-videos-take)
- [How long does it take to complete SAA-C02 course?](#how-long-does-it-take-to-complete-saa-c02-course)
- [Why do I get an error creating accounts?](#why-do-i-get-an-error-creating-accounts)
- [Whats Adrians Roadmap for new courses?](#whats-adrians-roadmap-for-new-courses)
- [What is the best path to take through the AWS certifications?](#what-is-the-best-path-to-take-through-the-aws-certifications)
- [Do I need to create new accounts for the course?](#do-i-need-to-create-new-accounts-for-the-course)
- [Are my associate certifications renewed when I pass a professional certification?](#are-my-associate-certifications-renewed-when-i-pass-a-professional-certification)
- [Can i download sessions for offline view?](#can-i-download-sessions-for-offline-view)
- [Why are only 4 layers are covered in the network starter fundamentals?](#why-are-only-4-layers-are-covered-in-the-network-starter-fundamentals)
- [Are the slides of the course available?](#are-the-slides-of-the-course-available)


## How many hours do videos take?

This question has been asked numerous times on [TechStudySlack](https://techstudyslack.com/). So much so, that a student Sherif Fanous created a site that 
Sherif built this Webapp. There are also charts showing the ooverlap between courses. Check it out.
You can find it here: https://cantrill.io.i-aws.cloud/

## How long does it take to complete SAA-C02 course?

For most people you should budget with 6-8 weeks with 1-2 hours study per day. Take all the fundamental lessons to get understanding of the basics in place before 
continuing with the course. The videos are specifically put in an order to help you get the understanding and knowledge of the course.

## Why do I get an error creating accounts

An error "You have exceeded the allowed number of AWS accounts" is sometimes seen even though you are way below the quota maximum. There is a bug. It's been 
around for some time now. It shows "10", but for new accounts the quota is actually set to "2". From discussions on [TechStudySlack](https://techstudyslack.com/)
this error can be seen after some unknown/unspecified period. It grows to the displayed value of 10. Logging a ticket with AWS can help expedite this.

## Whats Adrians Roadmap for new courses?

Adrian has put a notion site together which he keeps updated. 
You can find it here: https://www.notion.so/96fc88a739dc45a59174f1acd8a96776?v=604d7bc7ed9744e1982ef257273d44f9 

## What is the best path to take through the AWS certifications?

Best answer is "It depends" on the role you are going for :-) The certs are divided into Associate and Professional. The specialities are also considered 
Professional. For most people wanting to work with AWS, its best to take the Solutions Architect - Associate (SAA-C02) first to give you the broadest knowledge 
of AWS. Then you can take the other associates; Developer (DVA-01) and SysOps (SOA-C02) or go directly to the Solutions Architect - Professional (SAP-C01) if you
have worked with AWS and feel comfortable moving on to the SAP. Remember: The SAP certification is broad and deep across all AWS services and takes a serious 
focus on study. 

If you do get the SAP-C01, its also a good idea to take the AWS Certified Security - Specialty soon after the SAP-C01 as many of the topics are 
covered already in Adrians SAP-C01 course (with extra reading on AWS KMS). Then the rest of the specialties can be taken in any order. 

## Do I need to create new accounts for the course?

Yes. Create new accounts for each course you take. THIS IS VERY IMPORTANT. 
Accounts in AWS are disposable and give you the permission boundary needed to contain your labs etc. Dont use
existing accounts either as they might have password policies and other contraints that will give you problems during the course. Take the time to create new 
accounts. It will make your life easier :-)

## Are my associate certifications renewed when I pass a professional certification?

As soon as you pass a Professional exam, the relevant **ACTIVE** associate certifications are automatically renewed. If you pass the DevOps Professional 
certification, then both Dev Associate and SysOps Associate are renewed instantly. If you pass the Architect Professional certification, then Architect 
Associate is renewed. 

## Can i download sessions for offline view?

There is no "offline" or download function available as such. However, if you use the Teachable IOS app from the Apple App Store you can download videos and
listen/see them offline. I use it when travelling or when out walking/running to refresh some courses. The Teachable setup is not very user friendly, so patience
is required :-) You need to create a teachable account and link your cantrill.io account to it to be able to access it. See this link for details:
https://support.teachable.com/hc/en-us/articles/236078487-Teachable-Accounts 
At the time of writing, there is no Android equivalent. 

## Why are only 4 layers are covered in the network starter fundamentals?

Layers 5 (SESSION), 6 (PRESENTATION) and 7 (APPLICATION). The application layer is something you organically learn (HTTP/S etc) and the presentation and session layers 
are covered intrinsically throughout the course. The 1-4 layers are the ones that need to be covered in isolation and you get to understand the rest as you go through  
the course.  

## Are the slides of the course available?

Short answer "no". The reasoning behind this is that you need to learn and understand the architecture by going though the course material understanding bit by bit on 
all visuals. On the associated github under https://github.com/acantril you will find a 00_LearningAids folder under some of the topics where a png version of the visuals
is available. 


