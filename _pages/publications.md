---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
portfolio: true
excerpt: "Research papers, preprints, and patents by Mingdian Liu, spanning generative AI, language models, sensing, and computational design."
---

<div class="portfolio-intro" markdown="1">

Research in generative AI, conversational agents, computational design, and sensing.

For citation counts and the latest indexing, visit my [Google Scholar profile](https://scholar.google.com/citations?user=I0_tNbsAAAAJ&hl=en).

</div>

<nav class="publication-nav" aria-label="Publication categories">
  {% for section in site.data.publications %}
  <a href="#{{ section.id }}">{{ section.title }}</a>
  {% endfor %}
</nav>

{% for section in site.data.publications %}
<section class="portfolio-section publication-section" aria-labelledby="{{ section.id }}">
  <h2 id="{{ section.id }}">{{ section.title }}</h2>
  {% include publication-list.html publications=section.items %}
</section>
{% endfor %}

<p class="publication-updated">Last updated September 2026. ‡ Equal contribution.</p>
