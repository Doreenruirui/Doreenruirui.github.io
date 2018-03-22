---
layout: page
title: Tag
---
<div class="post">
<ul>
{% for tag in site.tags %}
{% capture tag_name %}{{ tag | first }}{% endcapture %}
<!--<h1>Tag: {{ tag_name }}</h1> -->
<a class="no-underline" href="/tag/{{ tag_name }}"><code class="highligher-rouge"><nobr>{{ tag_name }}</nobr></code>&nbsp;</a>
<!--{% for post in site.tags[tag_name] %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date_to_string }})<br>
    {{ post.description }}
  </li>
{% endfor %}
-->
{% endfor%}
</ul>
</div>
<hr>
