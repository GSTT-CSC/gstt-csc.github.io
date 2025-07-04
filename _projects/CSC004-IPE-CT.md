---
layout: project_page
title: IPE
status: Current
image: /assets/img/projects/lung_pe.jpg
summary: AI for detection of PEs in CTs.
csc-lead: <a href="/team_member/Anil.html">Anil</a>
modality: Contrast-enhanced CT
pathology: Pulmonary embolism

---
A pulmonary embolism (PE) is a blockage in one of the pulmonary arteries in the lungs, often caused by blood clots that travel from elsewhere in the body. It commonly affects individuals with risk factors such as prolonged immobility, surgery, cancer, or clotting disorders. There is an opportunity to find PEs when patients undergo lung imaging for other reasons (incidental pulmonary embolism findings, IPE). This can potentially reduce the time from incidental finding to dedicated imaging and treatment, preventing further clinical complications.
<br>
<br>
<b>Clinical lead</b>: Dr. Jacques Audrey <br>
<br>
<h3>Rationale</h3> 
Incidental PEs can be found faster with automated analysis of all suitable lung CT images acquired in the radiology department. A dedicated AI tool 

<h3>Patient pathway</h3> 
Patients present to radiology for a number of other conditions wherein lung imaging with contrast CT is needed. This solution will affect multiple clinical pathways.

<h3>Testing data</h3> 
Retrospective evaluation was completed on 5000 chest CTs (accounting for the 2% expected prevalence of IPEs in patient population). Sufficient accuracy was demonstrated (findings published [here](https://onlinelibrary.wiley.com/doi/10.1155/rrp/9091895)). The prospective trial was commenced in spring 2025 and is currently still ongoing.

<h3>Risks</h3> 
High number of false positives will lead to alert fatigue and eventual ignoring of the highlighted AI result. Both AI and clinical staff missing a PE, resulting in a loss of opportunity to treat early. Clinicians eventually relying on AI results only. Financial risks also implied as the solution being tested is a commercial product.

<h3>Goals</h3> 
All CTs containing lung region with sufficient contrast are screened with AI to identify PEs and highlight this finding to the reporting radiologist. The goal is to prioritise reporting based on this finding so CTs where PEs are suspected are reported first.

<h3>Success Criteria</h3>
Quicker turnaround time in IPE findings compared to current benchmark, and prevention of missed opportunity for early treatment.

<b>References</b> <br> 
[Computer Aided Detection of Pulmonary Embolism Using Multi-Slice Multi-Axial Segmentation](https://doi.org/10.3390/app10082945)<br>
[Automated detection of pulmonary embolism in CT pulmonary angiograms using an AI-powered algorithm](https://doi.org/10.1007/s00330-020-06998-0)<br>
[Independent Evaluation of a Commercial AI Software for Incidental Findings of Pulmonary Embolism (IPE) on a Large Hospital Retrospective Dataset](https://onlinelibrary.wiley.com/doi/10.1155/rrp/9091895)<br>