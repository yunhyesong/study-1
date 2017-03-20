# point
```html
<script src="http://code.jquery.com/jquery-latest.js"></script>
<script>
$(function () {
    var arrayObj = [['data1', 'data2', 'attribute2', 'attribute1', 'attribute20'], ['attribute19','data1', 'data2', 'attribute2', 'attribute1'], ['attribute20', 'attribute19','data1', 'data2', 'attribute2'], ['attribute1', 'attribute20', 'attribute19','data1','datalast']];

    // push
    var tagPush = [];
    tagPush.push('<table>');
    tagPush.push('<tbody>');
    for (var i = 0, max = arrayObj.length; i < max; i++) {
        tagPush.push('<tr>');
        for (var td = 0, tmax = arrayObj[i].length; td < tmax; td++) {
            tagPush.push('<td>' + arrayObj[i][td] + '</td>');
        }
        tagPush.push('</tr>');
    }
    tagPush.push('</tbody>');
    tagPush.push('</table>');
    $('.push_html').get(0).innerHTML = tagPush.join('');

    // +=
    var tagPlus = [];
    tagPlus += '<table>';
    tagPlus += '<tbody>';
    for (var i = 0, max = arrayObj.length; i < max; i++) {
        tagPlus += '<tr>';
        for (var td = 0, tmax = arrayObj[i].length; td < tmax; td++) {
            tagPlus += '<td>' + arrayObj[i][td] + '</td>';
        }
        tagPlus += '</tr>';
    }
    tagPlus += '</tbody>';
    tagPlus += '</table>';
    $('.plus_html').get(0).innerHTML = tagPlus;
});
</script>
</body>
```
