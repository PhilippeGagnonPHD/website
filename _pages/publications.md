---
layout: archive
title: ""
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% if site.pubPreprint.size > 0 %}
   <h2 class="h2publication">Preprint</h2>
   {% for post in site.pubPreprint reversed %}
      {% include archive-single-publication.html %}
   {% endfor %}
{% endif %}
<h2 class="h2publication">Published</h2>
{% for post in site.publications reversed %}
  {% include archive-single-publication.html %}
{% endfor %}
