---
layout: blogpost
title: "Pulse Sequences to Pull Requests: My Month with GSTT-CSC" 
tag-line: "Mario Nicola discusses his recent elective"
date: "19 May 2026"
read-time-mins: "7 mins"
image: /assets/img/blog/mario.png
author: "Mario Nicola" 
author-image: /assets/img/team/standard_user.jpg
author-role: "Trainee Clinical Scientist"
category: Blog
---
_Mario Nicola is a trainee clinical scientist in medical physics, but he is particularly interested in computer science._

Alongside studying physics and training as a clinical scientist, I have been interested in software development, especially in clinical use cases. In my MSc project at Nottingham, I built a traditional machine learning classifier for excised suspected skin cancer samples. In my MSc project at King's (right before my elective), I built a super-resolution network for real-time speech MRI. However, both of these projects lacked proper version control and modular code because the codebase was either solely written by me, or by me and one other person.

From speaking to past trainees who had spent time here and reading other blog posts, I decided that undertaking an elective at CSC would be the perfect way to gain a better understanding of how to build and maintain software collaboratively. After meeting [Elise](/team_member/elise.html) and [Molly](/team_member/molly.html) over Teams, we scheduled a month-long elective for April. Soon after, I found out that I would be joining GSTT in the MRI Physics team in September, with a secondary focus on computing, making the elective even more suitable for my professional development.

Before starting, I set out a few goals:
1. Understand how GSTT-CSC structure projects and maintain their Quality Management System.
2. Write a few unit tests and understand their importance.
3. Open at least one pull request, no matter how small the contribution is.
4. Understand how to use GitHub for version control.

The first thing I did was ask some members of the team what they were working on. I also went through the GitHub to see how projects have been built out and what I may be able to contribute to. I learned about the MLOps (machine learning operations) workflow through a tutorial that demonstrates how to use the CSC-MLOps XNAT interface along with PyTorch Lightning and Monai to run training for hippocampus segmentation. I was reminded of how useful Docker can be in the setup of XNAT and MLOps servers. And I used MLflow for the first time (despite having trained models in the past). After some repo-surfing and discussions, I decided that I could contribute to the Research Analytics App and help with some QMS Automation.

In terms of QMS automation, I was tasked with adapting the flowchart for ISO 13485 compliance. I added SOP and Template boxes in the draw.io schematic. When loading these changes into my integrated development environment, I used the properties of the XML file to write Python scripts for hyperlink injection. This converts lists of QMS documentation for a project into a clickable diagram that updates links according to a config file. This exercise fulfilled two of my above goals.

<figure>
<img src="/assets/img/blog/clickable_diagrams.png" width="100%">
<figcaption>Adapting a flowchart for ISO 13485 compliance.</figcaption>
</figure>

For the Research Web App, I was keen to write some unit tests for the first time ever. Unit testing catches bugs early before they cascade into production, saving hours of debugging later. With pytest, I found tests can be surprisingly fast to write and give confidence when refactoring. The most difficult part was thinking of what tests to do. I picked up a live issue involving API and serializer unit tests. On future projects, I will carry on the practice of proper unit testing since seeing tests passed made me more confident in submitting code.

<figure>
<img src="/assets/img/blog/research_web_app.png" width="100%">
<figcaption>Testing the Research Web App.</figcaption>
</figure>

Probably the most fun I had coding was when I was building a paginated static guidance page for the Research Web App. I had never worked with Django, React, or any sort of frontend development. So, it took a while to get to grips with it all. I enjoyed watching my code change the Research Web App in real time, making for a dopamine-driven feedback loop that kept me going. From now on, I will never underestimate how much thought beautiful web pages and apps require. The image below shows my favourite part: the change in an arrow's colour when the cursor hovers over it.

<figure>
<img src="/assets/img/blog/colour_change.png" width="100%">
<figcaption>An arrow changes colour: dopamine is released.</figcaption>
</figure>

I also really enjoyed the variety of meetings the CSC team held. Technical Tuesdays meetings featured updates on projects like OsteoAI and AutoSegCT as well as brainstorming exercises on launching new projects. I especially appreciated the retrospective section of a 10X Thursday meeting during which recent events were discussed, with a focus on hearing out concerns and improving how the team works; it’s something I’d love to introduce my future teams to. Not least, it ensures that everyone’s voice is heard (even anonymously).

As a lifelong die-hard Tottenham F.C. fan, I never thought I’d be sitting in the home end of the Emirates stadium; but, for a CSC social, it was worth it. We watched Arsenal Women beat Leicester (and former Spurs captain Ashleigh Neville) 7-0 and had a great time away from our screens.

<figure>
<img src="/assets/img/blog/arsenal.png" width="100%">
<figcaption>A CSC social at the Emirates. Arsenal 7-0 Leicester!</figcaption>
</figure>

If anyone reading this is considering picking up some software development skills and experiencing a few weeks with a fun and friendly team of experts from a multidisciplinary background, apply!

I leave CSC with both more confidence in my ability to structure projects and a sense of humility in that I have even more than I thought to learn before becoming the physicist/computer scientist hybrid specialist I’ve always wanted to be.

Lastly, a massive thank you to Molly who supervised my elective (and a couple pub trips) and to the whole team for making me feel so welcome with their infectious enthusiasm. I would’ve loved to have spent more time with the team, but I have a OneFile mountain to finish climbing… See you around, CSC!
