---
title: Publications
permalink: /publications/
---

<section class="list-card">
  <p class="section-heading">Journal Articles</p>
  {% for item in site.data.publications.papers %}
  <article class="pub-item">
    <p>{{ item.citation }}</p>
  </article>
  {% endfor %}
</section>

<section class="list-card">
  <p class="section-heading">Book Chapters</p>
  {% for item in site.data.publications.book_chapters %}
  <article class="pub-item">
    <p>{{ item.citation }}</p>
  </article>
  {% endfor %}
</section>

<section class="grid-two">
  <div class="section-card">
    <p class="section-heading">Reports</p>
    <ul class="plain-list">
      {% for item in site.data.publications.reports %}
      <li>{{ item.citation }}</li>
      {% endfor %}
    </ul>
  </div>
  <div class="section-card">
    <p class="section-heading">Under Review / In Progress</p>
    <ul class="plain-list">
      {% for item in site.data.publications.under_review %}
      <li>{{ item.citation }}</li>
      {% endfor %}
      {% for item in site.data.publications.in_preparation %}
      <li>{{ item.citation }}</li>
      {% endfor %}
    </ul>
  </div>
</section>
