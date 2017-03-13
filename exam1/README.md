# point
```html
<script src="http://code.jquery.com/jquery-latest.js"></script>
<script>
$(function () {
    // your script
    var eventSelector = $('.btn'),
        animateSelector = $('.box');
    var funcName = function () {
        animateSelector.css('background', 'yellow');
    };
    eventSelector.on('click', funcName);
});
</script>
</body>
```
