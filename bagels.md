---
layout: default
title: Everything (about) bagels
feature_image: "/assets/img/home_cover.jpg"
---

{% for bagels in site.bagels %}


<a href="{{ bagels.url | prepend: site.baseurl }}">
        <h2>{{ bagels.title }}</h2>
</a>

<p class="post-excerpt">{{ bagels.description | truncate: 160 }}</p>

{% endfor %}
