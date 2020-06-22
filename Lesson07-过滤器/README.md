过滤器
=======

## 知识点

* filters

### filters

格式化变量内容的输出。（日期格式化，字母大小写，数字再计算等等）

~~~html
<div id="App">
    <p>{{message}}</p>
    <p>{{message | toupper }}</p>
    <hr>
    <p>现在的vue.js学习进度是{{num}}({{num | topercentage}})。</p>
</div>
<script>
    var App = new Vue({
        el: '#App',
        data: {
            message: 'hello vue.js world.',
            num: 0.3
        },
        filters: {
            toupper: function(value){
                return value.toUpperCase();
            },
            topercentage: function(value){
                return value * 100 + '%';
            },
        },
    });
</script>
~~~

