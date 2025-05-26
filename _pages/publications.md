---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}
<h2>Preprint</h2>
{% for post in site.pubPreprint reversed %}
  {% include archive-single-publication.html %}
{% endfor %}
<h2>Published</h2>
{% for post in site.publications reversed %}
  {% include archive-single-publication.html %}
{% endfor %}
