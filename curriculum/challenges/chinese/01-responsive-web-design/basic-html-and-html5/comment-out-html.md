---
id: bad87fee1348bd9aedf08804
title: 给 HTML 添加注释
challengeType: 0
videoUrl: 'https://scrimba.com/p/pVMPUv/cGyGbca'
forumTopicId: 16782
---

# --description--

记住：注释的开始标记是`<!--`，结束标记是`-->`。

现在你需要在`h2`元素前终止注释。

# --instructions--

任务：注释掉`h1`元素和`p`元素，保留`h2`元素。

# --hints--

注释掉`h1`元素，这样它就从网页上消失了。

```js
assert($('h1').length === 0);
```

`h2`元素保持原样，这样网页上还能看到它。

```js
assert($('h2').length > 0);
```

注释掉`p`元素，这样它就从网页上消失了。

```js
assert($('p').length === 0);
```

确保每一个注释都以`-->`结尾。

```js
assert(code.match(/[^fc]-->/g).length > 1);
```

不要更改`h1`元素、`h2` 元素、`p`元素的顺序。

```js
assert(
  code.match(/<([a-z0-9]){1,2}>/g)[0] === '<h1>' &&
    code.match(/<([a-z0-9]){1,2}>/g)[1] === '<h2>' &&
    code.match(/<([a-z0-9]){1,2}>/g)[2] === '<p>'
);
```

# --solutions--

