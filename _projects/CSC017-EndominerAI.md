---
layout: project_page
title: EndominerAI
status: Current
image: /assets/img/projects/EndoMinerAi_Logo.png
summary: NLP for surveillance scan scheduling.
csc-lead: <a href="team_member/Agathe.html">Agathe</a>
modality: Endoscopy, EPR
pathology: Premalignant disease of the upper gastrointestinal tract
---
The COVID pandemic had lengthened the waiting lists for endoscopic surveillance for premalignant disease such that some patients may develop malignancy whilst waiting for endoscopy. Similarly, by booking follow up endoscopy too early for patients, scarce healthcare resources are being used inappropriately. This risk could be offset by a rigorous guideline based assessment of patients on the waiting list for assessment so that patients who have been planned to be endoscoped too early, or inappropriately, can be planned more appropriately. To do this endoscopy and pathology free text reports need to be analysed for patients on the waiting list. The decision about the timing of follow up endoscopy depends on the natural language information contained within both sets of reports. Because of the number of patients, the aim of the current study is to automate the analysis using natural language processing.

This project led to the creation and clinical deployment of the first of the set of models within EndominerAI suite. The accuracy of the developed tool has been consistently demonstrated to be around 98%, tested on GSTT, KCH and Birmingham data. The project is currently awaiting integration with the EHR system.
<br>
<br>
<b>Clinical lead:</b> Sebastian Zeki 
<br>
<h3>Rationale</h3> 
Patients with premalignant disease of the upper gastrointestinal tract need to undergo regular endoscopic surveillance to prevent malignancy. The timing of endoscopic procedures is often inaccurate and many patients are either surveyed endoscopically late or inappropriately which becomes a healthcare resource burden. Using natural language processing to automatically caluclate follow up timings based on information in the EPR system
<h3>Patient pathway</h3> 
The model will interpret endoscopy notes to determine the most appropriate follow up booking date. The practical output would be a spreadsheet containing the endoscopy and associated pathology report along with the extracted information of interest and a suggested follow up timing. In the first instance the spreadsheet would be passed to a manual vetter as a final check on the output prior to bookings being made
<h3>Training data</h3> 
Endoscopy and Pathology reports from EPR. Synthetic dataset used to date for proof of concept.
<h3>Risks</h3> 
Patient may be given inappropriately early/late follow up exam
<h3>Goals</h3>
Optimise available endoscopy resources by refining booking process for patient follow up exams
<h3>Success criteria</h3> 
1. Reduction in the number of endoscopies done inappropriately early.
2. Reduction in the number of endoscopies performed too late (?with decrease in missed early cancer rate).
3. Reduction in patients lost to follow up. 
<h3>Alternatives</h3> 
None identified.
<br>
<h3>References</h3> 
[Automated decision making in Barrett’s oesophagus: development and deployment of a natural language processing tool by Zecevic et al](https://www.nature.com/articles/s41746-024-01302-6)