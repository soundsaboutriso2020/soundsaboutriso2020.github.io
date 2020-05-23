---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
title: Angel Wing
next: /rumble-room
---

<div id="room3prints"></div>


{% assign room3print = site.works | where: 'roomtype', 'angel-wing-print' | sort: 'order' %}

<div class="prints room3 flex-row space-around aligncenter">
  {% for post in room3print %}
  <div class="print product hvr-bob {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}" alt="{{post.alttext}}"></a>
</div>
  {% endfor %}
</div>

<div id="room3zines" class="full-width">
{% assign room3zine = site.works | where: 'roomtype', 'angel-wing-zine' | sort: 'order' %}

<div class="zines room3 flex-row space-around aligncenter">
  {% for post in room3zine %}
   <div class="zine product hvr-bob {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}" alt="{{post.alttext}}"></a>
</div>
  {% endfor %}
</div>
</div>
