#This is a Sample Page

My text goes here. And we can *all* see it.
<h5>{{ site.minutes.label }}</h5>

{% for minfile in site.minutes %}
  <h2>
    <a href="{{ minfile.url }}">Link to File
      <!-- (( staff_member.name }} - (( staff_member.position }} -->
    </a>
  </h2>
  <p>{{ minfile.content | markdownify }}</p>
{% endfor %}
