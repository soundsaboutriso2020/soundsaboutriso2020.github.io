---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
---

{% assign room2print = site.works | where: 'room', 'room2print' %}

<div class="prints room1 flex-row">
  {% for post in room2print %}
  <div class="print product">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>

{% assign room2zine = site.works | where: 'room', 'room2zine' %}

<div class="zines room1 flex-row">
  {% for post in room2zine %}
   <div class="zine product">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>