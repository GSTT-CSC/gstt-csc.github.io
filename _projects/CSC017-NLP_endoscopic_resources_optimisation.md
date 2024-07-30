---
layout: project_page
title: NLP for optimisation of endoscopic resources
status: Reporting
image: /assets/img/blog/nhs_logo.png
summary: Natural Language Processing of Endoscopic and associated pathology text to optimise post COVID endoscopy resources
csc-lead: <a href="team_member/Agathe.html">Agathe</a>
modality: Endoscopy, EPR
pathology: Premalignant disease of the upper gastrointestinal tract
rationale: Patients with premalignant disease of the upper gastrointestinal tract need to undergo regular endoscopic surveillance to prevent malignancy. The timing of endoscopic procedures is often inaccurate and many patients are either surveyed endoscopically late or inappropriately which becomes a healthcare resource burden. Using natural language processing to automatically caluclate follow up timings based on information in the EPR system
patient-pathway: The model will interpret endoscopy notes to determine the most appropriate follow up booking date. The practical output would be a spreadsheet containing the endoscopy and associated pathology report along with the extracted information of interest and a suggested follow up timing. In the first instance the spreadsheet would be passed to a manual vetter as a final check on the output prior to bookings being made
training-data: Endoscopy and Pathology reports from EPR. Synthetic dataset used to date for proof of concept.
errors: Patient may be given inappropriately early/late follow up exam
goals: Optimise available endoscopy resources by refining booking process for patient follow up exams
success-criteria: 1. Reduction in the number of endoscopies done inappropriately early. <br><br> 2. Reduction in the number of endoscopies performed too late (?with decrease in missed early cancer rate). <br><br> 3.	Reduction in patients lost to follow up 
alternatives: N/A
---
The current COVID pandemic has lengthened the waiting list for endoscopic surveillance for premalignant disease such that some patients may develop malignancy whilst waiting for endoscopy. Similarly, by booking follow up endoscopy too early for patients, scarce healthcare resources are being used inappropriately. This risk could be offset by a rigorous guideline based assessment of patients on the waiting list for assessment so that patients who have been planned to be endoscoped too early, or inappropriately can be planned more appropriately. To do this endoscopy and pathology free text reports need to be analysed for patients on the waiting list. The decision about the timing of follow up endoscopy depends on the natural language information contained within both sets of reports. Because of the number of patients, the aim of the current study is to automate the analysis using natural language processing.
<br>
<br>
<b>Clinical lead:</b> Sebastian Zeki 
<br>
<br>
<b>Project Plan</b><br>
1.<strike>Meeting of all persons involved to determine AI specifications. <br><br> 2.	Setting technical and system requirements for AI model. <br> <br> 3. Dataset curation (retrospective). <br><br> 4.	Model training<br><br>5.	Model testing <br><br></strike>6.	Implementation <br><br>7. Audit 
<br>
<br>
<b>References</b> 