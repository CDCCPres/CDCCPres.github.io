---
title: Sample
---
#This is a Sample Page

My text goes here. And we can *all* see it.

{% for page in site.pages %}
  <li>{{ page.collection }}</li>
  <h2>
    <a href="{{ page.url }}">(( page.name }}</a>
  </h2>
  <!-- <p>(( minfile.content | markdownify }}</p> -->

{% endfor %}

<p>Collections should appear here:<br>
{% for collection in site.collections %}
  <li>{{ collection.name }}</li>
{% endfor %}
</p>
