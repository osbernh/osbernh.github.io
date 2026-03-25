---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

Research agenda
======
My work examines how democratic attitudes are formed, sustained, and challenged across political settings. I study public opinion, democratic consolidation, political trust, and survey methodology, with a regional focus on East and Southeast Asia and comparative work extending to Australia.

Current projects
======
{% for item in site.data.projects %}
* **{{ item.title }}** ({{ item.period }})
  * {% for bullet in item.bullets %}{{ bullet }}{% unless forloop.last %}; {% endunless %}{% endfor %}
{% endfor %}

Methods
======
* Survey experiments
* Mixed-mode surveys
* Probability-based online panels
* GIS/GPS sampling
* Comparative public opinion research
* Quantitative data analysis
