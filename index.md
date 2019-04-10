# トップ
- [メンバー](./members.md)
- [割り振り](./dates.md)

# 最近の投稿
<ul>
  {% for post in site.posts limit:10 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br>
      <font size="1">{{ post.date | date_to_string }}</font>
    </li>
  {% endfor %}
</ul>
[→ 全ての投稿](./posts.md)

# その他
- [Christian Diary](https://www.christian-diary.net/)
- 賛美伴奏講座
  - [チラシ1](./accompaniment1.md)
  - [チラシ2](./accompaniment2.md)
