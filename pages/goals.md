---
layout: kz-page
title: "My goals"
permalink: "/goals/"
meta_description:
header:
  title: ""
  image_fullwidth: main.jpg
widgets:
- url: /goals/samudra/
  image: indonesia-landfill-thejakartapost-dot-com.jpg
  title: <a href="/goals/samudra/" target="_self">Samudra.world</a>
  text: Samudra is dedicated to solving global waste management challenges that don’t have a profitable solution.
- url: /goals/london-pytorch-meetup/
  image: pytorch_image.jpg
  title: <a href="/goals/london-pytorch-meetup/" target="_self">London PyTorch Meetup</a>
  text: The aim is to bring together London-based PyTorch users as well as other people working/interested in ML and AI.




---

I am currently working towards several goals.


<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
