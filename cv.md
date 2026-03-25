---
title: CV
permalink: /cv/
---

<section class="list-card">
  <p class="section-heading">Curriculum Vitae</p>
  <p>The current CV used to build this site is available here: <a href="{{ site.data.profile.cv_file | relative_url }}">Download PDF</a>.</p>
  <p>Details that were not available directly from the CV remain marked as <code>[placeholder]</code> in the site configuration so they are easy to find and replace later.</p>
</section>

<section class="grid-two">
  <div class="section-card">
    <p class="section-heading">Grants and Scholarships</p>
    <ul class="plain-list">
      {% for item in site.data.service.grants %}
      <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </div>
  <div class="section-card">
    <p class="section-heading">Conference Activity</p>
    <ul class="plain-list">
      {% for item in site.data.service.panel_discussant %}
      <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </div>
</section>

<section class="list-card">
  <p class="section-heading">Conference Presentations</p>
  <ul class="plain-list">
    {% for item in site.data.service.conference_presentations %}
    <li>{{ item }}</li>
    {% endfor %}
  </ul>
</section>
