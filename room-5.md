---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
title: Room 5
next: /interviews
---

<div id="room5prints"></div>


{% assign room5print = site.works | where: 'room', 'room5print' %}

<div class="prints room5 flex-row space-around">
  {% for post in room5print %}
  <div class="print product hvr-hang">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>

<div id="room5zines" class="full-width">
{% assign room5zine = site.works | where: 'room', 'room5zine' %}

<div class="zines room5 flex-row space-around">
  {% for post in room5zine %}
   <div class="zine product hvr-bob">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>
</div>

