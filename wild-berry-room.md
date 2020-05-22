---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
title: wild berry room
next: /interviews
---

<div id="room6prints"></div>


{% assign room5print = site.works | where: 'roomtype', 'wild-berry-room-print' | sort: 'order' %}

<div class="prints room5 flex-row space-around aligncenter">
  {% for post in room5print %}
  <div class="print product hvr-hang {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>

<div id="room6zines" class="full-width">

{% assign room5zine = site.works | where: 'roomtype', 'wild-berry-room-zine' | sort: 'order' %}

<div class="zines room5 flex-row space-around aligncenter">
  {% for post in room5zine %}
   <div class="zine product hvr-bob {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>
</div>

