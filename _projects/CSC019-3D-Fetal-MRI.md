---
layout: project_page
title: Motion-corrected 3D Fetal Brain MRI
status: Concluded
image: /assets/img/projects/3d_fetal_mri_project_image.jpg
summary: An automated software workflow for reconstruction of motion-corrected 3D fetal MRI images 
csc-lead: <a href="/team_member/Tom.html">Tom</a>
modality: MRI
pathology: Congenital birth defects
rationale: Fetal MRI is predominantly performed using 2D MRI, but this approach is susceptible to motion artefacts when the baby moves. Motion-corrected 3D MRI produces higher quality images, with the potential to improve diagnosis of abnormalities.
patient-pathway: 
training-data: 
errors: 
goals: 
success-criteria: 
alternatives: 
---
<b>Academic Partners</b>

Mary Rutherford, Joseph Hajnal, Maria Deprez, Alena Uus @ Perinatal Imaging & Health, King's College London

<b>Project Overview</b>

Fetal MRI is an important adjunct to ultrasound imaging as it can provide additional confidence and insights when making 
a prenatal diagnosis. However, fetal motion during MRI scans can cause images to be blurry and not of sufficient 
diagnostic quality. In some cases, fetal motion can be so severe that the radiographer has to reacquire multiple scans 
until quality images are obtained, which can be very inefficient.

For more than 15 years, researchers in the department of Perinatal Imaging & Health at King's College London have 
been developing advanced motion-correction MRI techniques. These techniques can provide artefact-free 3D MRI 
reconstructions of the fetal brain, heart and body. 

In this project, CSC is working closely with the team at KCL to make these advanced 3D MRI 
techniques easier and more efficient for clinicians to use, and to make it easier for other hospitals to adopt these 
tools in their clinical pathways. For example, one of the first apps available on AIDE will be for motion-corrected 3D 
fetal brain MRI.

3D fetal brain MRI is performed by reconstruction of single-slice 2D MRI images into 3D volumes using slice-to-volume 
registration ([SVR – www.svrtk.github.io](https://www.svrtk.github.io)) methods. Now, with the advent of machine 
learning technologies, it is possible for hospitals to perform 3D fetal brain MRI in a fully automated manner.

<b>References</b>

<a href="https://doi.org/10.1259/bjr.20220071">Uus A, et al. 2022. Retrospective motion correction in foetal MRI for 
clinical applications: existing methods, applications and integration into clinical practice</a>

<a href="http://www.svrtk.github.io/">SVRTK GitHub repository</a>
