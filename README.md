## ChineseCities
#### 中国省市选择插件
1.原生JS，不依赖jquery,zepto  
2.前端学习交流群：739574382
#### 快速入门
1.引用 ChineseCities.min.js  
2.拷贝以下布局结构
```html
<select id="province">
	<option value="请选择城市">请选择省份</option>
</select>
<select id="city">
	<option value="请选择城市">请选择城市</option>
</select>
```
3.创建ChineseCities对象:
```js
var chineseCities = new ChineseCities({
	'province':'province', //省份ID
	'city':'city', //城市ID
	'hasSelect': function(data){
		console.log(data);
	}//选择后的回调函数
});
```
#### API文档
参数名    |  默认值 | 说明
--        |    --   | --
province  |   null  | 省份下拉框ID
city      |   null  | 城市下拉框ID
hasSelect |   function(data){...}  | 选择后的回调，返回数据{'province':'省份名','city':'城市名'}

#### 案例展示
![查看演示](https://github.com/chaorenzeng/ChineseCities/blob/master/demo/index.gif)
