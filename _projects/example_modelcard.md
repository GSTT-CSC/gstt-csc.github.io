---
layout: modelcard
title: Modelcard layout test
devicename: ScaphX
status: Developing
image: /assets/img/projects/xray_carpel.jpg
sex_graph: /assets/img/projects/ScaphX_sex_graph.png
ethn_graph: /assets/img/projects/ScaphX_ethn_graph.png
age_graph: /assets/img/projects/ScaphX_age_graph.png
summary: ScaphX offers real-time decision support for the detection of scaphoid fractures. The application interprets wrist x-rays to increase the accuracy and confidence of diagnosis, enabling rapid turnaround treatment with discharge or appropriate further management of these patients.
modality: X-ray
model: MODEL
pathology: PATHOLOGY
rationale: MRI imaging is superior in identification of occult carpal fracture, but is not always accessible. Imaging from X-rays can give suboptimal views, and the presentation of arthritis can make small fractures difficult to see. An AI tool to aide clinical diagnosis of occult carpal fractures using x-rays would increase diagnostic sensitivity in areas and situations where MRI is not available. A computer aided diagnosis tool which would automatically run when either a scaphoid fracture is suspected or if a patient is referred for a hand/wrist x-ray from A&E would increase sensitivity and confidence of diagnosis. Carpal fractures can be difficult to identify and patients with high clinical suspicion are put in a splint and referred to the fracture clinic even if a fracture isn’t seen on the x-ray by the clinician. Subtle lucency of an un-displaced fracture and the significance of a small bone fragment is currently easily missed. A successful tool would therefore increase diagnostic confidence and accuracy and reduce repeated x-rays and needless fracture clinic referrals.
patient-pathway: PATHWAY
training-data: Training data was collected using CogStack at GSTT.
train_data_excl: Images with no carpal bones and images with multiple fused views were deleted. Images with poor quality and artefacts were noted but not eliminated from the dataset.
train_input: Images
train_size: 1444
errors: ERRORS
goals: GOALS
success-criteria: CRITERIA

alternatives: <a href="http://www.gleamer.ai/">Gleamer</a>, which specialise in trauma x-rays, has been considered for this purpose but was decided not suitable to solve this particular clinical problem. The decision was made to train an in-house algorithm instead.




---

**Project Plan** <br>
<strike>1.	Meeting of all persons involved to determine AI specifications. <br><br> 2.	Setting technical and system requirements for AI model. </strike> <br> 3. Dataset curation (retrospective). <br><br> 4.	Model training<br><br>5.	Model testing <br><br>6.	Implementation <br><br>7. Audit
<br>
<br>
<b>References</b>:<br> <a href="https://online.boneandjoint.org.uk/doi/full/10.1302/0301-620X.101B8.BJJ-2018-1590.R1"> TOHETI trial results </a>