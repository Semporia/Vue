组件：传递变量
==============

## 知识点

* 为组件传递变量数据

### 组件的数据

制作可接受变量参数的组件。

## 综合例

~~~html
<div id="App">
    <div>请输入您的名字：<input v-model="myname"></div>
    <hr/>
    <say-hello :pname="myname" />
</div>
<script>
    Vue.component('say-hello', {
        props: ['pname'],
        template: '<div>你好，<strong>{{pname}}</strong>！</div>',
    });
    var App = new Vue({
        el: '#App', 
        data: {
            myname: 'Koma'
        }
    });
</script>
~~~

