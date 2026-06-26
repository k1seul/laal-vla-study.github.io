---
layout: page
title: 공지사항
nav_exclude: true
description: 스터디 공지 모음.
---

# 공지사항

공지는 `_announcements` 디렉토리에 저장되고 `_layouts/announcement.html`로 렌더링됩니다.

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
