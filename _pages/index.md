---
layout: page
title: Garden 🌱
id: garden
permalink: /garden
---

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">

Take a look at <span style="font-weight: bold"><a href="{{ site.baseurl }}/digital-rupee" class="internal-link">How India's CBDC Will Fit into Digital Payments</a></span> to get started on your exploration.

</p>

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
