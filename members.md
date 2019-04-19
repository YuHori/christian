# メンバー
<table border="1">
  <colgroup>
    <col width="30%" />
    <col width="70%" />
  </colgroup>
  <thead>
    <tr class="header">
      <th>名前</th>
      <th>性別</th>
        {% for x in site.data.members[0].conditions %}
          {% if x[0] == 'noon_catering' %}
            <td markdown="span" bgcolor="#FFFFFF">昼配膳</td>
          {% elsif x[0] == 'noon_washing' %}
            <td markdown="span" bgcolor="#FFFFFF">昼皿洗い</td>
          {% else %}
            <td markdown="span" bgcolor="#FFFFFF">夜配膳</td>
          {% endif %}
        {% endfor %}
    </tr>
  </thead>
  <tbody>
    {% for member in site.data.members %}
      <tr>
        <td markdown="span">{{ member.name }}</td>
        {% if member.gender == 1 %}
          <td markdown="span" bgcolor="#DDFFFF">兄弟</td>
        {% else %}
          <td markdown="span" bgcolor="#FFDDFF">姉妹</td>
        {% endif %}
          {% for x in member.conditions %}
            {% if x[1] == true %}
              <td markdown="span" bgcolor="#FFFFFF">:+1:</td>
            {% else %}
              <td markdown="span" bgcolor="#FFCCCC">:x:</td>
            {% endif %}
          {% endfor %}
      </tr>
    {% endfor %}
  </tbody>
</table>
