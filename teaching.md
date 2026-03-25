---
title: Teaching
permalink: /teaching/
---

<section class="list-card">
  <p class="section-heading">Teaching Experience</p>
  {% for item in site.data.teaching %}
  <article class="timeline-item">
    <div class="timeline-head">
      <h3>{{ item.course }}</h3>
      <p class="timeline-meta">{{ item.period }}</p>
    </div>
    <p><strong>{{ item.role }}</strong></p>
    {% if item.notes %}
    <ul>
      {% for note in item.notes %}
      <li>{{ note }}</li>
      {% endfor %}
    </ul>
    {% endif %}
  </article>
  {% endfor %}
</section>

<section class="grid-two">
  <div class="section-card">
    <p class="section-heading">Languages</p>
    <div class="pill-list">
      {% for item in site.data.service.skills.languages %}
      <span class="pill">{{ item }}</span>
      {% endfor %}
    </div>
  </div>
  <div class="section-card">
    <p class="section-heading">Technical Skills</p>
    <div class="pill-list">
      {% for item in site.data.service.skills.tools %}
      <span class="pill">{{ item }}</span>
      {% endfor %}
    </div>
  </div>
</section>
