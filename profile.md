---
layout: default
title: My Profile
permalink: /profile/
netid: javerage
fruit:
  - name: apple
    cost: $1
    color: red
  - name: banana
    cost: $2
    color: yellow
  - name: orange
    cost: $1.50
    color: orange
---

<h1>{% if page.netid %}{{ page.netid }}{% else %}My Profile{% endif%}</h1>

Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Aenean faucibus felis id nunc pharetra, eget condimentum lorem facilisis. Etiam porta et augue in molestie. Sed maximus augue tincidunt, viverra ipsum sed, varius nunc. Nulla tincidunt purus purus. Morbi in lacinia massa, quis porttitor magna. Cras vulputate lacus eget venenatis viverra. Morbi in fringilla felis.


{{ page.netid }}

<ul>
    {% for item in page.fruit %}
    <li>{{ item.name }}, cost: {{ item.cost }}, color: {{ item.color }}</li>
    {% endfor %}
</ul>
