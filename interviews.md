---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: interviews
---



<ul>
	{% assign works = site.works | sort: 'artist' %}
  {% for book in works %}
    <li>
      <a href="{{site.baseurl}}{{book.url}}">{{ book.title }}</a>, 
      {{book.artist}},
      				<img src="{{site.baseurl}}/img/products/{{book.img1}}" alt="{{book.alt-text}}">
    </li>
  {% endfor %}
</ul>