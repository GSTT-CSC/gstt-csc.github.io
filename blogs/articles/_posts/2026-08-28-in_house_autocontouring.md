---
layout: blogpost
title: "The Case for In-House Autocontouring" 
tag-line: "Why one size doesn't fit all for radiotherapy treatment planning"
date: "28 August 2026"
read-time-mins: "3 mins"
image: /assets/img/blog/linac-large.jpg
author: "Mike Woodward" 
author-image: /assets/img/team/Mike.jpg
author-role: "AI Development Lead & Senior Clinical Scientist in AI"
category: Article
---
_Featured image: 'Inaugurazione Centro Radioterapia' by Università Campus Bio-Medico di Roma, licensed under [CC BY-NC-SA 2.0](https://creativecommons.org/licenses/by-nc-sa/2.0/deed.en)._ 

<span class="dropcap">C</span>ontouring is a crucial component of patient care within the radiotherapy pathway, partly involving outlining the organs at risk to ensure that a treatment plan doesn’t deliver avoidable harmful doses of radiation to these critical regions. As you can imagine, manually performing this for each patient is a time-intensive task, often performed by a consultant clinician, that is ripe for automation. However, the idea of this article isn’t to sell you the value of autocontouring; I’ll let others do that. Autocontouring has been described as 'game-changing' by the UK Government, who in 2024 [allocated £15.5 million](https://www.gov.uk/government/news/ai-technology-to-help-cut-cancer-waiting-lists) for it to be rolled out to all NHS radiotherapy departments. This [funding was subsequently cut](https://www.theguardian.com/politics/2025/mar/31/ridiculous-cuts-to-ai-cancer-tech-funding-in-england-could-cost-lives-experts-warn), leading to outrage amongst clinicians who were already utilising the tools. Rather, I'm hoping to persuade you of the value of *in-house* autocontouring solutions.

With autocontouring solutions, we control the data used to train the model. Despite what published guidelines suggest, contouring is surprisingly cultural. Conventions, such as where the brainstem ends and the spinal cord begins or even what counts as a distinct organ, can change from one centre to another. Commercial products cannot account for this, whereas an in-house solution can. By training on scans from our trust, we can also ensure that the model performs well for our population demographics and with our imaging equipment. Again, commercial products cannot guarantee this.

Not only does training the model on local data improve the model's performance based on raw metrics, but, just as importantly, it builds the trust our clinicians have in using the model. They see contours that are familiar while having complete knowledge of the data that was used to generate them.

Additionally, we can operate at pace. Once the data is collated, we can train and have a model ready for deployment within 24 hours. This is incredibly useful for quickly spinning up evaluations prior to full clinical deployment, but the real value is found in rapidly updating models. Given new guidance or perhaps a recurring problem with a contour, or even just changing the name of a contour, our clinicians are not beholden to commercial release schedules. 

An in-house solution is arguably more robust in the long term due to avoiding vendor lock-in. There is no risk of sudden increases in costs making the solution no longer viable as a business case. Of course, there are downsides here as well: you’re reliant on your own infrastructure and you now have a service to maintain. But, at least for our department, the positives outweigh these negatives.

It’s not just theoretical. Here at GSTT we have deployed three in-house-developed autocontouring models into clinical use: pelvis and prostate, head and neck, and thoracic. Together, their use covers 39 structures and improves the care of over 1000 patients a year, with incredible feedback from clinicians. 

There are numerous other models in the pipeline, too, with the most exciting among them being for cervical brachytherapy. The introduction of this model could have a significant positive impact on the patient experience by reducing the time each patient spends undergoing treatment by up to an hour.

One caveat. The in-house approach works for us at GSTT because we have the necessary ingredients. We not only have a dedicated [in-house team](https://gstt-csc.github.io/) with the time, knowledge, and expertise to train complex models, but we also have the necessary infrastructure to facilitate these projects, from [access to GPUs](https://www.kcl.ac.uk/news/kings-and-nvidia-to-build-uks-first-al-platform) to a fully connected [deployment platform](https://deepc.ai/insight/deepc-and-the-ai-centre-for-value-based-healthcare). So, while I have been fully advocating for this approach, I appreciate that it may not be reproducible in all NHS trusts. 

That being said, if you are looking to set up your own in-house autocontouring service, or if you are missing just one or two of the pieces in order to do so, we offer our expertise on a consultancy basis. If that is of interest to you, please do [reach out to us](https://gstt-csc.github.io/get-in-touch.html). 

_Follow us on [LinkedIn](https://www.linkedin.com/company/gstt-csc/) for more updates on CSC activities._