---
title: swan.setClipboardData
header: develop
nav: api
sidebar: swan-setClipboardData
---

 

**解释**：设置系统剪贴板的内容

**百度APP中扫码体验：**

<img src="https://b.bdstatic.com/miniapp/assets/images/doc_demo/clipboardData.png"  class="demo-qrcode-image" />


**方法参数**：Object object

**`object`参数说明**：

|属性名 |类型  |必填 | 默认值 |说明|
|---- | ---- | ---- | ----|----|
|data  |  String  |是  | | 需要设置的内容|
|success |Function  |  否  | | 接口调用成功的回调函数|
|fail  | Function  |  否  | | 接口调用失败的回调函数|
|complete   | Function   | 否  | | 接口调用结束的回调函数（调用成功、失败都会执行）|

**图片示例**：

<div class="m-doc-custom-examples">
    <div class="m-doc-custom-examples-correct">
        <img src="https://b.bdstatic.com/miniapp/images/setClipboardData.gif">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>     
</div>

**代码示例**：

<a href="swanide://fragment/ea39eea822a594a02b300d528c37da981574214762675" title="在开发者工具中预览效果" target="_self">在开发者工具中预览效果</a>

* 在 js 文件中

```js
Page({
    setClipboardData() {
        swan.setClipboardData({
            data: 'xxxxxx',
            success: () => {
                swan.showToast({
                    title: '设置成功'
                });
            },
            fail: err => {
                swan.showToast({
                    title: '设置失败'
                });
                console.log('setClipboardData fail', err);
            }
        });
    }
});   
               
```
 
#### 错误码
* Andriod

|错误码|说明|
|--|--|
|202|解析失败，请检查参数是否正确      |

* iOS

|错误码|说明|
|--|--|
|202|解析失败，请检查参数是否正确      |

