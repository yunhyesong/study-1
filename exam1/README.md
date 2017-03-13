# point
```html
<script src="http://code.jquery.com/jquery-latest.js"></script>
<script>
$(function () {
    // your script
    var selector = $('.btn');
    var funcName = function () {
        selector.css('background', 'yellow');
    };
    selector.on('click', funcName);
});
</script>
</body>
```
