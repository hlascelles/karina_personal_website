---
layout: default
permalink: "/rubbish-stories/"
title: Rubbish stories
teaser: "Here you can find snapshots of interesting days in my waste management career and find out how I got into waste management in the first place. <br/> <br/> July 2021: Since the pandemic started all of my work has been online, video calls don't make good stories. The most exciting thing that happened recently was in Isla Mujeres, Mexico. I approached a security guard at a landfill - the only waste management facility on the island. I wanted to say 'I can see a big pile of plastic furniture there - is that for recycling?', but he only listened to the first couple of words in my broken Spanish and mistook it for 'can I see?'. 'Sure, go see whatever you want,' he replied. I walked in, I was the only person in the whole landfill apart from the security guard. I walked up to the very top of the rubbish pile and had a good look around. This was my first time in a landfill with no protective equipment, I'm sure it's not the last."
header:
  title: ""
  image_fullwidth: rubish-stories.jpg

---

<div id="blog-index" class="row">
	<div class="small-12 columns t30">
		<h1>{{ page.title }}</h1>
		{% if page.teaser %}
			<p class="teaser">{{ page.teaser }}</p>
		{% endif %}
		<dl class="accordion" data-accordion>
			{% assign counter = 1 %}
			{% for post in site.posts limit:1000 %}
				{% if post.story_post == true %}
					<dd class="accordion-navigation">
						<a href="#panel{{ counter }}"><span class="iconfont"></span> {% if post.date %}{{ post.date | date: "%Y-%m-%d" }}{% endif %} &middot; <strong>{{ post.title }}</strong></a>
						<div id="panel{{ counter }}" class="content">
           					<p>{% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% else post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %} <a href="{{ post.url }}" title="Read {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a></p>
						</div>
					</dd>
				{% assign counter=counter | plus:1 %}
				{% endif %}
			{% endfor %}
		</dl>
	</div><!-- /.small-12.columns -->
</div><!-- /.row -->



 