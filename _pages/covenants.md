---
layout: default
title: Covenants
permalink: /covenants/
---

# Covenants

Below is the live catalog of the 40 Memphis DC covenants. Click any title to jump; each section includes **Orders**, **Effect**, and **Proof Protocol**.

{% assign covs = site.data.covenants %}
{% if covs and covs.size > 0 %}

<nav class="container" aria-label="Covenant index" style="margin:16px 0;">
  <strong>Jump to:</strong>
  <ul style="columns: 2; -webkit-columns: 2; -moz-columns: 2; padding-left: 18px;">
  {% for c in covs %}
    {% assign slug = c.slug | default: c.title | slugify %}
    <li style="break-inside: avoid;"><a href="#{{ slug }}">{{ c.title }}</a></li>
  {% endfor %}
  </ul>
</nav>

{% for c in covs %}
  {% include covenant-item.html c=c %}
{% endfor %}

{% else %}
> No covenants found. Add items to **_data/covenants.yml**.
{% endif %}
