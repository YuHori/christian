# 担当
<table border="1">
<colgroup>
<col width="30%" />
<col width="70%" />
</colgroup>
<thead>
<tr class="header">
<th>名前</th>
<th>条件</th>
</tr>
</thead>
<tbody>
{% for date in site.data.dates %}
<tr>
<td markdown="span">{{ date.date }}</td>
<td markdown="span">{{ date.conditions }}</td>
</tr>
{% endfor %}
</tbody>
</table>
