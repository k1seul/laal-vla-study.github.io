---
layout: page
title: 멤버
description: 스터디 멤버 목록.
nav_order: 5
---

# 멤버

멤버 정보는 `_staffers` 디렉토리에 마크다운 파일로 저장됩니다. 새 멤버가 합류하면 파일을 추가하세요.

{% for staffer in site.staffers %}
{{ staffer }}
{% endfor %}
