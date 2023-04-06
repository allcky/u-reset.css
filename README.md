# u-reset.css
> 这是一个小而美的现代CSS样式重置优秀实践！

This is a small and beautiful modern CSS style reset excellent practice!

![npm-version](https://img.shields.io/npm/v/u-reset.css.svg "当前版本号")
![npm-download](https://img.shields.io/npm/dm/u-reset.css.svg "NPM月下载量")
![cnpm-download](https://npm.taobao.org/badge/d/u-reset.css.svg "CNPM月下载量")
![npm-installsize](https://badgen.net/packagephobia/install/u-reset.css "安装大小")
![npm-minsize](https://img.shields.io/bundlephobia/min/u-reset.css.svg "生产版本大小")
![npm-license](https://img.shields.io/npm/l/u-reset.css.svg "许可")

## 特性
1. 统一终端(windows,mac,linux)中文/英文字体
2. 统一相关标签预设样式
3. 支持REM布局，且支持自定义设计稿尺寸
4. 支持单行、多行文本的溢出显示省略号
5. 支持网站灰度模式、色弱模式
6. 支持清除浮动

## 安装导入
```
npm install u-reset.css
```
构建工具导入模块：
```
// es module
import "u-reset.css";
```
> 提示：默认导入压缩`u-reset.min.css`文件，大小仅为1KB。
## 下载引入

点击下载：https://unpkg.com/u-reset.css

```
<link rel="stylesheet" href="path/u-reset.min.css">
```

浏览器CDN引入
```
// CDN
<link rel="stylesheet" href="https://unpkg.com/u-reset.css">
```
## 功能使用
### REM布局
支持REM布局，默认适配750px、1080px设计稿，且支持自定义设计稿尺寸。

使用流程：
1. 引入 u-reset.css 
2. 在`<html>`添加 `rem` 属性
3. 将设计稿尺寸px转换CSS rem单位(比例：design 100px : css 1rem)

#### 尺寸比例
```
design 100px  ->  css 1rem
```
如：
```
design 100px  ->  css 1rem
design 150px  ->  css 1.5rem
design 284px  ->  css 2.84rem
```

#### 默认适配尺寸
使用需在html标签添加属性rem
```
<html rem></html>
```
> 提示：默认适配设计稿尺寸为：移动端 750px、PC端 1080px

#### 自定义适配尺寸

示例：自定义适配尺寸，如设计稿 1440px，则在html标签添加如下代码：
```
***.html
<html rem style="--design-width: 1440px">
</html>
```
> 提示：`--design-width` 为自定义CSS变量，通过该变量自定义设计稿尺寸。

### 文本的溢出显示省略号

- 添加`class="hidden1"`  1行溢出出现省略号
- 添加`class="hidden2"`  2行溢出出现省略号
- ...
- 添加`class="hidden5"`  5行溢出出现省略号

示例：
```
<div class="hidden1"></div>
<div class="hidden2"></div>
...
<div class="hidden5"></div>
```

### 清除浮动
在待清除浮动元素添加`clearfix` 类名即可。

示例：
```
<div class="clearfix"></div>
```
### 灰度模式
> 支持 属性 与 class 两种方式

给html 添加 gray-model 属性
```
<html gray-model>
```
或者，给html 添加 gray-model 类名
```
<html class="gray-model">
```
### 色弱模式
> 支持 属性 与 class 两种方式

给html 添加 color-weak-model 属性
```
<html color-weak-model>
```
或者，给html 添加 color-weak-model 类名
```
<html class="color-weak-model">
```
## 浏览器支持

![Chrome](https://raw.github.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png) | ![Firefox](https://raw.github.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png) | ![Safari](https://raw.github.com/alrra/browser-logos/master/src/safari/safari_48x48.png) | ![Opera](https://raw.github.com/alrra/browser-logos/master/src/opera/opera_48x48.png) | ![Edge](https://raw.github.com/alrra/browser-logos/master/src/edge/edge_48x48.png) | ![IE](https://raw.github.com/alrra/browser-logos/master/src/archive/internet-explorer_9-11/internet-explorer_9-11_48x48.png) |
--- | --- | --- | --- | --- | --- |
Latest √ | Latest √ | Latest √ | Latest √ | Latest √| × |

> 提示：不支持IE浏览器！

## 版本历史
- V2.0.0 **去除IE兼容**，**新增灰度、色弱模式**，**REM支持自定义尺寸**，清除浮动，重置标签预设样式，统一终端字体
- V1.0.0 兼容IE，REM，清除浮动，重置标签预设样式，统一终端字体