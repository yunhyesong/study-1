# point
```html
<script src="http://code.jquery.com/jquery-latest.js"></script>
<script>
$(function () {
    var eventSelector = $('.btn'),
        animateSelector = $('.box');
        animateSelectorChild = animateSelector.children(),
        currentIndex = 0;
    var funcName = function () {
        animateSelectorChild.eq(currentIndex).css('background', 'yellow');
        currentIndex += 1;
    };
    eventSelector.on('click', funcName);
});
</script>
</body>
```
