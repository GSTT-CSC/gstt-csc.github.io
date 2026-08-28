---
layout: blogpost
title: "The Case for In-House Autocontouring" 
tag-line: "Why one size doesn't fit all for radiotherapy treatment planning"
date: "28 August 2026"
read-time-mins: "3 mins"
image: /assets/img/csc-logo-text.png
author: "Mike Woodward" 
author-image: /assets/img/team/Mike.jpg
author-role: "AI Development Lead & Senior Clinical Scientist in AI"
category: Article
---

<span class="dropcap">C</span>ontouring is a crucial component of patient care within the radiotherapy pathway, partly involving outlining the organs at risk to ensure that a treatment plan doesn’t deliver avoidable harmful doses of radiation to these critical regions. As you can imagine, manually performing this for each patient is a time intensive task , often performed by consultant clinicians, that is ripe for automation. However, the idea of this article isn’t to sell you on the value of autocontouring; I’ll let others do that. It was described as “game-changing” by the UK Government in 2024 to the point where they allocated [£15.5m for it to be rolled out to all NHS radiotherapy departments](https://www.gov.uk/government/news/ai-technology-to-help-cut-cancer-waiting-lists) and subsequently lead to outrage amongst clinicians now utilising the tools when this [funding was cut](https://www.theguardian.com/politics/2025/mar/31/ridiculous-cuts-to-ai-cancer-tech-funding-in-england-could-cost-lives-experts-warn?CMP=Share_iOSApp_Other). What I am looking to do, is sell you on the value of *in-house* autocontouring solutions.

Firstly, we control the data used to train the model. Despite published guidelines, contouring is surprisingly cultural. Conventions, such as where the brain stem ends and the spinal cord begins or even what counts as a distinct organ, can change from one centre to another. Commercial products cannot account for this whereas an inhouse solution can. Similarly, by training on scans that are from our trust, we can ensure that the model performs well for our population demographics and with our imaging equipment. Again, commercial products cannot guarantee this. Not only does this improve model performance based on raw metrics, but just as importantly, it builds trust from our clinicians. They see contours that are familiar while having complete knowledge of the data that was used to generate them.

Additionally, we can operate at pace. Once the data is collated we can train and have a model ready for deployment within 24 hours. While this is incredibly useful for quickly spinning up evaluations prior to full clinical deployment, the real value is found in rapidly updating models. Given new guidance or perhaps a recurring problem with a contour or even just changing the name of a contour our clinicians are not beholden to commercial release schedules. 

An in-house solution is arguably more robust in the long term due to avoiding vendor lock in. There is no risk of a sudden increase in costs making the solution no longer viable as a business case. Of course there are downsides here as well: you’re reliant on your own infrastructure and you now have a service to maintain, but for our department the positives outweigh these negatives.

It’s not just theoretical. Here at GSTT we have deployed three in-house developed autocontouring models currently in clinical use; pelvis & prostate, head & neck, and thoracic; between them covering thirty nine structures improving the care of over one thousand patients a year with incredible feedback from clinicians. There are numerous other models in the pipeline, with the most exciting among them being for cervical brachytherapy which could have a significant impact on the patient experience by potentially reducing the time patients spend undergoing treatment by up to an hour.

This approach works for us here at GSTT as we have the necessary ingredients. Where we not only have a dedicated [in-house team with the time, knowledge, and expertise to train complex models](https://gstt-csc.github.io/), but we also have the necessary infrastructure to facilitate these projects, from [access to GPUs](https://www.kcl.ac.uk/news/kings-and-nvidia-to-build-uks-first-al-platform) to a fully connected [deployment platform](https://deepc.ai/insight/deepc-and-the-ai-centre-for-value-based-healthcare). So, while advocating for this approach I appreciate that it may not be reproducible in all NHS trusts. However, if you are looking at setting up your own in-house autocontouring service or even just missing one or two pieces, we offer our expertise on a consultancy basis so please do [reach out if that is of interest](https://gstt-csc.github.io/get-in-touch.html). 

_Follow us on [LinkedIn](https://www.linkedin.com/company/gstt-csc/) for more updates on CSC activities._