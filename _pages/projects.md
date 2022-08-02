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
{% endfor %} <br> <br> For new projects within Guy's and St Thomas' NHS Foundation Trust (GSTT), please submit the [Project Initiation Document (PID)](../assets/docs/CSC-SubmissionForm-V3.docx)  via email to [CSC Team](mailto:CSCTeam@gstt.nhs.uk)