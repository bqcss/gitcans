
**meta标签使用**
---------------
```
　<meta charset="UTF-8">
　　<meta content="keyword" name="keywords">
　　<meta content="description" name="description">
　　<meta name="renderer" content="webkit">
　　<meta http-equiv="X-UA-Compatible" content="IE=Edge,chrome=1">

　　<meta http-equiv="Cache-Control" content="no-siteapp" />

　　<meta name="viewport" content="width=device-width, initial-scale=1.0">


　　<meta name="apple-mobile-web-app-capable" content="yes" />
　　<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />


　　<meta name="format-detection" content="telephone=no,email=no" />



```


注释： 常用的有，编码、关键字.

优先使用webkit ，优先使用最新ie

no-siteapp 防止被百度转码篡改

为移动设备设定，viewport也可作为宽度单位，一些参数设定，width viewport 宽度(数值/device-width)，height viewport 高度(数值/device-height)，initial-scale 初始缩放比例，user-scalable 是否允许用户缩放(yes/no)，一般移动网页上都是设定设备宽度，默认不可缩放的；

apple-mobile-web-app-capable苹果专用
format-detection 不自动识别

以下就是一些uc、QQ强制的设定
```
　　<meta name="screen-orientation" content="portrait">
　　<meat name="x5-orientation" content="portrait">
　  <meta name="full-screen" content="yes">
　  <meta name="x5-fullscreen" content="true">
　  <meta name="browsermode" content="application">
　  <meta name="x5-page-mode" content="app">
　  <meta name="msapplication-tap-highlight" content="no">

```

------------------------
**整理的可以直接使用的**
//pc的
```

```

--------------

参考http://www.cnblogs.com/libin-1/p/5979300.html