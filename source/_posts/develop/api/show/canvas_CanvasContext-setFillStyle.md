---
title: CanvasContext.setFillStyle
header: develop
nav: api
sidebar:  canvas_CanvasContext_setFillStyle
---
 

**解释**：设置填充色。

**百度APP中扫码体验：**

<img src="https://b.bdstatic.com/miniapp/assets/images/doc_demo/pages_createCanvasContext.png"  class="demo-qrcode-image" />

**方法参数**： [Color](/develop/api/canvas_color/) color

**图片示例**：

![图片](../../../../img/api/canvas/setFillStyle.png)

**代码示例**：

<a href="swanide://fragment/130dc92945ea6869f8d81213f6e780e71573717221468" title="在开发者工具中预览效果" target="_self">在开发者工具中预览效果</a>

```js
const canvasContext = this.createCanvasContext('myCanvas');
canvasContext.setFillStyle('blue');
canvasContext.fillRect(30, 30, 150, 75);
canvasContext.draw();
```


