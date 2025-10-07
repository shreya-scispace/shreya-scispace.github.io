---
layout: page
title: Home
permalink: /
---

<style>
/* Background image (uses Jekyll relative_url) */
body {
  background-image: url('{{ "/images/blackhole.jpg" | relative_url }}') !important;
  background-size: cover !important;
  background-position: center center !important;
  background-repeat: no-repeat !important;
  min-height: 100vh;
  margin: 0;
  color: #fff !important;
}

/* Content container */
.main-content {
  max-width: 980px;
  margin: 48px auto;
  background: rgba(0,0,0,0.55);
  padding: 28px;
  border-radius: 12px;
  box-shadow: 0 6px 18px rgba(0,0,0,0.35);
}

/* Links styling */
.home-links ul { padding-left: 1.2rem; }
.home-links a { color: #dfefff; text-decoration: underline; }
</style>

<div class="main-content">
# 👩‍🔬 Shreya Fal Dessai

Welcome to my undergraduate science portfolio — a collection of my academic projects, experiments, and certifications.

## Quick links
<div class="home-links">
<ul>
  <!-- Auto-list pages that include front matter 'title' -->
  {% for p in site.pages %}
    {% if p.title and p.url != "/" %}
      <li><a href="{{ p.url | relative_url }}">{{ p.title }}</a></li>
    {% endif %}
  {% endfor %}

  <!-- Explicit fallbacks (always visible) -->
  <li><a href="{{ '/experiments/' | relative_url }}">Experiments</a></li>
  <li><a href="{{ '/README.html' | relative_url }}">Repository README</a></li>
</ul>
</div>

</div>
