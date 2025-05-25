---
layout: project_page
title: AI fairness
status: Current
image: /assets/img/blog/racial_bias.jpg
summary: AI fairness toolkit for bias checking.
csc-lead: <a href="/team_member/dika.html">Dika</a>
modality: N/A
pathology: N/A
---

In our mission to deploy safe and well-tested AI, we have been discussing the topics of fairness since our inception in 2020. 
The guidance thus far published on bias mitigation in AI and addressing health disparities through digital solutions lacks practical instruction. While we appreciate the importance of diversity in data, validation and developer teams, we find it difficult to benchmark at what point these aims can be considered achieved. 

Moreover, we found that fairness metrics often address individual attributes independently of healthcare context and without intersectional analysis, focusing on equality in terms of sample numbers only. This partly stems from the intuition to address health disparities through the lens of the protected characteristics (Equality Act 2010). These do not account for societal factors (e.g. poverty, literacy), 
which play defining roles in healthcare outcomes and are the leading causes of health disparities globally. 
Guidance also champions transparency on training and testing data by encouraging publication of communication tools such as model cards, similar in nature to information leaflets produced for medications. However, the guidance does not address how this information can be interpreted by clinicians considering implementation of AI products when a patient is not demographically represented in AI model data. 

The end outcome is that results of clinical AI evaluations are difficult to interpret and difficult to communicate, increasing the potential for harm, which reinforces the need for effective methodologies to detect and mitigate bias. We have faced this problem when both developing and evaluating AI solutions.  

In this project, we aim to develop and implement an open-source toolkit which can analyse AI evaluation results for fairness and bias.  

The toolkit will give context-driven mitigation advice supported by robust statistical testing, 
ensuring that the AI models are reaching conclusions based on pathology-only, and not patient characteristics which affect healthcare outcomes and navigation of the clinical pathways. 

<h3>AI Fairness NHS Working Group</h3>
This mission has led to the creation of the AI Fairness Working Group which is working on both the toolkit mentioned here and a few other projects. More can be found on the [AI Fairness NHS Working Group website](https://www.aifairness.co.uk/). 
 