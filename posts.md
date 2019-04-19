# 投稿一覧
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a><br>
      <font size="1">{{ post.date | date_to_string }}</font>
    </li>
  {% endfor %}
</ul>
