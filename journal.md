---
layout: page
permalink: /journal/
title: journal
description: Class journal for The Iron Yard.
---

<ul class="post-list">
{% for journal in site.journal reversed %}
    <li>
        <h2><a class="journal-title" href="{{ journal.url | prepend: site.baseurl }}">{{ journal.title }}</a></h2>
        <p class="post-meta">{{ journal.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
