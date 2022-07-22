---
title: Redirect to URL
tags: browser
expertise: beginner
 : blog_images/coffee-phone-tray-2.jpg
 : 2017-12-17T17:55:51+02:00
 : 2020-10-20T11:46:23+03:00
---

Redirects to a specified URL.

- Use `Window.location.href` or `Window.location.replace()` to redirect to `url`.
- Pass a second argument to simulate a link click (`true` - default) or an HTTP redirect (`false`).

```js
const redirect = (url, asLink = true) =>
  asLink ? (window.location.href = url) : window.location.replace(url);
```

```js
redirect('https://google.com');
```
