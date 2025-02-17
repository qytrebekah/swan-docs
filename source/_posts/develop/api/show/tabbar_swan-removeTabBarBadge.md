---
title: swan.removeTabBarBadge
header: develop
nav: api
sidebar: tabbar_swan-removeTabBarBadge
---
  

**解释**：移除tabBar某一项右上角的文本。

**百度APP中扫码体验：**

<img src="https://b.bdstatic.com/miniapp/assets/images/doc_demo/fragment_TabBarBadge.png"  class="demo-qrcode-image" />

**方法参数**：Object object

**`object`参数说明**：

|属性名 |类型  |必填 | 默认值 |说明|
|---- | ---- | ---- | ----|----|
|index |Number  |是| |tabBar的哪一项，从左边算起|
|success| Function |   否  | | 接口调用成功的回调函数|
|fail   | Function |   否  | | 接口调用失败的回调函数|
|complete  |  Function  |  否 | |  接口调用结束的回调函数（调用成功、失败都会执行）|

**图片示例**：

<div class="m-doc-custom-examples">
    <div class="m-doc-custom-examples-correct">
        <img src="https://b.bdstatic.com/miniapp/image/tabbarbadge.gif">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>     
</div>

**代码示例**：

<a href="swanide://fragment/6fa8cb5655d510b33220f6203e4e02c51574137194069" title="在开发者工具中预览效果" target="_self">在开发者工具中预览效果</a>

* 在 swan 文件中

```html
<view class="wrap">
    <button type="primary" bindtap="setTabBarBadge">setTabBarBadge</button>
    <button type="primary" bindtap="removeTabBarBadge">removeTabBarBadge</button>
</view>
```

* 在 js 文件中

```js
Page({
    setTabBarBadge() {
        swan.setTabBarBadge({
            index: 0,
            text: '文本'
        });
    },
    removeTabBarBadge() {
        swan.removeTabBarBadge({
            index: 0,
            success: function () {
                console.log('removeTabBarBadge success');
            },
            fail: function (err) {
                console.log('removeTabBarBadge fail', err);
            }
        });
    }
});
```
#### 错误码

* Andriod



|错误码|说明|
|--|--|
|1001|执行失败      |



* iOS


|错误码|说明|
|--|--|
|202|解析失败，请检查参数是否正确   |
|1001|当前页面不含tabbar|


