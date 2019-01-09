# u-reset.css
> 这是一个简洁的重置样式库。

This is a reset style library.

![npm-version](https://img.shields.io/npm/v/u-reset.css.svg)
![npm-download](https://img.shields.io/npm/dm/u-reset.css.svg)
![npm-installsize](https://packagephobia.now.sh/badge?p=u-reset.css)
![npm-minsize](https://img.shields.io/bundlephobia/min/u-reset.css.svg)
![npm-devdependencies](https://img.shields.io/david/dev/allcky/u-reset.css.svg)
![npm-dependencies](https://img.shields.io/david/allcky/u-reset.css.svg)
![npm-license](https://img.shields.io/npm/l/u-reset.css.svg)


## Install
```
npm install u-reset.css
```
## Download

https://unpkg.com/u-reset.css

## Example
```
//module
require("u-reset.css");
import "u-reset.css";

//CDN
<link rel="stylesheet" href="https://unpkg.com/u-reset.css">
```
## REM布局
> 引入`u-reset.css`就可以进行REM布局。<br/>

如果设计稿测量的宽度为 100px => 1rem。
```
design 100px  ->  css 1rem
design 150px  ->  css 1.5rem
design 284px  ->  css 2.84rem
```
> 注意：需在html标签添加属性rem(\<html rem="750">\</html>)。

目前添加的适配尺寸为： 750px、1080px

示例
```
***.html
<html rem="750">
</html>
```
```
***.css
.container{
    width:1rem;
    height:1.54rem;
}
.col{
    width:0.36rem;
    height:0.52rem;
}
```

## 文本的溢出显示省略号

- 添加`class="hidden1"`  1行溢出出现省略号
- 添加`class="hidden2"`  2行溢出出现省略号
- ...
- 添加`class="hidden5"`  5行溢出出现省略号

```
<div class="hidden1"></div>
<div class="hidden2"></div>
...
<div class="hidden5"></div>
```

## 清除浮动 
```
<div class="clearfix"></div>
```

## 特性
1. 基于CSS的REM布局
2. 统一终端中文/英文字体
3. 文本的溢出显示省略号
4. 清除浮动 

## Browser support

![Chrome](https://raw.github.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) | ![Firefox](https://raw.github.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) | ![Safari](https://raw.github.com/alrra/browser-logos/master/src/safari/safari_48x48.png) | ![Opera](https://raw.github.com/alrra/browser-logos/master/src/opera/opera_48x48.png) | ![Edge](https://raw.github.com/alrra/browser-logos/master/src/edge/edge_48x48.png) | ![IE](https://raw.github.com/alrra/browser-logos/master/src/archive/internet-explorer_9-11/internet-explorer_9-11_48x48.png) |
--- | --- | --- | --- | --- | --- |
Latest √ | Latest √ | Latest √ | Latest √ | Latest √| 8+ √


