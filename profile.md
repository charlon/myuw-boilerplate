---
layout: default
title: My Profile
permalink: /profile/

---

<h1>{% if site.uw_netid %}{{ site.uw_netid }}{% else %}My Profile{% endif%}</h1>

{% assign user = site.data.profiles.[site.uw_logged_in] %}

{{ user.uw_netid }}

{{ user.uw_affiliation }}

{% if user.uw_courses %}
course schedule
<ul>
    {% for item in user.uw_courses %}
    <li>{{ item.name }}</li>
    {% endfor %}
</ul>
{% endif %}
