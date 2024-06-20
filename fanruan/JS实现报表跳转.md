# JS实现报表跳转

报表可以通过配置超链接实现跳转，但是也有其他方式实现，如在参数面板框上添加一个按钮实现。

配置按钮的点击事件

```js
window.open(encodeURI(encodeURI("${servletURL}?viewlet=/xxx/重构计划/月度接单发货情况.cpt")))
```

如果是需要填报预览，则在后面拼接参数。如下

```js
window.open(encodeURI(encodeURI("${servletURL}?viewlet=/苏日锐/电子工程/电子工程群组目标填报.cpt&op=write")))
```

