---
layout: page
permalink: /say/
title: say
description: any thoughts deposit here.
---

<ul class="post-list">
{% for poem in site.say reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y--%H:%M' }}</p>
      </li>
{% endfor %}
</ul>