---
layout: default
title: Schedule
description: A site about the sunset farm projects
navclass: enterprises
navtitle: enterprises
---


<div class="banner" style="background-image: url(/images/backgrounds/sunset.jpg);">
	<hgroup>
		<h1>Enterprises</h1>
	</hgroup>
</div>

<ul class="blogposts">
	{% for post in site.projects %}
		<li>
			<a href="{{ post.url }}">
				<div class="postbanner" style="background-image: url({{ post.bannerimage_path }});"></div>
				<!--<h3>{{ post.category }}</h3>-->
				<h2>{{ post.title }}</h2>
				{{ post.excerpt }}
			</a>
		</li>
	{% endfor %}
</ul>