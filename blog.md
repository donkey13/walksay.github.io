---
layout: page
permalink: /blog/
title: blog
description: Showcase your writing, short stories, or poems. Replace this text with your description.
---

<ul class="post-list">
{% for poem in site.blog reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y 鈥� %H:%M' }}</p>
      </li>
{% endfor %}
</ul>