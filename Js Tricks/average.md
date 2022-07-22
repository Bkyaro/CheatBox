---
title: Average of numbers
tags: math,array
expertise: beginner
 : blog_images/interior-8.jpg
 : 2017-12-29T13:29:49+02:00
 : 2020-10-22T20:23:47+03:00
---

Calculates the average of two or more numbers.

计算两个或以上数字的平均值

- Use `Array.prototype.reduce()` to add each value to an accumulator, initialized with a value of `0`.
- Divide the resulting array by its length.

- 使用 `Array.prototype.reduce()` 把每个值加到累加器，用0来初始化
- 用所得数字与参数的长度相除

```js
const average = (...nums) =>
  nums.reduce((acc, val) => acc + val, 0) / nums.length;
```

```js
average(...[1, 2, 3]); // 2
average(1, 2, 3); // 2
```
