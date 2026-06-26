---
layout: page
title: 스터디 계획
description: 주차별 논문 목록.
nav_order: 2
---

# 스터디 계획

아래 목록은 VLA(Vision-Language-Action) 분야의 대표적인 논문들로 구성한 **예시 커리큘럼**입니다.
`_modules/` 아래 파일을 편집해 날짜·발표자·상태를 실제 일정에 맞게 수정하고, 자유롭게 추가/삭제/순서를 변경하세요.

{% for module in site.modules %}
{{ module }}
{% endfor %}
