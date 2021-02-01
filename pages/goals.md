---
layout: kz-page
title: "My goals"
permalink: "/goals/"
meta_description:
teaser: "Here are the goals I've set myself:"
header:
  title: ""
  image_fullwidth: main.jpg
widgets:
- url: /goals/samudra/
  image: samudra.jpg
  title: <a href="/goals/samudra/" target="_self">Improve waste management worldwide</a>
  dates: Since Feb 2020
  text: My goals are to reduce the environmental pollution and greenhouse gas emissions associated with waste, and to minimise the impact of waste on human and animal health. Currently I am working towards increasing the coverage of waste collection services in low and medium income countries.
- url:
  image: bio-maths.jpg
  title: Never stop making friends
  dates: Since Apr 2018
  text: I've noticed that at a certain age people stop making new friends. I realised that some day I might lose my ability to strike up a conversation with a stranger and grow it into a friendship. To avoid that, I decided to meet at least a couple of new people every week. <a href="https://lunchclub.com/" target="_blank">Lunchclub</a> has been a huge help. Apart from making new friends, this has changed my perspective on the world.
- url: /goals/big-cities/
  image: big_cities.jpg
  title: <a href="/goals/big-cities/" target="_self">Visit world's biggest cities</a>
  dates: Since Jun 2009
  text: I am a big city addict. I only truly feel alive when I live in a big city. Apart from London, my current home, I'd love to spend some time living in Mexico City, Singapore and Mumbai. My goal is to visit all cities with over 5 million people.
- url:
  image: pytorch.jpg
  title: Run a meetup group
  dates: Jun 2019 - Feb 2021
  text: I created the London PyTorch Meetup group together with <a href="https://www.mindstream-ai.com" target="_blank">Paul Dowling</a>. Our aim was to provide a platform where London-based ML professionals can share their experiences, make new friends, find advice and initiate collaborations. After 15 events both in person and online the group grew to 1000+ members.
- url: /goals/phd/
  image: phd.jpg
  title: <a href="/goals/phd/" target="_self">Get a PhD</a>
  dates: Sep 2015 - Sep 2019
  text: I spent 8 years in academia - a BSc in mathematics that I never finished, an MSc in mathematics and finally a PhD at UCL. If you are considering whether to do a PhD or if you are already doing one and feeling stuck, go get in touch. I'm good at asking the right questions to help you figure out what is right for you.
- url:
  image: airbnb.jpg
  title: Become a superhost
  dates: May 2018 - Sep 2018
  text: Ever wondered what the superhost label means on AirBnB? At the moment in my life when I was living alone and had flexible work hours, I decided to find out! It was a fun journey of meeting people from different walks of life, chatting late into the night over a bottle of wine, surprising my guests with a smell of pancakes in the morning. I got the label.

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
