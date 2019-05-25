---
layout: page
title: "Talks"
permalink: /talks/
author_profile: true
---

{% for post in site.talks reversed %}
  {% include talk.html %}
{% endfor %}
  

