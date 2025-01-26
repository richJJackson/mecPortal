---
layout: allapp
title: Applications
description: List of Applied Problems
image: assets/images/pic11.jpg
nav-menu: true
---


<h1> All Applications </h1>


{% for app in site.applications %}
  <h2>{{ app.title }} - {{ app.area }}</h2>
  <p>{{ app.content | markdownify }}</p>
{% endfor %}

