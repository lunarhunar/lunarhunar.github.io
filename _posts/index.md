---
layout: home
---

<h2>All Pages</h2>
<ul>
  {% for page in site.pages %}
    {% if page.title and page.layout != "home" %}
      <li><a href="{{ page.url | relative_url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

