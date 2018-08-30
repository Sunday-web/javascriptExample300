#  javascriptExample300
说明
javascript网页特效经典300例 书中的案例

按照书中的例子，把每一个示例敲一遍，加深印象。

本人使用了[bulma](https://github.com/jgthms/bulma "bulma")简洁轻便的css框架 美化了样式。


## 第一章 网页特效
### 实例001  自动刷新页面

【实例描述】
> 有一些具有实效特点的网页，譬如股票价格、外汇牌价等，有这样的用户需求：定时地自动刷新网页，把最新数据展示给用户。那么这样的效果如何实现呢？JavaScript里有一个reload()函数可以实现这样的效果。

【实现代码】
```javascript
<script>
  function fresh() {
    window.location.reload();
  }
  setTimeout(fresh,10000);
</script>
```
### 实例002  让页面后退和前进

【实例描述】
> 在浏览一些文档形式的网页时（如html格式的技术说明书、html格式的小说等），往往需要给用户提供这样两个功能：前进和后退。用户通过单击按钮达到访问之前网页和之后网页的功能。

【实现代码】
```html
<a onclick="goForward()" class="button is-info">前进</a>
<a onclick="goBack()" class="button is-info">后退</a>
```
```javascript
<script>
  function goForward() {
    window.history.forward();
  }
  function goBack() {
      window.history.back();
    }
</script>
```
### 实例003  动态关闭页面

【实例描述】
> 网页有时候不需要等待用户的操作而自动关闭。例如，子窗口的作用已经结束，或者本窗口已经过期需要关闭。使用JavaScript可以很好地实现这个效果。

【实现代码】
```html
<a onclick="closeWin()" class="button is-info">关闭窗口</a>
```
```javascript
<script>
 function closeWin() {
   window.close();
  }
</script>
```
更多代码请查看示例文件