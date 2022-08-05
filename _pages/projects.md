---
layout: project_board
title: Projects
permalink: /projects.html
---

The Project Board below tracks the progress of each CSC project through the different 
phases of the software developmental lifecycle. 

These stages are:

{% for project in site.data.project-board %}
- **{{ project.project-status }}**: {{ project.description -}}
{% endfor %}

<br>

#### Project Evaluation submission form

If you are creating medical software and would like the CSC Team to consider evaluating it for clinical use 
within Guy's and St Thomas' NHS Foundation Trust, please complete and submit the
[Project Initiation Document (PID)](../assets/docs/CSC-SubmissionForm-V3.docx) via email to [CSCTeam@gstt.nhs.uk](mailto:CSCTeam@gstt.nhs.uk)