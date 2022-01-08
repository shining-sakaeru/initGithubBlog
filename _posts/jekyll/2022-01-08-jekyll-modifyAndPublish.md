---
layout: post
current: post
cover: assets/built/images/jekyll-logo.png
navigation: True
title: Jekyll 따라하기(2) - Jekyll Modify and Publish
date: 2021-01-08 18:14:00
tags: [jekyll]
class: post-template
subclass: "post tag-python"
author: noah
---

{% include jekyll-table-of-contents.html %}

github blog 사용을 위한 Jykell Setup 과정입니다.

- Reference: https://moon9342.github.io/jekyll-struct

---

1. Jasper2 테마 install

   > http://jekyllthemes.org/themes/jasper2/
   > Download & Move to folder you want

2. Modify _config.yml_

   > Jasper2 테마 main 설정 파일 수정

3. Modify authors.yml

   > 저자 정보 수정

4. Modify tags.yml

   > tag 설정

5. Modify \_include/navigation.html

   > Page navigation 설정

6. \_posts

   > 2022-01-08-file-name.md

7. archive.md / author_archive.md

   > Posting 시간순 정렬

8. Content list

   > <tagName>-table-of-contents.html 생성 및 css 설정

9. Gulp 설치 및 gulpfile.js 설정

   > CSS 연동

10. Github Push

> git push origin master
> push 하면 10-20분 뒤 홈페이지에서 확인 가능

---

gulp 설치 시 알수 없는 에러들이 많았는데,  
googling으로 해결이 불가능 했습니다.  
해결책으로 관련 package 싹 밀고 재설치 하니 잘 동작했습니다.
