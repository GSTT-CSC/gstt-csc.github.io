---
layout: project_page
title: ScaphX
status: Current
image: /assets/img/projects/ScaphX-logo.png
summary: AI detection of scaphoid fractures in X-rays.
csc-lead: <a href="/team_member/Dika.html">Dika</a>, <a href="/team_member/Mike.html">Mike</a>
modality: X-ray
pathology: Occult scaphoid fracture
---
MRI imaging is superior in identification of occult carpal fracture, but is not always accessible. Imaging from X-rays can give suboptimal views, and the presentation of arthritis can make small fractures difficult to see. An AI tool to aid clinical diagnosis of occult carpal fractures using x-rays would increase diagnostic sensitivity in areas and situations where MRI is not available. 

A computer aided diagnosis tool which would automatically run when either a scaphoid fracture is suspected or if a patient is referred for a hand/wrist x-ray from A&E would increase sensitivity and confidence of diagnosis. Carpal fractures can be difficult to identify and patients with high clinical suspicion are put in a splint and referred to the fracture clinic even if a fracture isn’t seen on the x-ray by the clinician. Subtle lucency of an un-displaced fracture and the significance of a small bone fragment is currently easily missed. A successful tool would therefore increase diagnostic confidence and accuracy and reduce repeated x-rays and needless fracture clinic referrals
<br>
<br>
<b>Clinical lead</b>: Davina Mak <br>
<br>
<h3>Patient pathway</h3> 
A&E attendance with a suspected scaphoid fracture or hand/wrist injury.
<h3>Training data</h3> 
Training data for ScaphX consists of 3 separate datasets - a set of x-rays of the wrist used to train the scaphoid classifier which locates the scaphoid bone in the x-ray; of approximately 2000 Xrays which had follow up MRIs within two weeks of the injury used to reach definitive diagnosis; and of approximately 8000 Xrays which do not have a corresponding MRI.
<h3>Testing data</h3>
The testing data for ScaphX consists of approximately 1000 Xrays which are not a part of the training dataset and are held separately. 
<h3>Risks</h3> 
The biggest risks is a negative disruption to the clinical pathway if there are too many false positive results which lead to needless treatment.
<h3>Goals</h3>
The reduction of need for further imaging where fractures can be diagnosed from Xrays alone, improving the patient experience and reducing waste.
<h3>Success criteria</h3>
A reduction in negative wrist MRIs.
<h3>Alternatives</h3>
Commercial applications were considered to solve this clinical problem but were found to be optimised for `negatives` while the clinical pathway at GSTT can only benefit from an AI tool which is optimised for `positive` scans.
<br>
<h3>Additional resources</h3>
<a href="https://online.boneandjoint.org.uk/doi/full/10.1302/0301-620X.101B8.BJJ-2018-1590.R1"> TOHETI trial results </a><br>
<a href="https://journals.sagepub.com/doi/10.1177/17531934241312896"> A critical review of AI use in scaphoid fracture detection</a>

