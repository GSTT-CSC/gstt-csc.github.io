---
layout: blogpost
title: "My Eight-Week Internship with CSC" 
tag-line: "Maame joined CSC through an internship organised by Health Data Research UK"
date: "23 September 2026"
read-time-mins: "2 mins"
image: /assets/img/blog/London_Bridge.jpg
author: "Maame Owusu-Ansah" 
author-image: /assets/img/blog/Maame-Owusu.jpg
author-role: "HDR UK Intern"
category: Blog
---
_Featured image: Thomas Karagiannis, Pexels._

_Maame is a PhD student who works on deep learning for medical image analysis, with a focus on cardiac imaging. Maame joined CSC for eight weeks as an intern on the Health Data Science Black Internship Programme, [class of 2026](https://www.hdruk.ac.uk/study-and-train/health-data-science-black-internship-programme/class-of-2026/). This was organised by [Health Data Research UK (HDR UK)](https://www.hdruk.ac.uk/)._

<span class="dropcap">I</span> came into the internship from a background working on coronary artery segmentation, so I arrived expecting to spend the summer on models: architectures, loss functions, evaluation metrics. That is not what happened, and I am glad it is not.

Before starting with Clinical Scientific Computing (CSC), I set out a few goals:
1.	Understand how CSC turns a research model into something deployable in a clinical pathway.
2.	Learn how a quality management system works day to day, rather than as an abstraction.
3.	Contribute something to a repository that someone would use after I left.
4.	Get better at working in a codebase I did not write.

I collaborated with [Mike](/team_member/mike.html) and [Keri](/team_member/keri.html) on the [AutoSegCT](/blogs/articles/article/2026/09/01/in_house_autocontouring.html) and [quality management system (QMS)](/blogs/articles/news/2026/01/01/QMS_press_release.html) automation projects. AutoSegCT is an AI tool that automates the process of outlining organs at risk for radiotherapy treatment planning. It has been clinically deployed, and it is regulated as a Class IIa medical device. The team are developing automated checks to confirm that their projects' documentation complies with QMS requirements.

The first thing I learned was that developing the model is not the hard part, having the documentation is. For every project there is a hazard log, a list of device record requirements, and a set of test records, all held as YAML files under version control, and if those are incomplete or inconsistent the tool cannot be released, however good the segmentations are.

During this time, the overall project was being restructured so that each segmentation model counted as its own device, with its own documentation set. This raised an immediate practical question: how do you know whether the 30-odd YAML files across three models are accurate and up to date? At the time, somebody manually opened each file, read it, and checked it.

So, I wrote a script to automate this process. This script uses PyYAML and Pydantic to walk the documentation directory, find every model, and check each file against what the QMS requires. Are the fields present? Are they filled in, rather than being blank or stating ‘TBC’? Are the values drawn from the permitted scales? The script writes a markdown report naming the field, what it found, and what it expected.

I also spent time in [David](/team_member/david.html)’s branch, which validates the same files using Pydantic, and adapted the reporting so that the output is something a project lead can act on rather than a stack trace.

The most useful thing the script found was not something I went looking for. The project template had not been updated to match the current clinical risk management standard, so new projects were starting with an outdated risk matrix. That is not a bug in anyone’s code. It is the kind of gap that only appears when you check documents against the standard automatically.

I met three of my four goals. The fourth, working comfortably in someone else’s codebase, I am partway through. I am extremely grateful to CSC for the opportunity. I learned a lot!

_Follow us on [LinkedIn](https://www.linkedin.com/company/gstt-csc/) for more updates on CSC activities._