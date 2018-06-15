---
layout: page
title: tags 

---

<div class="page-content wc-container">
	<div class="post">
		<h1>tags</h1>  
		{% highlight bash %}
		>weeklyTopic: something I've come across during the week that I'd like to explore further (i.e. news, research, code)
		>certReview: resources/notes for studying
		{% endhighlight bash %}
		<ul>
			{% for tag in site.tags %}
			<li><a href="{{ '/tag/' | append:tag[0] | relative_url }}">{{ tag[0] }}</a></li>
			{% endfor %}
		</ul>
	</div>
</div>