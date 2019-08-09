---
title: Post by Tag
permalink: /tagview/
active: archivebytag
sitemap: false
layout: page
---

{% assign tags = site.tags | sort %}
{% assign sorted_posts = site.posts | sort: 'title' %}
<div> 
{% for tag in tags %}
<a href="#{{ tag | first | slugify }}">{{ tag | first | replace: '-', ' ' }}({{ tag | last | size }})</a>{% if forloop.last == false %} • {% endif %}{% endfor %}
</div>
<p>&nbsp;</p>

{% for tag in tags %}
<p><a name="{{ tag | first | slugify }}"></a>&nbsp;</p>
<h3 class="archivetitle">{{ tag | first | replace:'-', ' ' }} <i class="badge">{{ tag | last | size }}</i> </h3>

<ul>{% for post in sorted_posts %}{%if post.tags contains tag[0]%}<li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a> {% if post.author %} • {{ post.author }}{% endif %}{% if post.date %} • {{ post.date | date: "%B %e, %Y" }}{% endif %}</li>{%endif%}{% endfor %}</ul>
{% endfor %}