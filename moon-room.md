---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: room
title: Moon Room
next: /angel-wing
---

<div id="room2prints"></div>


{% assign room2print = site.works | where: 'roomtype', 'moon-room-print'  | sort: 'order' %}

<div class="prints room2 flex-row space-around aligncenter">
  {% for post in room2print %}
  <div class="print product hvr-hang {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}" alt="{{post.alttext}}"></a>
</div>
  {% endfor %}
</div>
<div id="room2zines" class="full-width">

{% assign room2zine = site.works | where: 'roomtype', 'moon-room-zine'  | sort: 'order' %}

<div class="zines room2 flex-row space-around aligncenter">
  {% for post in room2zine %}
   <div class="zine product hvr-bob {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}" alt="{{post.alttext}}"></a>
</div>
  {% endfor %}
</div>
</div>