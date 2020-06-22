Class绑定
==========

## 知识点

* v-bind:class

### v-bind:class

为html标记绑定样式单class属性。

~~~html
<div id="App">
    <div v-bind:class="{active:isActive}">红色文本1</div>
    <div :class="{active:isActive}">红色文本2</div>
    <button @click="btnClick">改变class吧</button>
</div>
<script>
    var App = new Vue({
        el: '#App',
        data: {
            isActive: true,
        },
        methods: {
            btnClick: function(){
                this.isActive = false;
								//this.isActive = !this.isActive （取反值）
            },
        },
    });
</script>
~~~

