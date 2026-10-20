---
layout: default
---
# {{ site.tagline }}

{{ site.description }}

<ul class="post-list">
{% for p in posts %}
  <li><a href="{{ p.url }}">{{ p.title }}</a> <span class="dim">{{ p.date | date: '%b %e, %Y' }}</span></li>
{% endfor %}
</ul>
