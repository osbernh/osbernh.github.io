---
permalink: /
title: "Osbern Huang"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Osbern Huang is a Research Fellow in the School of Government and International Relations at Griffith University. His research focuses on democratization, democratic consolidation, political trust, public opinion, and survey methodology, with particular attention to East and Southeast Asia and comparative work extending to Australia.

His work connects comparative politics with applied survey research, combining experience in mixed-mode survey design, probability-based online panels, GIS/GPS sampling, and large-scale post-survey data management.

Research interests
======
* Democratization and democratic consolidation
* Public opinion and survey methodology
* Comparative politics in East and Southeast Asia
* Political trust, cultural values, and redistribution

Current positions and recent experience
======
{% for item in site.data.experience limit: 4 %}
* **{{ item.title }}**, {{ item.institution }} ({{ item.period }})
  * {{ item.bullets[0] }}
{% endfor %}

Selected projects
======
{% for item in site.data.projects limit: 4 %}
* **{{ item.title }}** ({{ item.period }})
  * {{ item.bullets[0] }}
{% endfor %}

Education
======
{% for item in site.data.education %}
* **{{ item.degree }}**, {{ item.institution }} ({{ item.period }})
{% endfor %}

Download
======
* [Curriculum Vitae](/files/CV.pdf)
