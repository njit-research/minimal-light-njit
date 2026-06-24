<ul style="list-style: none; padding: 0; margin: 0; display: inline-flex; float: right;">
  {% for link in site.data.navigation.main %}
    <li style="display: inline-block;">
      {% if link.right %}
        <a class="normal right" href="{{ link.url | relative_url }}">{{ link.title }}</a>
      {% else %}
        <a class="normal" href="{{ link.url | relative_url }}">{{ link.title }}</a>
      {% endif %}
    </li>
  {% endfor %}
</ul>
