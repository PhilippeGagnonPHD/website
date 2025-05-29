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

{% if site.preprints.size > 0 %}
   <h1 class="h2publication">Preprints</h1>
   {% for post in site.preprints reversed %}
      {% include archive-single-publicationV2.html %}
   {% endfor %}
{% endif %}
<h1 class="h2publication">Publications</h1>
{% for post in site.publications reversed %}
  {% include archive-single-publicationV2.html %}
{% endfor %}
