---
title: {{ date }}
lang: ko
date: {{ date }}
updated:
top_img: /img/galaxy-3219390-2.webp
cover: /img/galaxy-3219390-2.webp
sticky: false

categories:
- [private, diary]
- []
sticky_categories: []
tags: []
sticky_tags: []

keywords:
description:
password: {{ title }}

inject_head:
  # 검색 엔진에 추가 안 되게
  - <meta name="robots" content="noindex">
  # 체크박스 추가 (checkbox 태그)
  - <link rel="stylesheet" href="/css/tag_plugins_custom@1.0.17/checkbox@0.0.1.css">

katex: false  # default: true
comments: # default: true
toc:   # default: true
toc_number:   # default: false
toc_style_simple:   # default: true
copyright:   # default: true
copyright_author:
copyright_author_href:
copyright_url:
copyright_info:
aplayer:   # default: false
highlight_shrink:   # default: true
aside:   # default: true
abcjs:   # default: false
---

Not Written Yet

# TO-DO
{% checkbox 일반 텍스트 테스트 %}
{% checkbox checked , 간단한 [markdown](https://guides.github.com/features/mastering-markdown/) 지원 %}
{% checkbox red, 사용자 정의 지원정의 색상 %}
{% checkbox green checked, 초록색 + 기본 선택 %}
{% checkbox yellow checked, 노란색 + 기본 선택 %}
{% checkbox cyan checked, 청록색 + 기본 선택 %}
{% checkbox blue checked, 파란색 + 기본 선택 %}
{% checkbox plus green checked, plus 선택 %}
{% checkbox minus yellow checked, minus 선택 %}
{% checkbox times red checked , times 선택 %}


# asdf