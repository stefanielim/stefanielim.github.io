---
layout: archive
permalink: /
title: ""
---

<div>
  <h1>Hello World</h1>
  <p>I'm Stef - a freelance full-stack web developer with a passion for learning and building things. Formerly a research chemist, I've shifted my focus to coding full-time after discovering it during my spare time and realising how much I enjoy it. I have experience with both WordPress- and Ruby/Rails-based projects but am always open to new technologies. I'm currently looking to join a development team so please don't hesitate to contact or find out more about me through the links above!</p>
</div>

<h2>Latest work</h2>
<div class="tiles wrapper">
{% for post in site.categories.portfolio limit: 4 %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

<div class='divider'><hr/></div>


{% if site.categories.blog %}
<h2>Latest posts</h2>
<div class="tiles wrapper">
{% for post in site.categories.blog limit: 4 %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
{% endif %}
