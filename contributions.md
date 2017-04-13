---
layout: page
title: Contributions
permalink: /contributions/
---
<ul class="contribution-list">
  {% for contribution in site.contributions %}
    <li>
      <span class="contribution-meta">{{ contribution.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="contribution-link" href="{{ contribution.url | relative_url }}">{{ contribution.title | escape }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
