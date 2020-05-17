---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
---



<ul>
  {% for post in site.artists %}
    <li>
      {{ post.title }}, 
      {{post.artist}}
    </li>
  {% endfor %}
</ul>