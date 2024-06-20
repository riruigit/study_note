# 帆软自定义按钮实现发送POST请求

常见的场景如下：填报完毕推送到某一个人的企业微信，通过API调起对用的调度任务等。

## 引入jquery.js

需要下载jquery.js，然后上传到服务器对应的路径上。因为需要用到AJAX。

## 配置对应的JS

```js
    $.ajax({
        url: 'http://api.xxx.com.cn:9880/push2huangfen/',
        type: 'POST',
        data: JSON.stringify({
            url: "xxx"
            , title: "新废水站每日填报明细"
        }),
        dataType: 'json'
    });
```

## 帆软配置

在web页面属性上面，添加一个自定义按钮，然后设置对应的JS事件即可。