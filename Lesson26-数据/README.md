组件：数据
==========

## 知识点

* 组件的数据函数

### 组件的数据

为Vue.js组件添加数据，使组件可以动态显示各种数据，注意是数据函数，不是数据属性。

## 综合例

~~~html
<div id="App">
    <div>今天的天气是<today-weather/></div>
</div>
<script>
    Vue.component('today-weather', {
        template: '<strong>{{todayWeather}}</strong>',
        data: function(){
            return {
                todayWeather: '雨加雪'
            };
        }
    });
    var App = new Vue({
        el: '#App', 
    });
</script>
~~~

