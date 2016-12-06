# areaMap
百度地图API——实现北京市各行政区房产数据展示
## 特点
### 支持热力图显示：使用百度地图热力图API实现
### 前端组件化：js+css+html
### 目前使用测试数据：可通过注释掉的ajax方法请求后台数据

## 使用方法
### html：
```html
link rel="stylesheet" type="text/css" href="/stylesheets/areaMap.css">
<script type="text/javascript" src="http://api.map.baidu.com/api?v=2.0&ak=iyPuuhgLuXn9kgnqiyC32m6Z"></script>
<!--百度地图容器-->
  <div class="areaMap" style="border:#ccc solid 1px;" id="dituContent"></div>

```
### script：
```javascript
 //调用areaMap jQuery组件，实例化JS对象
 var areaMap =  $("#dituContent").areaMap({
                level:'province'   //地图级别为北京市
          });
 //调用初始化地图的方法
 areaMap.init();
 //调用生成热力图的方法
 var overlay = areaMap.heatmap();

```
