---
layout: page
title: Resume
permalink: /resume/
---
<ul class="job-list">
  {% for job in site.jobs %}
    <li>
      <span class="job-meta">{{ job.startdate | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="job-link" href="{{ job.url | relative_url }}">{{ job.employer | escape }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
