---
layout: default
title: Green beans
permalink: "/kitchen/green-beans/"
header: no
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
				{% if post.greenbean_post == true %}
					<dd class="accordion-navigation">
						<a href="#panel{{ counter }}"><span class="iconfont"></span><strong>{{ post.title }}</strong></a>
						<div id="panel{{ counter }}" class="content">
           					<p>{{ post.content }}</p>
						</div>
					</dd>
				{% assign counter=counter | plus:1 %}
				{% endif %}
			{% endfor %}
		</dl>
	</div><!-- /.small-12.columns -->
</div><!-- /.row -->



 