---
layout: page
title: Proyectos
permalink: /projects/
---

{% for p in site.projects reversed %}
### [{{ p.title }}]({{ p.url | relative_url }})
{{ p.summary }}

{% if p.visor_url %}
**Visor:** [Abrir]({{ p.visor_url }})
{% endif %}

---
{% endfor %}
