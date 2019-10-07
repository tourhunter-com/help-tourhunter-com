---
layout: index2
permalink: /categories/
title: Categories
---
[//]: # wx: later use site.categories instead of hardcode, when those cats get filled

<div id="archives">
{% assign categories = 'Getting Started, Bookings, Marketplace, Suppliers, Notifications, Billing, Languages, Customers, Agents, For Developers, Account, Admin Panel, Updates' %}

{% for category in categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}


</div>
