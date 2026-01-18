---
title: Home
description: Portfolio — projects and background
---

<section class="section">
  <h2>About</h2>
  <div class="card">
    <p>
      I’m Caio Correa — I build data products and decision-support tools, from forecasting and scenario analysis
      to applied research analytics.
    </p>
    <div class="row">
      <a class="btn" href="https://github.com/dr-caio-correa" target="_blank" rel="noreferrer">GitHub</a>
      <a class="btn ghost" href="/about">More about me</a>
      <!-- Optional: add LinkedIn + Resume PDF later -->
    </div>
  </div>
</section>

<section class="section" id="projects">
  <h2>Projects</h2>

  <div class="grid">
    {% assign items = site.projects | sort: "order" %}
    {% for p in items %}
      <div class="card">
        <h3>{{ p.title }}</h3>
        <p>{{ p.subtitle }}</p>
        <div class="row">
          <a class="btn" href="{{ p.url | relative_url }}">Read more</a>
          <a class="btn ghost" href="{{ p.repo }}" target="_blank" rel="noreferrer">Repo</a>
        </div>
      </div>
    {% endfor %}
  </div>
</section>
