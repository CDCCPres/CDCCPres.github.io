---
title: Sample
---
#This is a Sample Page

My text goes here. And we can *all* see it.
<h5>{{ site.minutes.label }}</h5>

{% for minfile in site.pages %}
  <li>minfile.collection</li>
  <h2>
    <a href="{{ minfile.url }}">
      (( minfile.name }}
    </a>
  </h2>
  <!-- <p>(( minfile.content | markdownify }}</p> -->
{% endfor %}
