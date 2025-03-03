---
layout: education
permalink: /fellowship_publications.html
title: Fellows' Publications
display_title: NHS Fellowship in Clinical AI<br>Fellows' Publications
---

Fellows have opportunities to publish academically during NHS Fellowship in Clinical AI, particularly relating to their AI project.
Explore the fellowship-related publications of our fellows below.


<!-- Fellows' Publications -->
<table class="table table-hover">
  <thead>
    <tr>
      <th scope="col">Publication</th>
      <th scope="col">Fellow</th>
    </tr>
  </thead>
  <tbody>
  {% for resource in site.data.fellowship_publications %}
  <tr>
    <td>{% if resource.link %}<a href="{{ resource.link }}">{{ resource.title }}</a>{% else %} {{ resource.title }}{% endif %}</td>
    <td>{{ resource.fellow }}</td>
  </tr>
{% endfor %}
  </tbody>
</table>
<!-- Fellows' Publications -->

<i> Last updated: March 2025 </i>