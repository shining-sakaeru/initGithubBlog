---
layout: post
current: post
cover: assets/built/images/jekyll-logo.png
navigation: True
title: Jekyll 따라하기(8) - Travis CI
date: 2021-01-08 19:39:00
tags: [jekyll]
class: post-template
subclass: "post tag-python"
author: noah
---

{% include jekyll-table-of-contents.html %}

github blog 사용을 위한 Jykell Setup 과정입니다.

- Reference: https://moon9342.github.io/jekyll-travis-ci-public

---

1. Source Folder 및 Target Folder 준비

   > Source Folder: Before Compile
   > Target Folder: After Compile

2. Github push

   > 위 2개 Folder에 대한 github repository 생성

3. \_config.yml 설정

   > destination 값을 ./output 을 변경

4. Git Submodule 생성

   > git submodule add https://github.com/github-username/repository.github.io.git output
   > git submodule update

5. Travis계정 생성

   > public으로 생성함.

6. .travis.yml 및 Rakefile 설정

   > 두개 File 생성 및 설정

7. Github Token 생성

   > Setting > Developer settings > Personal access tokens - Generate New Token

8. Token Encrypt. 암호화.

   > gem install travis

   > travis login --pro

   > `travis encrypt GITHUB_TOKEN=<생성한 github token> -r <github username>/<repository>`

   > 생성된 secure code를 .travis.yml 안에 위치한 secure 에 반영함

9. Run Travis CI

   > Source folder에서 git push를 진행

   > Travis CI homepage에서 진행상황 check

   > 자동 build 및 Target folder로 push

   > github.io 홈페이지 업데이트 완료

---

## 2022-01-08

- 현재 travis-ci.org는 사용되지 않으며  
  travis-ci.com 를 사용하는 것을 확인.

- cli에서 travis login시 fail. 아래처럼 사용하면 정상 동작함

  > `travis login --com --github-token <생성한 github token>`

- Source folder에서 push시 fail 발생
  ![Travis error](./assets/built/images/travis error.png "Travis error")
  파악해보니 Travis CI가 유료화 된 것으로 보임  
   Trial Plan 사용시 정상 동작하는 것 확인함.  
   신용카드 번호 등록해야 하며, VAT ID가 나오는데 필자는 아무렇게나 적어도 문제 없었음.  
   아래 이미지들 참고.  
  ![Travis select plan](./assets/built/images/travis select plan.png)
  ![Travis trial plan](./assets/built/images/travis trial plan.png)
  ![Travis credit usage](./assets/built/images/travis credit usage.png)
  ![Travis build start](./assets/built/images/travis build start.png)
  ![Travis build completed](./assets/built/images/travis build completed.png)
