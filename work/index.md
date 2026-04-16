---
layout: default
title: Work
---

<section class="section page-intro">
  <h2>Work</h2>
  <p>A selection of portfolio pieces, technical work, talks, and notes.</p>
</section>

<section class="section">
  <div class="project-grid">
    {% for project in site.data.projects %}
      {% include project_card.html project=project %}
    {% endfor %}
  </div>
</section>
