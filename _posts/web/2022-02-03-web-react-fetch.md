---
layout: post
current: post
cover: assets/built/images/nasa-web-unsplash.jpg
navigation: True
title: React - fetch
date: 2021-02-03 23:21:00
tags: [web]
class: post-template
subclass: "post tag-python"
author: noah
---

<!-- {% include jekyll-table-of-contents.html %} -->

API를 느져오는 React 기능. fetch

<!-- - Reference: https://en.wikipedia.org/wiki/Search_engine_optimization -->

---
url에서 fetch를 사용하여 json 정보를 끌어와 보여줌.

```
fetch("url")
  .then((response) => response.json())
  .then((data) => console.log(data));
```

---

화면에 뿌려줄 때, useState와 map 기능을 사용하여 진행하려는데
마음대로 되지 않아 시도중.. 성공 후 업데이트 하려합니다.