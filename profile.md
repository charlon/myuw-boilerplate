---
layout: default
title: My Profile
permalink: /profile/
---

<div class="myuw-card">

    {% assign user = site.data.profiles.[site.uw_logged_in] %}

    <h1>{{ user.uw_netid }}</h1>
    <p>{{ user.uw_affiliation }}</p>

</div>
