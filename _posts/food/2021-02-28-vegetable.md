---
layout: kz-page
permalink: "/food/vegetable/"
title: Vegetable-centric dishes
header: no
widgets:
- url: /food/aubergine/
  image: aubergine.jpg
  title: <a href="/food/aubergine/" target="_self">Aubergine</a>
  text:

---

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
