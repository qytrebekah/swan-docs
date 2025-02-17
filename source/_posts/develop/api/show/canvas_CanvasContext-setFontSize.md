---
title: CanvasContext.setFontSize
header: develop
nav: api
sidebar: canvas_CanvasContext_setFontSize
---
 
**解释**：设置字体的字号。

**百度APP中扫码体验：**

<img src="https://b.bdstatic.com/miniapp/assets/images/doc_demo/pages_createCanvasContext.png"  class="demo-qrcode-image" />

**方法参数**：Number fontSize

`fontSize`参数说明：字体的字号 

**图片示例**：

<div class="m-doc-custom-examples">
    <div class="m-doc-custom-examples-correct">
        <img src="https://b.bdstatic.com/miniapp/image/setFontSize.png">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>
    <div class="m-doc-custom-examples-correct">
        <img src=" ">
    </div>     
</div>

**代码示例**：

<a href="swanide://fragment/94b824f65c4ffa7f78b40f0d6f10bd1a1573724116782" title="在开发者工具中预览效果" target="_self">在开发者工具中预览效果</a>

```js
const canvasContext = swan.createCanvasContext('myCanvas');

canvasContext.setFontSize(20);
canvasContext.fillText('20', 20, 20);
canvasContext.setFontSize(30);
canvasContext.fillText('30', 40, 40);
canvasContext.setFontSize(40);
canvasContext.fillText('40', 60, 60);
canvasContext.setFontSize(50);
canvasContext.fillText('50', 90, 90);

canvasContext.draw();
```
