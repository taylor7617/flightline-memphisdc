---
layout: default
title: Gates
permalink: /gates/
---

# Gates

<div class="gate-grid">
{% for gate in site.data.gates %}
  {% include gate-card.html gate=gate %}
{% endfor %}
</div>
