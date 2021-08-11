---
title: Sample
---
#This is a Sample Page

My text goes here. And we can *all* see it.

{% for page in site.pages %}
  <li>{{ page.collection }}</li>
  <h2>
    <a href="{{ page.url }}">{{ page.name }}</a>
  </h2>
  <!-- <p>(( minfile.content | markdownify }}</p> -->

{% endfor %}

<p>Collections should appear here:<br>
{% for minute in site.collections %}
  <li>{{ minute.label }}</li>
{% endfor %}
</p>

<p>Minutes should appear here:<br>
{% for minute in site.minutes %}
  <li>{{ minute.name }}</li>
{% endfor %}
</p>
