---
title: 立法院會議逐字稿
---

{% assign docs = site.pages | where_exp: "p", "p.path contains 'transcripts/'" | sort: "path" | reverse %}
<ul>
{% for p in docs %}
  <li><a href="{{ p.url | relative_url }}">{{ p.name | remove: ".md" }}</a></li>
{% endfor %}
</ul>
