---
title: Home
---

<section class="hero">
  <div>
    <p class="section-heading">Academic Profile</p>
    <h1>{{ site.data.profile.short_name }}</h1>
    <p class="lede">{{ site.data.profile.position }} at {{ site.data.profile.institution }}, working on democratization, public opinion, political trust, and survey methodology across East and Southeast Asia.</p>
    <p>{{ site.data.profile.bio }}</p>
    <div class="button-row">
      <a class="button primary" href="{{ '/publications/' | relative_url }}">View Publications</a>
      <a class="button" href="{{ site.data.profile.cv_file | relative_url }}">Download CV</a>
    </div>
  </div>
  <aside class="hero-panel">
    <img class="portrait" src="{{ site.data.profile.portrait | relative_url }}" alt="Portrait of {{ site.data.profile.short_name }}">
    <h2>Contact</h2>
    <ul class="contact-list">
      <li>{{ site.data.profile.institution }}</li>
      <li>{{ site.data.profile.location }}</li>
      <li><a href="mailto:{{ site.data.profile.email }}">{{ site.data.profile.email }}</a></li>
      <li>{{ site.data.profile.phone }}</li>
      <li>
        {% if site.data.profile.website contains '[placeholder]' %}
        <code>{{ site.data.profile.website }}</code>
        {% else %}
        <a href="{{ site.data.profile.website }}">{{ site.data.profile.website }}</a>
        {% endif %}
      </li>
    </ul>
    <h2>Profiles</h2>
    <ul class="contact-list">
      {% for profile in site.data.profile.profiles %}
      <li>
        {% if profile.url contains '[placeholder]' %}
        {{ profile.label }}: <code>{{ profile.url }}</code>
        {% else %}
        <a href="{{ profile.url }}">{{ profile.label }}</a>
        {% endif %}
      </li>
      {% endfor %}
    </ul>
  </aside>
</section>

<section class="grid-two">
  <div class="section-card">
    <p class="section-heading">Research Interests</p>
    <div class="pill-list">
      {% for item in site.data.profile.research_interests %}
      <span class="pill">{{ item }}</span>
      {% endfor %}
    </div>
  </div>
  <div class="section-card">
    <p class="section-heading">Current Snapshot</p>
    <ul class="key-list">
      {% for item in site.data.profile.summary_points %}
      <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </div>
</section>

<section class="section-card">
  <p class="section-heading">Selected Experience</p>
  {% for item in site.data.experience limit:3 %}
  <article class="timeline-item">
    <div class="timeline-head">
      <h3>{{ item.title }}</h3>
      <p class="timeline-meta">{{ item.period }}</p>
    </div>
    <p><strong>{{ item.institution }}</strong></p>
    <ul>
      {% for bullet in item.bullets limit:2 %}
      <li>{{ bullet }}</li>
      {% endfor %}
    </ul>
  </article>
  {% endfor %}
</section>

<section class="section-card">
  <p class="section-heading">Education</p>
  {% for item in site.data.education %}
  <article class="timeline-item">
    <div class="timeline-head">
      <h3>{{ item.degree }}</h3>
      <p class="timeline-meta">{{ item.period }}</p>
    </div>
    <p><strong>{{ item.institution }}</strong>, {{ item.location }}</p>
    {% if item.details %}
    <ul>
      {% for detail in item.details %}
      <li>{{ detail }}</li>
      {% endfor %}
    </ul>
    {% endif %}
  </article>
  {% endfor %}
</section>
