---
title: Research
permalink: /research/
---

<section class="list-card">
  <p class="section-heading">Research Agenda</p>
  <p>My work examines how democratic attitudes are formed, sustained, and challenged across different political settings. I study public opinion, political trust, democratic consolidation, and survey methodology, with a regional focus on East and Southeast Asia and comparative work that extends to Australia and other democracies.</p>
  <p>Current priorities include democratic accountability, cross-national survey experimentation, public trust in institutions, and the relationship between cultural values and preferences for redistribution or authoritarian alternatives.</p>
</section>

<section class="list-card">
  <p class="section-heading">Academic Projects</p>
  {% for project in site.data.projects %}
  <article class="timeline-item">
    <div class="timeline-head">
      <h3>{{ project.title }}</h3>
      <p class="timeline-meta">{{ project.period }}</p>
    </div>
    <ul>
      {% for bullet in project.bullets %}
      <li>{{ bullet }}</li>
      {% endfor %}
    </ul>
  </article>
  {% endfor %}
</section>

<section class="grid-two">
  <div class="section-card">
    <p class="section-heading">Methods</p>
    <div class="pill-list">
      <span class="pill">Survey experiments</span>
      <span class="pill">Mixed-mode surveys</span>
      <span class="pill">Probability-based online panels</span>
      <span class="pill">GIS/GPS sampling</span>
      <span class="pill">Comparative public opinion</span>
      <span class="pill">Quantitative analysis</span>
    </div>
  </div>
  <div class="section-card">
    <p class="section-heading">Collaboration</p>
    <p>I am open to collaborations in comparative politics, democratic resilience, public trust, survey design, and East and Southeast Asian politics.</p>
    <p>Email: <a href="mailto:{{ site.data.profile.email }}">{{ site.data.profile.email }}</a></p>
  </div>
</section>
