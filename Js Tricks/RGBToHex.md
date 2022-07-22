---
title: RGB to hex
tags: string,math
expertise: intermediate
 : blog_images/colors-mural.jpg
 : 2017-12-17T17:55:51+02:00
 : 2020-11-03T22:11:18+02:00
---

Converts the values of RGB components to a hexadecimal color code.

- Convert given RGB parameters to hexadecimal string using bitwise left-shift operator (`<<`) and `Number.prototype.toString()`.
- Use `String.prototype.padStart()` to get a 6-digit hexadecimal value.

```js
const RGBToHex = (r, g, b) =>
  ((r << 16) + (g << 8) + b).toString(16).padStart(6, '0');
```

```js
RGBToHex(255, 165, 1); // 'ffa501'
```
