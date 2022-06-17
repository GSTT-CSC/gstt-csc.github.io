---
layout: project_board
title: Projects
permalink: /ourwork.html
---

The Project Board below tracks the progress of each CSC project through the different 
phases of the software developmental lifecycle. 

These stages are:

{% for project in site.data.project-board %}
- **{{ project.project-status }}**: {{ project.description -}}
{% endfor %}
