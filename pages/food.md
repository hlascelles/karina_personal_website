---
layout: kz-page
title: Recipes for those who don't like to cook
permalink: "/food/"
meta_description:
teaser: All recipe websites I've come across have one thing in common - they are made by people who love to cook. Here I made a list of my favourite recipes to share with people like me, who would rather go out for a run than cook. The recipe instructions are optimised for speed and using less items you'll need to wash later. All amounts are in grams, even for liquids, so you can add everything into a container on the scales, without using any measuring devices. No photos included because it doesn't matter how it looks like; the goal is to make nutritious and satisfying meals. You won't start liking to cook, but you'll love the food you make and how it makes you feel.
header:
  title: ""
  image_fullwidth: main.jpg
widgets:
- url: /food/vegetable/
  image: vegetables.jpg
  title: <a href="/food/vegetable/" target="_self">Vegetable-centric dishes</a>
  text:

- url: /food/carbs-fats/
  image: carbs-fats.jpg
  title: <a href="/food/carbs-fats/" target="_self">Party of carbs and fats</a>
  text:

- url: /food/cake/
  image: cake.jpg
  title: <a href="/food/cake/" target="_self">Oven baked happiness</a>
  text:

- url: /food/sweet/
  image: sweet-stuff.jpg
  title: <a href="/food/sweet/" target="_self">Sweet stuff</a>
  text:

- url: /food/start/
  image: start.jpg
  title: <a href="/food/start/" target="_self">Where to start</a>
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
