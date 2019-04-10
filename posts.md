# 投稿一覧
<ul>
  {% for post in site.posts limit:10 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br>
      <font size="1">{{ post.date }}</font>
    </li>
  {% endfor %}
</ul>
