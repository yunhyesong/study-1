# point
```html
<script src="http://code.jquery.com/jquery-latest.js"></script>
<script>
$(function () {
    var objFunc = {
        init : function () {
            this.setElements();
            this.bindEvents();
        },
        setElements : function () {
            this.obj = $('.obj');
            this.btn = $('.btn');
        },
        bindEvents : function () {
            this.btn.on('click', $.proxy(this.viewFunc, this));
        },
        viewFunc : function () {
            console.log(this);
            console.log('click');
        }
    };
    objFunc.init();
});
</script>
</body>
```
