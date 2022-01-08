---
layout: post
current: post
cover: assets/built/images/jekyll-logo.png
navigation: True
title: Jekyll 따라하기(6) - Google Search Console
date: 2021-01-08 18:49:00
tags: [jekyll]
class: post-template
subclass: "post tag-python"
author: noah
---

{% include jekyll-table-of-contents.html %}

github blog 사용을 위한 Jykell Setup 과정입니다.

- Reference: https://moon9342.github.io/jekyll-sitemap

---

1. robots.txt 생성

   > https://support.google.com/webmasters/answer/6062596?hl=ko&ref_topic=6061961

2. sitemap.xml 설정

   > ./sitemap.xml 생성 및 설정

3. Google Search Console 계정 생성

   > https://developers.google.com/search#?modal_active=none
   > Github page url 연결

4. Sitemaps 설정
   > 크롤링 - Sitemaps에 sitemap.xml 추가

---

제출된 사이트맵 - 상태: 가져올 수 없음 error 발생.  
문제점 파악 중.  
![Sitemap import error](./assets/built/images/sitemap failed to get.png)
