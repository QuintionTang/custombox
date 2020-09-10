Custombox [![npm version](https://badge.fury.io/js/custombox.svg)](https://badge.fury.io/js/custombox) [![Travis](https://travis-ci.org/dixso/custombox.svg?branch=master)](https://travis-ci.org/dixso/custombox) [![Coverage Status](https://coveralls.io/repos/github/dixso/custombox/badge.svg?branch=master)](https://coveralls.io/github/dixso/custombox?branch=master) ![npm License](http://img.shields.io/npm/l/custombox.svg "npm License")
==========

Modal dialog effects with transitions CSS3.

Usage
-----

Build

```bash
sudo npm run release
```


You can install custombox through bower:

```bash
bower install custombox
```

Or through npm:

```bash
npm install custombox
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