---
layout: project_page
title: Dental Disease Classifier  
status: On hold
image: /assets/img/projects/dental_tomograph_wikipedia.jpg
summary: AI disease detection & classification.
csc-lead: <a href="/team_member/Mike.html">Mike</a>
modality: Dental radiograph
pathology: Jaw tumours and cysts
---
---

This project is currently on hold. The AI model has been trained and demonstrates good performance, but significantly more clinical time must now be invested to evaluate the product before it can be deployed.

---

Dental panoramic tomograms (DPTs) are common radiographs performed as first-line imaging for a broad range of maxillofacial disease. Within both primary and secondary care, DPTs are interpreted by the requesting dentist, typically without input from a specialist in dental and maxillofacial radiology (DMFR). Specialist reporting is not currently commissioned by the NHS and there are less than 30 registered DMFR specialists nationally, so there is limited scope for second opinion within primary care. Published service evaluations indicate that DPTs referred for specialist opinion contain diagnoses ranging from normal anatomy to malignancy, suggesting that confidence in interpreting DPTs is variable for non-specialists.

DPTs are particularly prone to incidental findings and technical errors, which can obscure interpretation and contribute to misdiagnosis. In some cases, this can lead to missed diagnosis of significant disease, including radiological findings suspicious for malignancy, which leads to delays in appropriate management and subsequent reduced patient outcomes. 

A deep learning tool would be clinically useful if it could improve the diagnostic accuracy or efficiency of DPT interpretation by the reporting clinician. Useful output would include differentiation between normal variation and disease. Of the DPTs showing disease, flagging the ROI and suspected clinical behaviour of the lesion (e.g. developmental condition/cyst/benign tumour/malignant tumour) is likely to be more useful than outputting a specific diagnosis. This would assist in workflow prioritisation of time-critical disease e.g. specialist reporting of DPTs with suspected malignancy to streamline appropriate referral from primary to secondary care. The technology would be used by non-specialist clinicians to improve diagnostic accuracy, and could be used by specialist clinicians to improve efficiency. 

<b>Clinical lead</b>: Bethan Thomas <br>

<h3>Rationale</h3> 
DPTs are particularly prone to incidental findings and technical errors, which can obscure interpretation and contribute to misdiagnosis.
<h3>Patient pathway</h3> 
Within both primary and secondary care, DPTs are interpreted by the requesting dentist, typically without input from a specialist in dental and maxillofacial radiology (DMFR). Specialist reporting is not currently commissioned by the NHS.
<h3>Training data</h3>
Approximately 300 DPTs were labelled and used for training of the AI algorithm. The evaluation in clinic has not yet been undertaken.
<h3>Risks</h3> 
In cases of missed diagnosis of significant disease, including radiological findings suspicious for malignancy, the the result is delays in appropriate management and subsequent reduced patient outcomes. 
<h3>Goals</h3> 
Detect and classify a range of dental lesions.
<h3>Success criteria</h3> 
Improvement in diagnostic accuracy and diagnostic speed.
<h3>Alternatives</h3> 
Currently no commercial products identified 