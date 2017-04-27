---
# Notes:
# Only post.date until current date time are in site.posts
# Value of post.url is absolute (not relative)
menu_item_id: 0
---
# Posts
{% for post in site.posts %}
**{{ post.date | date: "%-d %B %Y"}}** -
[**{{ post.title }}**]({{ site.baseurl }}{{ post.url }}) -
By *{{ post.author }}*
{% endfor %}