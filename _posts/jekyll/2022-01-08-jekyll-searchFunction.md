---
layout: post
current: post
cover: assets/built/images/jekyll-logo.png
navigation: True
title: Jekyll 따라하기(5) - Search function with lunr.js
date: 2021-01-08 18:39:00
tags: [jekyll]
class: post-template
subclass: "post tag-python"
author: noah
---

{% include jekyll-table-of-contents.html %}

github blog 사용을 위한 Jykell Setup 과정입니다.

- Reference: https://moon9342.github.io/jekyll-search

---

1. search link 생성

   > \_includes/site-nav.html 에서 subscribe를 search로 변경

2. Search Page 설정

   > \_layouts/default.html 수정
   > \_includes/subscribe-form.html 수정
   > search.html 생성 및 수정

3. lunr.js 다운로드 및 설정

   > assets/js/lunr.js

---

lunr.js 추천코드 사용시 동작하지 않음.  
https://lunrjs.com/ 에서 다운로드 받아도 동작하지 않음.  
문제점 확인 중...
