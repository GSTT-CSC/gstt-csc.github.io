---
layout: blogpost
title: My elective with the CSC Team
tag-line: "Lydia describes her time with CSC on her 2-week-long STP elective."
date: "4 April 2023"
read-time-mins: "3 mins"
image: /assets/img/blog/lydia_blog.png
author: Lydia Davidson
author-image: /assets/img/team/standard_user.jpg
author-role: Trainee Clinical Scientist in Imaging with Ionising Radiation, Royal United Hospital Bath
---

As a trainee medical physicist, we’re encouraged to take a few weeks out to do some work experience to stretch ourselves beyond the remit of our day jobs – and I thought what better way to stretch myself than helping create artificial intelligence apps! 

My first week in the CSC team was an exciting one, where I was thrown into a three-day hackathon event in London. A hackathon, I soon found out, is an event that brings programmers and other interested parties together to improve upon or build a new software program. This form of working is novel in the NHS and so it was exciting to be part of one of the first groups paving the way on this front. The focus of the hackathon was to further develop a scaphoid fracture diagnostic tool the CSC team had been working on, ‘ScaphX’ (read more about the app [here](https://gstt-csc.github.io/projects/AIC002-occult-carpal-detection-xray.html)). We were split into three teams covering software development, app design and integration, and documentation. The attendees were an eclectic mix of people, from radiologists and surgeons to software developers, quality managers and physicists, with each bringing their own unique expertise and insights.  

My main task over the hackathon was to interrogate the data from the ‘gold standard’ test dataset. This is one of the three subsets that you split your original dataset into when creating an AI model (with the other two being the training set and the validation set). 

<figure>
<img src="/assets/img/blog/lydia_blog_TVT.png" width="100%">
<figcaption>Diagram showing the typical split in data when creating an AI model. </figcaption>
</figure>

In supervised learning, the ‘train’ dataset is used to feed the model labelled examples. You then test your trained dataset using the ‘validation’ dataset every time the model is fine tuned to compare which model parameters are optimal, and the golden standard ‘test’ dataset is only used once the model is completely trained and is used to provide an evaluation of the finished model.  

I analysed the distribution of the age, ethnicity, and gender categories in the golden standard dataset, and looked at the proportion of each sub-category who were diagnosed with a scaphoid fracture. This was partly to ensure there were enough of each category being represented in the test set, but also to look for any trends in the data. The results of my analysis indicated that there was a correlation between gender and fracture diagnosis, and so I performed a power analysis to work out if we had a sufficient sample size to reliably demonstrate that ScaphX results are not driven by patient characteristics, but by the presence or absence of a scaphoid fracture. I really enjoyed using the knowledge gained in my statistics lectures through my medical physics course in a meaningful way, and produce some useful data insights for the team at the same time.

In my second week, I yet again put my university lectures into practice when I was tasked with writing some code to automate a time-consuming task. After a lot of head scratching and YouTube tutorials, I produced a Python script that extracts a given DICOM tag from all subfolders containing DICOM files within a stated directory. This was a great exercise for me, as I had little previous coding experience and so it gave me a confidence boost in my ability to apply myself to new coding problems. 

Also in my second week, I got to talk with several members of the CSC team and find out a bit more about what they do. First I spoke to [Anil Mistry](https://gstt-csc.github.io/team_member/anil.html), who showed me the AIDE platform. AIDE essentially acts as both an ‘app store’ for AI apps and a router which can work out what type of data it’s being sent and then from this will send it to where it needs to go. I also learnt about the various regulatory hurdles associated with releasing an AI app and achieving department accreditation, such as ISO 13485 medical devices requirements, UKCA marking and BSI requirements. I was surprised CSC used Github for their quality management system as I hadn’t considered this as an option before, but it made a lot of sense and brought a lot of efficiencies. 

Two of the team’s AI engineers, [Laurence Jackson](https://gstt-csc.github.io/team_member/laurence.html) and [Thomas Roberts](https://gstt-csc.github.io/team_member/tom.html), talked to me about their interesting career journeys from getting PhDs in imaging physics to their current software development roles. Through Laurence I learnt that the AI models they develop are written in Python, and after tweaking the model parameters, the success of that particular run compared to others performed can be assessed using a program called MLflow. MLflow is essentially an end-to-end [MLOps](https://gstt-csc.github.io/platforms/mlops.html) platform that allows you to trigger training runs, track your experiments to see which performance was better or worse, and register your models for auditability. I also spoke to Tom, who told me a large part of his current role involves adapting and repacking existing AI models into apps that can be made available on AIDE. One such model is an open-source CT segmentation model that automatically contours specific anatomy, which Tom is currently working on adapting the input to be a DICOM imaging standard rather than the NlfTI standard. 

[Dika Vilic](https://gstt-csc.github.io/team_member/dika.html), a clinical scientist for the CSC gave me the low down on what [XNAT](https://gstt-csc.github.io/platforms/xnat.html) is and why it’s so valuable for the team. In short, XNAT is a research picture archiving and communication system (PACS) that allows much more freedom compared to most clinical PACS systems used by NHS trusts. It also links with both AIDE and PACS. With XNAT, you can retrieve bulk amounts of DICOM files from clinical PACS systems with ease, and it lets you write and apply patient data anonymisation scripts. 

These chats really helped to paint a picture of the overarching function of the department and how each member plays a part. 

My two weeks with the CSC team were varied, fun and hugely insightful. The key take-away from my experience is that everyone is capable of finding innovative ways to improve efficiency within their work remit and should feel empowered to do so, even if it disrupts a long-standing and well-established process. I’ve learnt that disruption can be a force of good, and it’s unlikely you can achieve innovation without it.

