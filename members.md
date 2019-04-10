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
<th>条件</th>
</tr>
</thead>
<tbody>
{% for member in site.data.members %}
<tr>
<td markdown="span">{{ member.name }}</td>
<td markdown="span">{{ member.gender }}</td>
<td markdown="span">{{ member.conditions }}</td>
</tr>
{% endfor %}
</tbody>
</table>
