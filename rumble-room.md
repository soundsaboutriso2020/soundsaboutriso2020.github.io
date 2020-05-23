---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
title: Rumble Room
next: /palm-room
---

<div id="room4prints"></div>

{% assign room4print = site.works | where: 'roomtype', 'rumble-room-print' | sort: 'order' %}

<div class="prints room4 flex-row space-around aligncenter">
  {% for post in room4print %}
  <div class="print product hvr-buzz {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}" alt="{{post.alttext}}"></a>
</div>
  {% endfor %}
</div>

<div id="room4zines" class="full-width">
{% assign room4zine = site.works | where: 'roomtype', 'rumble-room-zine' | sort: 'order' %}

<div class="zines room4 flex-row space-around aligncenter">
  {% for post in room4zine %}
   <div class="zine product hvr-buzz {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}" alt="{{post.alttext}}"></a>
</div>
  {% endfor %}
</div>
</div>

