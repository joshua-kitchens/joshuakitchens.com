---
title: Joshua Kitchens
layout: default
---

I'm an archivist and educator. This site collects the case studies I've written for teaching archives and archival issues, along with my [vita](/vita/).

## Archival Case Studies

The lecture is dead. Long live the lecture. I hate the lecture format, and as part of my efforts to move away from it, I've created a series of case studies to teach archives and archival issues. They're available here under a Creative Commons license.

{% assign groups = site.case_studies | sort: "title" | group_by: "category" | sort: "name" %}
{% for group in groups %}
### {{ group.name }}
{% for study in group.items %}
- [{{ study.title }}]({{ study.url | relative_url }}){% if study.description %} — {{ study.description }}{% endif %}
{% endfor %}
{% endfor %}

See also: [Interactive Case Studies](/interactive-case-studies/)
