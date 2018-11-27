---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
[welcome]({{ "/welcome" | relative_url }})
[about]({{ "/about" | relative_url }})

<ul>
  {% for post in site.pages reversed %}
  {% if post.title %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endif %}
  {% endfor %}
</ul>
