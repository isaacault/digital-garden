---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

This is my digital garden, a drop zone for anything and everything that I feel
like writing.

Hopefully one day, I'll be able to refine the blurb a bit, but for now I'm 
purposely leaving it open ended and my goal is for things to get a bit 
_experimental_.

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — 
      <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
