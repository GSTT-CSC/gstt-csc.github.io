---
layout: platform_page
platform-name: XNAT
title: XNAT
platform-image: /assets/img/platforms/xnat_logo.png
---

[XNAT](https://xnat.org/) is an open-source imaging informatics platform for storing and managing medical 
images and associated data for research purposes. At GSTT, we use XNAT to retrieve, anonymise, and manage medical imaging 
and non-imaging data for purposes of AI development, AI evaluation, and for data provision for various research projects 
which are run at GSTT or in collaboration with GSTT. 

XNAT at GSTT is currently connected to 3 PACS systems (radiology, foetal cardiology and radiotherapy PACS). Data anonymisation
processes include DICOM meta-data removal, face blurring and removal of burnt-in data. Data used for AI evaluation are pushed 
to relevant DICOM nodes using a Python script; data used for AI development are fetched by [MLOPs](https://gstt-csc.github.io/platforms/mlops.html) via
XNAT's [REST API](https://wiki.xnat.org/display/XAPI), and data are sent to external collaborators via pathways agreed in ethics approval of each individual project.

<figure>
<img src="https://github.com/GSTT-CSC/XNAT/blob/main/assets/anon-flowchart.jpg?raw=true" width="100%">
<figcaption>Schematic representation of XNAT setup at GSTT.</figcaption>
</figure>

Using XNAT for data anonymisation and management allows fast and automated retrieval of research data, allows for good quality 
control and application of highest standards of anonymisation to protect patient privacy. Data visibility is granted explicitly, so 
only collaborators on a certain project have data visibility. Lastly, access to XNAT is strictly controlled and regularly reviewed. 

XNAT is only available to GSTT employees with access to GSTT network and before access can be granted an online teaching and 
training session is held. If you need access to XNAT, please contact the <a href="mailto:CSCTeam@gstt.nhs.uk">CSC team</a>.

For a wealth of information, including our SOPs, anonymisation scripts, data retrieval and fetching scripts and similar, please visit our [XNAT GitHub repository](https://github.com/GSTT-CSC/XNAT).

If you would like to us to retrieve data for your project and perform the relevant anonymisation process, please fill in the [data
request form](../../assets/docs/CSC-XNATdataRequestForm-V1.docx) and <a href="mailto:CSCTeam@gstt.nhs.uk">email</a> us with your data request. Please attach appropriate ethics approvals to the
email.

#### Estimated quote calculator for new projects
For an initial estimated quote for new projects, please use the below calculator, specifically editing the first two columns on the left-hand side, to confirm:

- The project name
- The project lead
- The requestor organisation
- Whether a National Data Opt-Out check is required for the patient cohort
- Target completion date i.e., for all requested tasks to be completed
- Number of studies required
- Tasks and associated modalities required

Once finished, please:

- Include the Total Estimated Project Cost in your new project request
- Retain a screenshot as we will request this be sent to us via email after we've reviewed your request

<iframe width="700" height="450" frameborder="0" style="border: 5px solid black;" scrolling="no" src="https://emckclac-my.sharepoint.com/:x:/g/personal/k2252499_kcl_ac_uk/EXS5NZSBoqtLutkCXBP3QlMBXcl0s8H6QLJY6_PDYBV7JQ?e=aDgc9i&action=embedview&wdAllowInteractivity=False&AllowTyping=True&ActiveCell='Invoice'!B1&Item='Invoice'!A1%3AC20&wdHideGridlines=True&wdInConfigurator=True&wdInConfigurator=True"></iframe>