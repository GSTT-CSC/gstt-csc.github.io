---
layout: project_board
title: Projects
permalink: /projects.html
---
<br>
#### Project submission form

If you would like to work with us, have a project that needs our support in any project stage, or have a product you
would like us to evaluate for clinical use, please complete and submit the
[Project Initiation Document (PID)](../assets/docs/CSC-SubmissionForm-V3.docx) via email to [CSCTeam@gstt.nhs.uk](mailto:ClinicalScientificComputing@gstt.nhs.uk)

<br>
#### Project stages

The Project Board below tracks the progress of each CSC project through the different 
phases of the software developmental lifecycle. 

These stages are:

{% for project in site.data.project-board %}
- **{{ project.project-status }}**: {{ project.description -}}
{% endfor %}

<br>

