---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---
[welcome]({{ "/welcome" | relative_url }})
[to jest test]({{ "/test" | relative_url }})

<ul>
  {% for post in site.posts reversed %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
