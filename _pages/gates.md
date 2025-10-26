---
layout: default
title: Gates
permalink: /gates/
---

<div class="hero">
  <img src="{{ '/assets/headers/flight-1130-angels-kitchen.png' | relative_url }}" alt="Angel’s Kitchen — Flight 1130">
</div>

## Gates
Open full Gates directory — Every ZIP = Runway. Each Gate is a leaseable digital location.

<div class="gates-grid">
  {% for g in site.data.gates %}
    {% include gate-card.html gate=g %}
  {% endfor %}
</div>
