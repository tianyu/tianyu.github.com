---
layout: default
title: Latest Stuff
---
{% for post in site.posts limit:10 %}
{{ post.date | date_to_long_string }}
{: .post-date}
## [{{ post.title }}]({{ post.url }})
{% if post.abstract %}
{{ post.abstract }}
{: .abstract}
{% endif %}
{% endfor %}
