---
layout: null
---

# [deificx.github.io](https://deificx.github.io)

{% include about.md %}

## Projects
{% for post in site.posts %}
### {{ post.title }} ({{ post.date | date: "%b %-d, %Y" }})

{% if post.image %}<img src="https://github.com/deificx/deificx.github.io/blob/master{{ post.image }}" alt="{{ post.title }}">{% endif %}

- type: {{ post.type }}
{% if post.location %}- location: {{ post.location }}{% endif %}
{% if post.code %}- repository: {{ post.code }}{% endif %}
{% if post.blog %}- blog: {{ post.blog }}{% endif %}

{% endfor %}
