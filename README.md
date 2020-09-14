Customboxs [![npm version](https://badge.fury.io/js/custombox.svg)](https://badge.fury.io/js/custombox) [![Travis](https://travis-ci.org/dixso/custombox.svg?branch=master)](https://travis-ci.org/dixso/custombox) [![Coverage Status](https://coveralls.io/repos/github/dixso/custombox/badge.svg?branch=master)](https://coveralls.io/github/dixso/custombox?branch=master) ![npm License](http://img.shields.io/npm/l/custombox.svg "npm License")
==========

基于纯Javascript和CSS3构建模态对话框，支持多窗口。在开源的基础进行了修改，以支持z-index属性的支持。

期间如有冒犯原创造者，请联系我。

Usage
-----

npm:

```bash
npm install customboxs
```

Alternatively, download the package and reference the JavaScript and CSS files manually:

```html
<script src="custombox.min.js"></script>
<link rel="stylesheet" type="text/css" href="custombox.min.css">
```

Optional legacy file for along for the older browsers.
```html
<script src="custombox.legacy.min.js"></script>
```

## Basic usage
```js
new Custombox.modal({
  overlay: {
    color: "#000",  //遮罩层颜色
    opacity:0.5,    //遮罩层透明度，默认0.48
    zIndex: 9997    //遮罩层 z-index
  },
  content: {
    effect: 'fadein',
    target: '#modal'
  }
}).open();
```