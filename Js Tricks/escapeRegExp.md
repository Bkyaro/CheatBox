---
title: Escape RegExp
tags: string,regexp
expertise: intermediate
 : blog_images/frog-blue-flower.jpg
 : 2017-12-17T17:55:51+02:00
 : 2020-09-15T16:28:04+03:00
---

Escapes a string to use in a regular expression.

- Use `String.prototype.replace()` to escape special characters.

```js
const escapeRegExp = str => str.replace(/[.*+?^${}()|[\]\\]/g, '\\$&');
```

```js
escapeRegExp('(test)'); // \\(test\\)
```
