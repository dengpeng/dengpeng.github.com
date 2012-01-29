---
layout: page
title: Peng.u.i.n
---
{% include JB/setup %}

{% for post in site.posts %}

<h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
<span class="label">{{ post.date | date_to_string }}</span>
{% for cat in post.categories %}
<span class="label notice">{{ post.categories }}</span>
{% endfor %}
</h2>
{{ post.content }}

{% endfor %}
