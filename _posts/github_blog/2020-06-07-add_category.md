---
title: "블로그에 Category 추가하기"
categories:
    - Blog
tags:
    - Blog
---

# 카테고리 파일 생성
_pages 폴더에 적당한 이름으로 md 파일을 생성한다. _pages 폴더에는 다양항 유형의 파일들이 포함되어 있으므로, 구분하기 위해 앞에는 category 라고, 명시하고, 뒷부분에는 해당 카테고리 이름을 적어주는게 좋다.

예) _pages/category_blog.md

```yml
---
title: "블로그 설정"
permalink: /categories/blog/
layout: category
author_profile: true
taxonomy: blog
---
```
- title : 적당히 이름 적는다.
- permalink : 해당 카테고리로 이동하게 될 링크 주소를 적는다. 안적으면 전체 경로/파일명으로 접근해야 한다.
- layout : 유형이 카테고리니까 category
- author_profile : 작성자 정보를 보여줄건지 설정
- taxonomy : 글을 쓸때 카테고리에 입력하면 이 카테고리에 속하게 된다.

# 메뉴바에 카테고리 등록할 경우
상단 메뉴바에 카테고리를 등록하려면 _data/navigation.yml 파일을 수정한다. 

```yml
main:
  - title: "Blog"
    url: /categories/blog/
```
main 항목 안쪽에 추가한다.
- title : 메뉴바에 표시될 이름
- url : 위에서 만든 카테고리의 permalink 를 입력

# 사이드바에 카테고리 등록할 경우