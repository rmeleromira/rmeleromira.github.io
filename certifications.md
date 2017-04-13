---
layout: page
title: Certifications
permalink: /certs/
---
<ul class="certification-list">
  {% for certification in site.certifications %}
    <li>
      <span class="certification-meta">{{ certification.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="certification-link" href="{{ certification.url | relative_url }}">{{ certification.title | escape }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
