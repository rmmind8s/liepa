---
layout: page
title: Dokumentai
---

{% assign dokumentai = site.posts | where: "category", "dokumentas" %}
{% for doc in dokumentai %}

## [{{ doc.title }}]({{ site.baseurl }}{{ doc.url }})

{{ doc.excerpt }}

{% endfor %}
