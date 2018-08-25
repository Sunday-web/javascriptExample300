#  javascriptExample300
说明
javascript网页特效经典300例 书中的案例

按照书中的例子，把每一个示例敲一遍，加深印象。

本人使用了[bulma](https://github.com/jgthms/bulma "bulma")简洁轻便的css框架 美化了样式。

## 第一章 网页特效
实例001  自动刷新页面

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
