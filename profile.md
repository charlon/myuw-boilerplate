---
layout: default
title: My Profile
permalink: /profile/
---

<div class="myuw-card">

    <h1>{% if site.uw_netid %}{{ site.uw_netid }}{% else %}My Profile{% endif%}</h1>

    {% assign user = site.data.profiles.[site.uw_logged_in] %}

    <p>{{ user.uw_netid }}</p>

    <p>{{ user.uw_affiliation }}</p>

</div>
