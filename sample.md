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
  <p>...{{ minute.label }} - Output: {{ minute.output }} - <br>
      dir: {{ minute.directory }} - rel_dir: {{ minute.relative_directory }} - <br>
    Count: {{ minute.count }}</p>
    {% for minutefile in minute %}
      <p>{{ minutefile.content }}</p>
    {% endfor %}
{% endfor %}
</p>

<p>Minutes should appear here:<br>
{% for minute in site.minutes %}
  <li>{{ minute.relative_path }}</li>
  Collection: {{ minute.collection }}<br>
  Date: {{ minute.date }}<br>
  Redenered Output: <p>{{ minute.output }}</p>
    
  Unrendered Content: <p>{{ minute.content }}</p>
{% endfor %}
</p>
