---
id: 587d7db4367417b2b2512b93
title: 全局匹配
challengeType: 1
forumTopicId: 301342
---

# --description--

到目前为止，只能提取或搜寻一次模式匹配。

```js
let testStr = "Repeat, Repeat, Repeat";
let ourRegex = /Repeat/;
testStr.match(ourRegex);
// Returns ["Repeat"]
```

若要多次搜寻或提取模式匹配，可以使用`g`标志。

```js
let repeatRegex = /Repeat/g;
testStr.match(repeatRegex);
// Returns ["Repeat", "Repeat", "Repeat"]
```

# --instructions--

使用正则表达式`starRegex`，从字符串`twinkleStar`中匹配到所有的`"Twinkle"`单词并提取出来。

**注意：**  
在正则表达式上可以有多个标志，比如`/search/gi`。

# --hints--

你的正则表达式`starRegex`应该使用全局标志`g`。

```js
assert(starRegex.flags.match(/g/).length == 1);
```

你的正则表达式`starRegex`应该使用忽略大小写标志`i`。

```js
assert(starRegex.flags.match(/i/).length == 1);
```

你的匹配应该匹配单词`'Twinkle'`的两个匹配项。

```js
assert(
  result.sort().join() ==
    twinkleStar
      .match(/twinkle/gi)
      .sort()
      .join()
);
```

你的匹配`结果`应该包含两个元素。

```js
assert(result.length == 2);
```

# --solutions--

