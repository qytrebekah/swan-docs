---
title: swan.setTabBarStyle
header: develop
nav: api
sidebar: tabbar_swan-setTabBarStyle
---

 
**解释**：动态设置 tabBar 的整体样式

**百度APP中扫码体验：**

<img src="https://b.bdstatic.com/miniapp/assets/images/doc_demo/fragment_setTabBarStyle.png"  class="demo-qrcode-image" />

**方法参数**：Object object

**`object`参数说明**：

|属性名 |类型  |必填 | 默认值 |说明|
|---- | ---- | ---- | ----|----|
|color |HexColor | 否| |tab 上的文字默认颜色|
|selectedColor |HexColor | 否| |tab 上的文字选中时的颜色|
|backgroundColor |HexColor | 否| | tab 的背景色|
|borderStyle |String |否 | | tabbar上边框的颜色， 有效值 black/white|
|success| Function | 否 | |  接口调用成功的回调函数|
|fail   | Function  | 否 | |接口调用失败的回调函数|
|complete  |  Function  |  否| |接口调用结束的回调函数（调用成功、失败都会执行）|

**图片示例**：

<div class="m-doc-custom-examples">
    <div class="m-doc-custom-examples-correct">
        <img src="https://b.bdstatic.com/miniapp/image/settabbarstyle.gif">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>     
</div>

**代码示例**：

<a href="swanide://fragment/44d27e9d57b8848544201181fe547cb01574137906215" title="在开发者工具中预览效果" target="_self">在开发者工具中预览效果</a>

* 在 swan 文件中

```html
<view class="wrap">
    <button type="primary" bindtap="setTabBarStyle">setTabBarStyle</button>
</view>
```

* 在 js 文件中

```js
Page({
    setTabBarStyle() {
        swan.setTabBarStyle({
            color: '#000',// black
            selectedColor: '#FF0000',// red
            backgroundColor: '#FFFFBD',
            borderStyle: 'black',
            success: function () {
                console.log('setTabBarStyle success');
            },
            fail: function (err) {
                console.log('setTabBarStyle fail', err);
            }
        });
    }
});
```


#### 错误码

* Andriod

|错误码|说明|
|--|--|
|1001|执行失败   |

* iOS

|错误码|说明|
|--|--|
|1001|当前页面不含tabbar  |
