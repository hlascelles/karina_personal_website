---
layout: default
title: "Karina's recipe library:"
permalink: "/kitchen/"
header: no
widgets:
- url: /kitchen/protein/
  image: food-protein.jpg
  title: <a href="/kitchen/protein/" target="_self">Protein-forward</a>
- url: /kitchen/fibre/
  image: food-fibre.jpg
  title: <a href="/kitchen/fibre/" target="_self">Fibre-forward</a>
- url: /kitchen/carb/
  image: food-carb.jpg
  title: <a href="/kitchen/carb/" target="_self">Carb-forward</a>

- url: /kitchen/dessert/
  image: food-dessert.jpg
  title: <a href="/kitchen/dessert/" target="_self">Dessert</a>
- url: /kitchen/notes/
  image: food-notes.jpg
  title: <a href="/kitchen/notes/" target="_self">Notes</a>
---

{% include _widget_grid_layout.html widgets=page.widgets articles_per_row=3 %}
