---
layout: blogpost
title: Developing ScaphX and FOOSHnet, a 2-part hackathon
tag-line: "Developing AI in focussed-work events"
date: "18 May 2023"
read-time-mins: "8 mins"
image: /assets/img/blog/Hackathon-pic-1.jpg
author: Dika Vilic
author-image: /assets/img/team/dika.jpg
author-role: 
---

The CSC tackled the development of two AI models in two 3-day hyper focussed team events which we called hackathons. The first took place in November of 2022, where we focussed on both models in two separate teams, and the second took place in February 2023 where we focussed on only one model.

Both projects had been worked on in isolation before by two or three people at a time and were at model development stage. The projects tackled are described [here](https://gstt-csc.github.io/projects/AIC002-occult-carpal-detection-xray.html) and [here](https://gstt-csc.github.io/projects/AIC005-occult_carpal_detection_in_mri.html), and both aim to facilitate faster diagnosis of scaphoid fractures. 

This blogpost details the way we organised and executed both events and highlights the lessons we learned along the way.

# First hackathon


We identified tasks which broadly correspond to 3 parallel streams of work: model development, package development and documentation writing. The word spread that we were holding a hackathon and other people wanted to participate who do not
usually work with the CSC, including clinical AI fellows and other physicists, resulting in a total of 13 participants. For this reason we split into two teams, with half the team tackling the MRI project 
and the other half the X-ray project.

The preparation for the hackathon lasted around 2 months and included activities such as 
- data exploratory analysis
- stakeholder meetings to formalise user requirements
- model setup
- pre-hackathon meetings including 
    - scaphoid fracture diagnosis lesson 
    - MLOps lesson
    - QMS lesson
    
To measure the success of our teams we also set up achievement milestones:
- bronze medal: partial documentation, a basic model that takes data and gives output
- silver medal: partially complete QMS, trained model (not meeting performance requirements), basic app for AIDE
- gold medal: trained model on MONAI-compliant application with signed-off QMS, quantified performance across available demographic information
- platinum medal: all gold aims + app name, finishing time for pub, website updated

On the first day of the hackathon, we had a presentation on the two projects to get everyone up to speed. We divided into teams and got to work.

Most of the first day was spent on MLOps training, installation of requirements and getting the models to perform training. Each day was closed with a
show and tell of the day's progress and the final day included a wrap up with feedback from everyone on what went well and what could be improved upon.

By end of day 3 we had an X-ray team (naming their model ScaphX) with a silver medal and an MRI team (naming their model FOOSHnet) with a bronze medal. Overall, much more work was still needed.

<figure>
<img src="/assets/img/blog/Hackathon-pic-4.jpg" width="100%">
<figcaption>We separated into MRI-project team (FOOSHnet) and Xray-project (ScaphX) team.</figcaption>
</figure>

# Second hackathon
We learned many lessons from our first hackathon and tackled the second one in a different way. We 
adjusted our preparation work and the rules of the hackathon accordingly. 

Things we didn't know before:
1. The sheer amount of work needed to push forward model development and document the process in parallel requires all hands on deck.
2. There is not much time to train or install things during a hackathon: these activities should be done in advance.
3. The work which needs to be done must be broken down into smaller, manageable tasks in advance.
4. Each task should be transparently assigned to the person tackling it.
5. Tracking work is hard when multiple people are working on a task at once which leads to inefficiencies and errors.
6. Not having branch-naming rules causes confusion on what each branch is attempting to achieve.
7. Not having clearly defined goals makes large tasks feel insurmountable.
 
Things we did well:
1. Adding tiers of achievement as milestones of success.
2. Having different experts in the room discuss the project in detail.
3. Data was well labelled and easy to access.
4. Paired programming was an enjoyable way to solve problems.
5. End-of-day show and tells were good motivators and good way to present completed work.
6. End-of-hackathon feedback on the experience was extremely useful in taking things forward.

So for the second hackathon:
- We did not split into teams but worked as one, large team.
- We set mandatory training which had to be attended by all hackathon participants - 3 events in total - and recorded the training.
- We used GitHub's project capabilities to set tasks in the form of GitHub issues and separate the issues by team.
- We added data for testing only.
- We limited the number of participants to a manageable number.
- We appointed a scrum master to oversee all activities during the hackathons.
- We appointed team leaders for each work stream (documentation, model, package).
- We developed a toolkit for all future hackathons (found [here](https://gstt-csc.github.io/guides.html#Hackathon-Planning/)).

<figure>
<img src="/assets/img/blog/Hackathon-pic-3.png" width="100%">
<figcaption>GitHub projects allow clear oversight of tasks and progress.</figcaption>
</figure>

As a result, the second hackathon was much more focussed and much better executed. The team, as a whole, achieved a silver medal, but the
collaboration this time was much easier due to clearly set out goals and team leaders delegating tasks within each domain. The benefit 
of a dedicated scrum master was that all participants knew who to ask questions, and the scrum master kept an eye on pull requests and new branches
reducing misunderstandings and work duplication.

Model team tested several methods to try and improve the model performance, eventually deciding that segmentation was needed. The documentation
team completed the hazard log after extensive risk assessments, added a literature review, added details to the proposal and clinical evaluation plan.
The package team built an AIDE-ready package that can be deployed once the model performance is improved.

<figure>
<img src="/assets/img/blog/Hackathon-pic-2.jpeg" width="100%">
<figcaption>End of day show and tell.</figcaption>
</figure>

# Future work
No progress can be made without some trial and error. In the two events we pushed both scaphoid fracture detection 
projects much farther than would otherwise be achieved within a year or so. We also learned a lot about collaboration, 
event organisation and model development. Work on both projects is still ongoing.

If you're organising a similar event, have a look at our [hackathon planning kit](https://gstt-csc.github.io/guides.html#Hackathon-Planning/).

