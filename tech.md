---
layout: page
permalink: /tech/
title: tech
description: technics change the world
---

<ul class="post-list">
{% for poem in site.tech reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y--%H:%M' }}</p>
      </li>
{% endfor %}
</ul>