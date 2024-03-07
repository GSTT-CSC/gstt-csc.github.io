---
layout: project_page
title: X-Ray Occult Carpal Detection
status: Developing
image: /assets/img/projects/xray_carpel.jpg
summary: A computer aided diagnosis tool which would automatically run when a scaphoid fracture is suspected.
csc-lead: <a href="/team_member/Dika.html">Dika</a>
modality: X-ray
pathology: Occult carpal fractures (wrist and hands)
rationale: MRI is superior in identification of occult carpal fracture, but is not always accessible. An AI tool to aide clinical diagnosis of occult carpal fractures using x-rays would increase diagnostic sensitivity in areas and situations where MRI is not available.
patient-pathway: A&E attendance with a suspected scaphoid fracture or hand/wrist injury.
training-data: Patient cohort identified using CogStack looking for phrases 'scaphoid' and 'MRI clinical'. The query generated a list of approximately 1000 patients who have had an MRI, with the view that all patients who had an MRI will also have had an x-ray. The patient list is now being stratified to `test`, `control` and `back-up` groups.
errors: Needless referrals to fracture clinic and needless immobilisation in patients who do not have a fracture; repeated x-rays; referrals to MRI.
goals: An automated computer aided diagnosis tool triggered when appropriate x-rays are taken.
success-criteria: Improvement in diagnostic accuracy and diagnostic speed.
alternatives: <a href="http://www.gleamer.ai/">Gleamer</a>, which specialise in trauma x-rays, has been considered for this purpose but was decided not suitable to solve this particular clinical problem. The decision was made to train an in-house algorithm instead
---
MRI imaging is superior in identification of occult carpal fracture, but is not always accessible. Imaging from X-rays can give suboptimal views, and the presentation of arthritis can make small fractures difficult to see. An AI tool to aide clinical diagnosis of occult carpal fractures using x-rays would increase diagnostic sensitivity in areas and situations where MRI is not available. 
A computer aided diagnosis tool which would automatically run when either a scaphoid fracture is suspected or if a patient is referred for a hand/wrist x-ray from A&E would increase sensitivity and confidence of diagnosis. Carpal fractures can be difficult to identify and patients with high clinical suspicion are put in a splint and referred to the fracture clinic even if a fracture isn’t seen on the x-ray by the clinician. Subtle lucency of an un-displaced fracture and the significance of a small bone fragment is currently easily missed. A successful tool would therefore increase diagnostic confidence and accuracy and reduce repeated x-rays and needless fracture clinic referrals
<br>
<br>
<b>Clinical lead</b>: Davina Mak <br>
<br>
**Project Plan** <br>
<strike>1.	Meeting of all persons involved to determine AI specifications. <br><br> 2.	Setting technical and system requirements for AI model. </strike> <br> 3. Dataset curation (retrospective). <br><br> 4.	Model training<br><br>5.	Model testing <br><br>6.	Implementation <br><br>7. Audit
<br>
<br>
<b>References</b>:<br> <a href="https://online.boneandjoint.org.uk/doi/full/10.1302/0301-620X.101B8.BJJ-2018-1590.R1"> TOHETI trial results </a>