
hover对移动设备的效果无效，或者有些有效，但效果不对；

--------------

**-webkit-tap-highlight-color** 私有属性，其实safari 微信，给a或者js有事件的标签上默认加个浅灰色；

可以通过设置去除或者修改；


------------


**使用js** 的`touchStart` `touchMove`` touchEnd `结合css可以很容易定制

以下代码用jq

```
$(document).on("touchstart", ".action-btn:not(.disable)", function (e) {
    var $this = $(this);
    var flag = true;
    //遍历子类
    $this.find("*").each(function () {
        //查看有没有子类触发过active动作
        if ($(this).hasClass("active")) flag = false;
    });
    //如果子类已经触发了active动作，父类则取消active触发操作
    if (flag) $this.addClass("active");

});
$(document).on("touchmove", ".action-btn:not(.disable)", function (e) {
    if ($(this).hasClass("active")) $(this).removeClass("active");
});
$(document).on("touchend", ".action-btn:not(.disable)", function (e) {
    if ($(this).hasClass("active")) $(this).removeClass("active");
});
```

----------------

js升级版 `水波纹` 代码

**canves 实现**

**css3实现**

个人觉得css3实现更好

[代码示例](http://ogm1hxbsu.bkt.clouddn.com/shui.html)


