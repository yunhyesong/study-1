# point
```javascript
(중략)
...
&lt;script src="http://code.jquery.com/jquery-latest.js"&gt;&lt;/script&gt;
&lt;script&gt;
$(function () {
    // your script
    var selector = $('.btn');
    var funcName = function () {
        $(selector).css('background', 'yellow');
    };
    $(selector).on('click', funcName);
});
&lt;/script&gt;
&lt;/body&gt;
```
