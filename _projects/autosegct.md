---
layout: project_page
title: Radiotherapy Auto Segmentation
status: Evaluating
image: assets/img/projects/autosegct_logo.png
summary: Single application for all inhouse autosegmentation contours
csc-lead: <a href="/team_member/Anil.html">Anil Mistry</a> <a href="/team_member/Tom.html">Tom Roberts</a>
modality: Radiotherapy planning CT 
pathology: Cancer
rationale: Contouring organs on CT's scans for radiotherapy treatments is vital for patient safety, however is very time consuming for Oncologists. AI models have been developed locally to automate the CT image segmentation. 
patient-pathway: 
training-data: Gold standard dual-labelled CT's and structure sets of patients treated historically at Guy's Cancer Centre. 
errors:  N/A
goals:  Provide an application that can integrate the 
success-criteria: Improvement in diagnostic accuracy and speed. Increased identification of intermediate risk patients alerting the PERT.
---

<b>Clinical lead</b>: Christopher Thomas, Teresa Guerrero Urbano
<br>
<br> **Rationale:**

AI auto-contouring tools have improved dramatically in the last few years, and all major treatment planning system vendors are investing in this technology along with independent start-ups and NHS Trusts [NICE, 2023].

GSTT are in a strong position to develop our own auto-contouring pipeline using the AI expertise within RT physics, clinical oncology, and the Clinical Scientific Computing (CSC) team, strong links with King’s College London (KCL) academics and outputs from three KCL PhD students creating AI auto-contouring models.


<b>Project Plan</b>: 

1. **Proposal**
2. **Requirements gathering** 
3. **Clinical Risk management**
4. **Design Specification creation**
5. **Development**
6. **Soft deployment**
6. **Retrospective evaluation** 
7. **Prospective Evaluation**
8. **Training**
9. **Clinical Go Live**

<br>
<br>
<b>References</b>: 
<br><br>
### Academic papers

| Year | Authors                 | Title                                                                                                                                                    | Link                                                          | Key points |
|------|-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|------------|
| 2023 | K. Mackay et al         | A Review of the Metrics Used to Assess Auto-Contouring Systems in Radiotherapy                                                                           | https://doi.org/10.1016/j.clon.2023.01.016                    |            |
| 2022 | Mody, Prerak et al      | Improving Error Detection in Deep Learning Based Radiotherapy Autocontouring Using Bayesian Uncertainty                                                  | https://link.springer.com/chapter/10.1007/978-3-031-16749-2_7 |            |
| 2023 | Kareem A Wahid et al    | Evolving Horizons in Radiotherapy Auto-Contouring: Distilling Insights, Embracing Data-Centric Frameworks, and Moving Beyond Geometric Quantification    | https://pubmed.ncbi.nlm.nih.gov/37904737/                     |            |
| 2023 | S M Hasibul Hoque et al | Clinical Use of a Commercial Artificial Intelligence-Based Software for Autocontouring in Radiation Therapy: Geometric Performance and Dosimetric Impact | https://doi.org/10.3390/cancers15245735                       |            |
| 2023 | Hana Baroudi  et al     | Automated Contouring and Planning in Radiation Therapy: What Is ‘Clinically Acceptable’?                                                                 |                                                               |            |
| 2023 | Paul J. Doolan et al    | A clinical evaluation of the performance of five commercial artificial intelligence contouring systems for radiotherapy                                  | https://doi.org/10.3389/fonc.2023.1213068                     |            |
| 2023 | NICE guidelines         | Artificial intelligence technologies to aid contouring for radiotherapy treatment planning: early value assessment                                       | www.nice.org.uk/guidance/hte11                                |            |
| 2023 | Yasmin McQuinlan et al  | An investigation into the risk of population bias in deep learning autocontouring                                                                        | https://doi.org/10.1016/j.radonc.2023.109747                  |            |
| 2023 | S. Hindocha et al       | Artificial Intelligence for Radiotherapy Auto-Contouring: Current Use, Perceptions of and Barriers to Implementation                                     | https://doi.org/10.1016/j.clon.2023.01.014                    |            |
| 2021 | Weihua Mao et al        | Evaluation of Auto-Contouring and Dose Distributions for Online Adaptive Radiation Therapy of Patients With Locally Advanced Lung Cancers                | https://doi.org/10.1016/j.prro.2021.12.017                    |            |
| 2023 | Gabriele Palazzo et al  | Real-world validation of Artificial Intelligence-based Computed Tomography auto-contouring for prostate cancer radiotherapy planning                     |                                                               |            |
| 2021 | Jordan Wong et al       | Implementation of deep learning-based auto-segmentation for radiotherapy planning structures: a workflow study at two cancer centers                     |                                                               |            |
| 2021 | Weijun Chen             | A comparative study of auto‐contouring softwares in delineation of organs at risk in lung cancer and rectal cancer                                       | https://doi.org/10.1038/s41598-021-02330-y                    |            | 

### Commercially available products

| Manufacturer   | Product name | Details |
|----------------|--------------|---------|
| Limbus AI      | Limbus AI    |         |
| MVision AI     | Contour+     |         |
| Therapanacea   | ART Plan     |         |
| Mirada Medical | DLC Expert   |         |
| Vysioneer      | VBrain       |         |
|                |              |         |
