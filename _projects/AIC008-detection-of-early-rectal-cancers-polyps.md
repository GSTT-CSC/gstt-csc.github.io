---
layout: project_page
title: Early detection of rectal cancer
status: Data Curating
image: /assets/img/roadmap/polyps.jpg
summary: An application that identifies areas of concern on MRI images for the detection of rectal cancers/polyps
csc-lead: <a href="/team_member/Laurence.html">Laurence</a>
modality: MRI
pathology: Rectal cancer/polyps
rationale: Development of an AI tool to identify areas of concern that may indicate early development of cancer and polyps in rectal MRI images
patient-pathway: Once a lesion is identified whether these abnormalities are cancerous or polyps the ultimate treatment for this is removal which is curable if performed early.
training-data: Large MRI pelvis dataset within the trust with the T2 weighted axial and diffusion performed in most cases. This will give a high yield of normal. Rectal cancer datasets also collected via a recent audit.
errors: False positives will either result in early interval repeat imaging or proctoscopy performed by surgeons in clinic/endoscopy. False negative may result in cancers being detected at a later stage.
goals: An application that is able to identify areas of concern for further analysis by radiologists
success-criteria: Ability to identify lesions incidentally/early leading to improved outcomes for patients, early detection leads to stopping/reducing the development of malignancy which can be fatal when diagnosed at a late stage. 
alternatives: Currently no commercial products identified
---
MRI pelvis studies are reported by a variety of subspecialty radiologists leading to missed pathology in the rectum outside of the reporter’s immediate comfort zone. The consequence of a missed polyp is the development of later stage cancerous lesions which are more symptomatic and potentially incurable or require extensive surgery/treatment as oppose to minimally invasive endoluminal procedures. An artificial intelligent algorithm has the potential to reduce these errors by highlighting areas of concern particularly within the rectum which can be a challenging area to assess.
<br>
<br>
<b>Clinical lead</b>: Tina Mistry <br>
<br>
**Project Plan**

**Initial Meeting**<br>
   1. Meeting of all persons involved to determine AI specifications <br>

**Setting technical and system requirements for AI model**<br>
   1. Agree on most useful metrics for success – e.g. percentage reduction in missed polyps. This will require designing a fixed methodology for measuring currently missed polyps which can be performed before and after model deployment.<br>
   2. Agree on minimum valuable requirements for success e.g. 25% reduction in missed polyps. We are aiming for a 10% reduction in missed polyps using the methodology above.<br>
   3. Agree on size of POC and production datasets and who is responsible for compiling them. We will use existing database of 5 year audit to generate proof-of-concept dataset <br>
   4. Agree on how model will be deployed. The application will push information back to radiologist workstation to indicate suspect dicom series as well as slice number and region <br>

**Development phase (proof of concept (POC)**
   1. Dataset curation (retrospective)
   2. Model training 
   3. Produce effective POC model
   4. Model testing
   5. Test model against agreed criteria for success (where applicable)
   6. Agreement to continue to production phase OR iterative/improve model OR discontinue

**Development phase (production)**
5. Dataset curation (retrospective). Compile larger production dataset with all appropriate data properties (e.g. ethnicity, weight etc)
6. Model training. Produce effective deployment model
7. Model testing 
8. Test model against agreed criteria for success (where applicable). 
9. Clinical approval for model to be deployed

**Deployment phase**
8. Deployment to test environment (if applicable)
9. Deployment to hospital systems including training for users and continuous monitoring of model performance

<b>References</b><br>
   Lee, Joohyung, et al. "Reducing the model variance of a rectal cancer segmentation network." IEEE Access 7 (2019): 182725-182733. [online](https://arxiv.org/pdf/1901.07213.pdf)