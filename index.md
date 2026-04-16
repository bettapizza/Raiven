---
layout: default
title: Home
---

<section class="section hero-copy">
  <h2>Hi, I’m {{ site.profile.name }}, and I build calm, capable systems for modern teams.</h2>
  <p>{{ site.profile.intro }}</p>
</section>

<section class="section">
  <div class="section-heading">
    <div>
      <p class="eyebrow">Featured</p>
      <h3>Selected work</h3>
      <p>A curated set of projects, case studies, and writing.</p>
    </div>
  </div>

  <div class="project-grid">
    {% for project in site.data.projects limit:6 %}
      {% include project_card.html project=project %}
    {% endfor %}
  </div>
</section>

<section class="section footer-cta">
  <h2>{{ site.footer.heading }}</h2>
  <p>{{ site.footer.text }}</p>
  <p><a href="mailto:{{ site.footer.email }}">{{ site.footer.email }}</a> <span class="dot">•</span> {{ site.footer.phone }}</p>
</section>
