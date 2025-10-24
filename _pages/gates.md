---
layout: default
title: Gates
permalink: /gates/
---

<!-- HERO (Angel’s Kitchen — Flight 1130) -->
<div class="hero">
  <img src="{{ '/assets/headers/flight-1130-angels-kitchen.png' | relative_url }}"
       alt="Angel’s Kitchen — Flight 1130">
</div>

<!-- EXISTING CARDS (kept) -->
<div class="gates-grid">
  {% for gate in site.data.gates %}
    {% include gate-card.html gate=gate %}
  {% endfor %}
</div>
