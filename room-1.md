---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
title: Room 1
next: /room-2
---

<div id="room1prints"></div>


{% assign room1print = site.works | where: 'room', 'room1print' %}

<div class="prints room1 flex-row space-around">
  {% for post in room1print %}
  <div class="print product hvr-hang">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>

<div id="room1zines" class="full-width">
{% assign room1zine = site.works | where: 'room', 'room1zine' %}

<div class="zines room1 flex-row space-around">
  {% for post in room1zine %}
   <div class="zine product hvr-buzz">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>
</div>
