---
layout: default
title: My Profile
permalink: /profile/
courses:
  - name: CHEM 101
    cost: $1
    color: red
  - name: CSE 142
    cost: $2
    color: yellow
  - name: MATH 303
    cost: $1.50
    color: orange
---

<h1>{% if site.uw_netid %}{{ site.uw_netid }}{% else %}My Profile{% endif%}</h1>

{{ site.uw_affiliation }}

Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Aenean faucibus felis id nunc pharetra, eget condimentum lorem facilisis. Etiam porta et augue in molestie. Sed maximus augue tincidunt, viverra ipsum sed, varius nunc. Nulla tincidunt purus purus. Morbi in lacinia massa, quis porttitor magna. Cras vulputate lacus eget venenatis viverra. Morbi in fringilla felis.

course schedule

<ul>
    {% for item in page.courses %}
    <li>{{ item.name }}, cost: {{ item.cost }}, color: {{ item.color }}</li>
    {% endfor %}
</ul>
