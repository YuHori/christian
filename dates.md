# 日程表
<table border="1">
  <colgroup>
    <col width="30%" />
    <col width="70%" />
  </colgroup>
  <thead>
    <tr class="header">
      <th>日付</th>
        {% for x in site.data.dates[0].conditions %}
          <th>{{ x[0] }}</th>
        {% endfor %}
    </tr>
  </thead>
  <tbody>
    {% for date in site.data.dates %}
    <tr>
      <td markdown="span">{{ date.date }}</td>
        {% for x in date.conditions %}
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
