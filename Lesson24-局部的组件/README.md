组件：局部的组件
================

## 知识点

* 组件的局部注册

### 组件

Vue.js的组件不仅可以单独声明注册使用，还可以在Vue实例中进行局部注册使用。

## 综合例

~~~html
<div id="App">
    <my-weather></my-weather>
</div>
<script>
    var WeatherComponent = {
        template: '<div>今天下雨，随它去吧！</div>'
    };
    var App = new Vue({
        el: '#App', 
        data: {
        },
        components: {
            'my-weather': WeatherComponent
        },
    });
</script>
~~~

