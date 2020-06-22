Class对象绑定
=============

## 知识点

* v-bind:class

### v-bind:class

为html标记绑定样式单class对象。

~~~html
<div id="App">
    <div :class="myClass">红色文本</div>
    <button @click="btnClick">改变class吧</button>
</div>
<script>
    var App = new Vue({
        el: '#App',
        data: {
            myClass: {
                active: true,
                big: true,
            },
        },
        methods: {
            btnClick: function(){
								this.myClass.active = false;
                this.myClass.big = false;
								//this.myClass.active = !this.myClass.active;(取反值)
                //this.myClass.big = !this.myClass.big;(取反值)
            },
        },
    });
</script>
~~~

