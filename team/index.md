---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

We are currently building our inaugural team! Review [open positions]({{ "join" | relative_url }}) to see if you could be our next member.

{% include section.html %}

{% include list.html data="members" component="portrait" filter="!placeholder && role == 'principal-investigator'" %}
{% include list.html data="members" component="portrait" filter="!placeholder && role == 'postdoc'" %}
{% include list.html data="members" component="portrait" filter="!placeholder && role == 'phd'" %}
{% include list.html data="members" component="portrait" filter="!placeholder && role == 'ms'" %}
{% include list.html data="members" component="portrait" filter="!placeholder && role == 'staff'" %}
{% include list.html data="members" component="portrait" filter="!placeholder && role == 'undergrad'" %}
{% include list.html data="members" component="portrait" filter="!placeholder && !['principal-investigator', 'postdoc', 'phd', 'ms', 'staff', 'undergrad'].include?(role)" %}
{% include list.html data="members" component="portrait" filter="placeholder && role == 'principal-investigator'" %}
{% include list.html data="members" component="portrait" filter="placeholder && role == 'postdoc'" %}
{% include list.html data="members" component="portrait" filter="placeholder && role == 'phd'" %}
{% include list.html data="members" component="portrait" filter="placeholder && role == 'ms'" %}
{% include list.html data="members" component="portrait" filter="placeholder && role == 'staff'" %}
{% include list.html data="members" component="portrait" filter="placeholder && role == 'undergrad'" %}
{% include list.html data="members" component="portrait" filter="placeholder && !['principal-investigator', 'postdoc', 'phd', 'ms', 'staff', 'undergrad'].include?(role)" %}

{% comment %}
placeholder sections, hidden for now (remove the comment tags to show them again)

{% include section.html background="images/background.jpg" dark=true %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
{% endcomment %}
