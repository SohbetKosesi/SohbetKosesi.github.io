---
layout: page
title: Poems
permalink: /poems/
---

<h1>Poems</h1>

{% for poem in site.poems reversed %}
  <div class="poem-preview">
    <h2><a href="{{ poem.url }}">{{ poem.title }}</a></h2>
    <p class="date">{{ poem.date | date: "%b %d, %Y" }}</p>
  </div>
{% endfor %}
