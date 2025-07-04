---
layout: project_page
title: PERT  
status: On hold
image: /assets/img/projects/pert_image_wikipedia.png
summary: AI detection & classification of high-risk PE.
csc-lead: <a href="/team_member/Anil.html">Anil</a>
modality: CT Pulmonary Angiogram (CTPA)
pathology: Pulmonary Embolism
---
---

This project is currently on hold due to resource and capacity issues and prioritisation of a different AI product. It will be picked up again soon. 

---

The Pulmonary Embolism Response Team (PERT) comprises Interventional Radiologists, Haematology consultants, 
Cardiothoracic surgeons, and Respiratory consultants,  

Both patients arriving at GSTT, and in patients, with suspected High risk or intermediate-high risk PE will alert the 
PERT to allow multi-disciplinary decisions to be made for management, triage and treatment.
Reduction in the time to alert PERT of high-risk PE can result in reduced length of stay, morbidity and improved patient outcomes from MDT decisions.

<b>Clinical lead</b>: Narayan Karunanithy, Karen Breen
<br>
<h3>Rationale</h3>
Triggering PERT, if the patient is not high risk, may benefit intermediate-high risk patients, however the speed of results to assign that risk category to a patient could cause delays in triggering that alert. An AI application is being evaluated to automatically pull CTPA images and calculate the right ventricular/left ventricular (RV/LV) ratio as a good indicator of right heart strain, to risk stratify patients above a certain threshold as appropriate to alert the PERT, therefore speeding up the CTPA reporting and subsequent PERT engagement towards better patient outcomes. 
<br>
<h3>Patient pathway</h3>
<img src='/assets/img/projects/Pert_diagram_1.png' width="100%" alt="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9504600/">

<h3>Testing data</h3>
Approximately 4000 labelled CTs have been identified for retrospective testing of the commercial solution. Prospective trial will follow after if retrospective study demonstrates sufficient accuracy.
<h3>Goals</h3> Automated classification of high and intermediate-high risk PE patients by accurately calculating Right Heart Strain (RV/LV ratios) from CTPAs. 
<h3>Success criteria</h3> Improvement in diagnostic accuracy and speed. Increased identification of intermediate risk patients alerting the PERT.

<h3>References</h3>
<a href="https://doi.org/10.1007/s00330-022-08645-2"> Cheikh et al 2021</a><br>
<a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3718593/"> Bĕlohlávek et al 2013 </a><br>
<a href="https://doi.org/10.1002/rth2.12216"> Rosovsky et al 2018 </a>