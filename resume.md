---
layout: page
title: Resume
permalink: /resume/
---
<ul class="job-list">
  {% for job in site.jobs %}
    <li>
      {% if job.startdate == job.enddate %}
      <span class="job-meta">{{ job.startdate | date: "%b, %Y" }} - Current</span>
      {% else %}
      <span class="job-meta">{{ job.startdate | date: "%b, %Y" }} - {{ job.enddate | date: "%b, %Y" }}</span>
      {% endif %}
      <h2>
        <a class="job-link" href="{{ job.url | relative_url }}">{{ job.employer | escape }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
