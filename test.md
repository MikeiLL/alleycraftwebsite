---
title: 'Works Gallery'
date: '2011-02-14T15:06:21-06:00'
author: 'David Alley'
layout: page
---
# TESTING

{% for staff_member in site.staff_members %}
  <h2>
    <a href="{{ staff_member.url }}">
      {{ staff_member.name }} - {{ staff_member.position }}
    </a>
  </h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
