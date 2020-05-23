---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: solarium
next: /moon-room

---

<div id="room1prints"></div>


{% assign room1print = site.works | where: 'roomtype', 'solarium-print'  | sort: 'order' %}

<div class="prints room1 flex-row space-around aligncenter">
  {% for post in room1print %}
  <div class="print product hvr-hang {{post.imgsize}}">
   <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>

<div id="room1zines" class="full-width ">
{% assign room1zine = site.works | where: 'roomtype', 'solarium-zine'  | sort: 'order' %}

<div class="zines room1 flex-row space-around aligncenter">
  {% for post in room1zine %}
   <div class="zine product hvr-hang {{post.imgsize}}">
  	 <a href="{{site.baseurl}}{{post.url}}"><img src="{{site.baseurl}}/img/products/{{post.img1}}"></a>
</div>
  {% endfor %}
</div>
</div>
