---
layout: post
current: post
cover: assets/built/images/jekyll-logo.png
navigation: True
title: Jekyll 따라하기(4) - Highlighting with rouge
date: 2021-01-08 18:34:00
tags: [jekyll]
class: post-template
subclass: "post tag-python"
author: noah
---

{% include jekyll-table-of-contents.html %}

github blog 사용을 위한 Jykell Setup 과정입니다.

- Reference: https://moon9342.github.io/jekyll-rouge

---

1. install rouge

   > gem install rouge

2. 사용 가능한 style 확인

   > rougify help style

3. theme css 생성

   > rougify style monokai.sublime > assets/css/syntax.css

4. \_layouts/default.html 설정

   > make CSS to Post interface

---

특이사항 없이 잘 작동.
