---
title: Join Us
nav:
  order: 4
  tooltip: Open positions
---

# {% include icon.html icon="fa-solid fa-user-plus" %}Join Us

We are currently building our inaugural team! See our open positions below.

{% comment %} openings are listed in _data/openings.yaml {% endcomment %}

{% include section.html %}

{% for opening in site.data.openings %}

{% assign icon = site.data.types[opening.role].icon %}
## {% include icon.html icon=icon %}{{ opening.title }} {#{{ opening.role }}}

{{ opening.description | replace: "Handshake", "[Handshake](https://joinhandshake.com)" }}

{% if opening.link %}
{%
  include button.html
  link=opening.link
  text="View job description"
  icon="fa-solid fa-arrow-right"
  flip=true
%}
{% endif %}

{% endfor %}

{% include section.html %}