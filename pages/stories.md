---
layout: kz-default
permalink: "/archive/"
subheadline: subheadline
title: "All content in one place"
teaser: "Here you can see everything we've published so far in reverse chronological order."
header:
  title: ""
  image_fullwidth: landingpage_image.jpg
---
<div id="blog-index" class="row">
	<div class="small-12 columns t30">
		<h1>{{ page.title }}</h1>
		{% if page.teaser %}<p class="teaser">{{ page.teaser }}</p>{% endif %}

		<dl class="accordion" data-accordion>
			{% assign counter = 1 %}
			{% for post in site.posts limit:1000 %}
			<dd class="accordion-navigation">
			<a href="#panel{{ counter }}"><span class="iconfont"></span> {% if post.date %}{{ post.date | date: "%Y-%m-%d" }}{% endif %} &middot; <strong>{{ post.title }}</strong></a>
				<div id="panel{{ counter }}" class="content">
            <p>
                {% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% else post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}
                <a href="{{ post.url }}" title="Read {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a>
            </p>
				</div>
			</dd>
			{% assign counter=counter | plus:1 %}
			{% endfor %}
		</dl>
	</div><!-- /.small-12.columns -->
</div><!-- /.row -->



