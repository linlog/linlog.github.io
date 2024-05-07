---
title: GITHUB블로그에 jekyll테마(chirpy) 적용하기
author: lin
date: '2023-11-10 11:12:00 +0800'
categories:
  - Blogging
  - Tutorial
tags:
  - favicon
---


github에서 블로그용 repository를 생성하고 난 뒤, 블로그 테마를 적용해보기로 했다.
이번에 github로 블로그를 생성하면서 .. 글을 올려보기는 커녕 테마 적용하는데만 시간이 너무 오래 걸렸다. 
하지만 포기하지 않고 여러 블로그들을 뒤져가며 테마 적용에 성공하였다...!! 

jekyll 테마 사이트들이 몇개있었는데 퀄리티가 다소 떨어지는 게 대다수라서 
조금 완성도 있는 chirpy 테마를 선택하였다. (결론은 만족)

## 미리 설치해야할 것들 
1. ruby(3.0이상)
https://rubyinstaller.org/downloads/
> 버전은 반드시 3.0 이상으로 해야 chirpy 테마에서 사용하는 모듈이 정상적으로 동작한다.
{: .prompt-info }d

2. node.js
https://nodejs.org/en
> node.js 모듈을 설치하지 않으면 assets/js/dist/*.min.js Not Found 에러 발생과 함께 블로그 기능이 정상적으로 동작하지 않는다.
{: .prompt-info }


## chirpy 테마 설치 
chirpy 테마는 두가지 버전이 있는데
커스터마이징이 필요없다면 [**chirpy-starter**](https://github.com/cotes2020/chirpy-starter)을
커스터마이징이 필요하다면 [**chirpy**](https://github.com/cotes2020/jekyll-theme-chirpy)을
다운받으면 된다.

fork해서 계속 테마 업데이트를 받을수도 있지만, 
나는 업데이트 받지 않고 쓸거라서 zip파일로 다운받아서 로컬에 설치하기로 했다.
미리 github를 연결해둔 로컬경로에 zip파일을 풀어준 후
아래 명령어로 github에 소스 업데이트를 해주면된다.

```bash
git add .
git commit -m "zekyll theme apply"
git push origin main
```
