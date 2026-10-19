---
layout: default
title: Case Studies
permalink: /case_studies/
redirect_from: /case-studies/
---

Case studies for teaching archives and archival issues, grouped by topic. Each includes learning objectives, a scenario, discussion questions, and (where available) a bibliography.

{% assign groups = site.case_studies | sort: "title" | group_by: "category" | sort: "name" %}
{% for group in groups %}
## {{ group.name }}
{% for study in group.items %}
### [{{ study.title }}]({{ study.url | relative_url }})

{{ study.description }}
{% endfor %}
{% endfor %}
