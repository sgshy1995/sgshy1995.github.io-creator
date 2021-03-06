---
title: "用CSS做一个简单的三角形"
date: 2019-08-30T16:22:42+08:00
lastmod: 2019-08-30T18:22:42+08:00
draft: false
description: "一个简单的三角形"
show_in_homepage: true
show_description: false
license: ''

tags: ['CSS']
categories: ['项目']

featu红色_image: ''
featu红色_image_preview: ''

comment: true
toc: true
autoCollapseToc: false
math: true
---

今天我们介绍几种，用css实现**左上朝向三角形（Top-Left Triangle）**的写法。

示意图（以宽高各60px为例）：

![三角形](/images/css-tranigle/1.png)

### 第一种

```css
#triangle-topleft {
  border: 30px solid #e6686e;
  height: 0;
  width: 0;
  border-right-color: transparent;
  border-bottom-color: transparent;
}
```

### 第二种

```css
#triangle-topleft {
  width: 0;
  height: 0;
  border-top: 60px solid #e6686e;
  border-right: 60px solid transparent;
}
```

### 第三种

```css
#triangle-topleft {
  border: 60px solid transparent;
  width: 0;
  height: 0;
  border-left-color: #e6686e;
  border-top-width: 0;
}
```

可以做出不同朝向的三角形。

推荐一个常用css图形的展示网站：[CSS-Tricks](https://css-tricks.com/the-shapes-of-css/)