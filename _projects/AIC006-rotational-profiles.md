---
layout: project_page
title: Rotational Profiles
status: Developing
image: /assets/img/blog/nhs_logo.png
summary: An AI tool to measure degrees of misalignment of lower limb rotation in pre-surgical planning assessments .  
csc-lead: <a href="/team_member/Anil.html">Anil</a>
modality: CT Scans 
pathology: Lower limb rotation
rationale: Assessment of rotational profiles is time consuming and complex. An AI algorithm would significantly decrease the amount of time needed to measure the angles of rotation.
patient-pathway: Patients are referred by the orthopaedic team. CT imaging is part of the pre-surgical work up. The report is used to plan the surgical intervention.
training-data: Over 100 patients are referred annually. The data will be retrospective, acquiring a large cohort of patients and segmentation and profile results as annotated on PACS. It is possible annotations will need to be re-done if they cannot be exported from PACS.
errors: The tool is to help find the accurate rotational profile and will be supervised and signed off by the radiologist, so an error is unlikely to persist far enough to affect a patient.
goals: Reduction of radiologist time in reporting these scans as well as increase consistency in calculation.
success-criteria: Accurate, automated rotational profiles.
alternatives: Currently no commercial products identified
---

Current practice of manually drawing lines over the long bones and the joints on CT images in PACS to figure the degree of misalignment is time-consuming (15-20 minutes per case). An AI tool would automatically create these lines and angles, saving time and reducing variability.


<b>Clinical lead(s)</b>: Dr. Christopher Tang <br>
<br>
**Project Plan**
<br> <b> <strike> 1. Meeting of all persons involved to determine AI specifications.</b> <br><br> For radiologist (Chris) :<br> - Confirm +/3 to 5 degree precision with peers<br> - Confirm with surgeons how angles are used to guide knee surgery <br> - Confirm 3 bone ankle slice is the correct slice to analyse.<br>- Review software requirements spec <br> <br><b>2.	Setting technical and system requirements for AI model.</b><br><br> For CSC (Anil) <br>  -  Perform the risk assessment<br> - Create software design spec from software requirements spec <br> - Attempt to build non-A.I software with “dicom_server” and eventually “AI Deployment Engine” <br> - Investigate the AI route<br><br><b> 3. Dataset curation (retrospective). </b><br><br> - Collect Patient ID’s for 100-200 patients, analysed by different radiologists<br><br> </strike> <b>4.	Model training</b><br><br> <b>5.	Model testing</b> <br><br><b>6.	Implementation</b> <br><br>
<b>7. Audit </b> 
<br>
<br>
<b>References</b>:  Website used to help calculate rotational angles is <a href="http://uwmsk.org/legrotation.html"> here</a>. |

