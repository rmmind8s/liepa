---
layout: page
title: Dokumentai
---

{% assign dokumentai = site.posts | where: "category", "dokumentas" %}
{% for doc in dokumentai %}

## [{{ doc.title }}]({{ doc.url }})

{{ doc.excerpt }}

{% endfor %}
