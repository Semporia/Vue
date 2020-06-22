元素显示
=========

## 知识点

* v-show

### v-show

标记是否显示html元素。(注意：v-show设置的标记在html DOM中不会消失)

~~~html
<div id="App">
    <h1 v-show="result">任天堂新一代主机Switch</h1>
    <button @click="btnClick">考试成绩</button>
</div>
<script>
    var App = new Vue({
        el: '#App', 
        data: {
            result: true
        },
        methods: {
            btnClick: function(){
                this.result = !this.result;
            },
        },
    });
</script>
~~~

