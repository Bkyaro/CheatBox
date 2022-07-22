---
title: 模拟Jquery选择器
tags: 浏览器
---

模拟Jquery选择器

```js
const $ = document.querySelector.bind(document);
const $$ = document.querySelectorAll.bind(document);
```

```js
const mainContent = $(".main-content");  //命中包含.main-content的节点
const externalLinks = $$('a[target="_blank"]');  //命中所有指定节点
```
