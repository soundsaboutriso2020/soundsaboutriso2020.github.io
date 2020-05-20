---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
title: Room 4
---

<div id="room4prints"></div>


{% assign room4print = site.works | where: 'room', 'room4print' %}

<div class="prints room4 flex-row space-around">
  {% for post in room4print %}
  <div class="print product">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>

<div id="room4zines" class="full-width">
{% assign room4zine = site.works | where: 'room', 'room4zine' %}

<div class="zines room4 flex-row space-around">
  {% for post in room4zine %}
   <div class="zine product">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>
</div>

