---
layout: page
title: 모임 시간
description: 정기 모임 시간.
nav_order: 3
---

# 모임 시간

아래는 예시 모임 시간입니다. `_schedules/weekly.md`를 편집해 실제 요일/시간/장소로 수정하세요.

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
