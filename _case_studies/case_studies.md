---
layout: default
title: Case Studies
permalink: /case_studies/
---

# {{ page.title }}

{% for study in site.case_studies %}
## [{{ study.title }}]({{ study.url | relative_url }})

{% if study.description %}
{{ study.description }}
{% endif %}

---
{% endfor %}