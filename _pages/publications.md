---
layout: page
title: "Publications"
permalink: /publications/
author_profile: true
---

{% for post in site.publications reversed %}
  {% include publication.html %}
{% endfor %}
  

