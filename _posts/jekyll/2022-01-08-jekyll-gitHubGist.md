---
layout: post
current: post
cover: assets/built/images/jekyll-logo.png
navigation: True
title: Jekyll 따라하기(7) - GitHub Gist
date: 2021-01-08 19:22:00
tags: [jekyll]
class: post-template
subclass: "post tag-python"
author: noah
---

{% include jekyll-table-of-contents.html %}

github blog 사용을 위한 Jykell Setup 과정입니다.

- Reference: https://moon9342.github.io/jekyll-gist

---

1. Install jekyll-gist

   > gem install jekyll-gist

2. \_config.yml 설정

   > plugins에 jekyll-gist 추가

3. gist 적용

   > gist link copy  
   > 형식은 다음과 같음

   ```
   <script src="https://gist.github.com/userID/url.js"></script>
   ```

   > 아래 처럼 사용.

   ```
   {% gist userID/url %}
   ```

---

특이사항 없이 잘 동작합니다.
