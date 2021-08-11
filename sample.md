---
title: Sample
---
#This is a Sample Page

My text goes here. And we can *all* see it.

{% for minfile in site.pages %}
  <li>{{ minfile.collection }}</li>
  <h2>
    <a href="{{ minfile.url }}">
      (( minfile.name }}
    </a>
  </h2>
  <!-- <p>(( minfile.content | markdownify }}</p> -->
{% endfor %}
<p>
{% for collection in site.collections %}
  <li>{{ collection.name }}</li>
{% endfor %}
</p>
