# トップ
- [メンバー](./members.md)
- [日程表](./dates.md)
- :sunny: 担当表作成(準備中)
- [聖書表](./bible_table.md)

# 最近の投稿
<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a><br>
      <font size="1">{{ post.date | date_to_string }}</font>
    </li>
  {% endfor %}
</ul>
[→ 全ての投稿](./posts.md)

# その他
- [ラビリンスウォーク体験](./labyrinth_walk.md)
- 賛美伴奏講座
  - [チラシ1](./accompaniment1.md)
  - [チラシ2](./accompaniment2.md)
- [祈祷会](./prayer_party.md)

# リンク
- [Christian Diary](https://www.christian-diary.net/)
