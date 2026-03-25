---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Download
======
* [Full CV PDF](/files/CV.pdf)

Education
======
{% for item in site.data.education %}
* **{{ item.degree }}**, {{ item.institution }}, {{ item.location }} ({{ item.period }})
{% endfor %}

Work experience
======
{% for item in site.data.experience %}
* **{{ item.title }}**, {{ item.institution }} ({{ item.period }})
  * {% for bullet in item.bullets %}{{ bullet }}{% unless forloop.last %}; {% endunless %}{% endfor %}
{% endfor %}

Research projects
======
{% for item in site.data.projects %}
* **{{ item.title }}** ({{ item.period }})
{% endfor %}

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Conference activity
======
{% for item in site.data.service.conference_presentations %}
* {{ item }}
{% endfor %}

Grants and scholarships
======
{% for item in site.data.service.grants %}
* {{ item }}
{% endfor %}
