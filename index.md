---
layout: default
---

{% for group in site.data.projects %}
### {{ group.category }}

<ul>
{% for project in group.projects %}
  <li><a href="{{ project.url }}"><strong>{{ project.name }}</strong></a> — {{ project.description }}</li>
{% endfor %}
</ul>

{% endfor %}
