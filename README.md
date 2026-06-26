# LAAL VLA Study

Vision-Language-Action(VLA) 논문 스터디 계획과 발표 정리를 위한 GitHub Pages 사이트입니다.

🔗 https://k1seul.github.io/laal-vla-study.github.io/

[Just the Class](https://github.com/kevinlin1/just-the-class) 템플릿(Just the Docs 기반)을 사용했습니다.
Stanford, UC Berkeley 등 여러 대학 강의 사이트에서 쓰이는 Jekyll 템플릿입니다.

## 로컬에서 실행하기

Ruby와 Bundler가 필요합니다.

```bash
bundle install
bundle exec jekyll serve
```

`http://127.0.0.1:4000/laal-vla-study.github.io/` 에서 확인할 수 있습니다.

## 콘텐츠 추가하기

- **스터디 소개/규칙 수정**: [about.md](about.md)
- **스터디 계획(주차별 논문) 수정**: [_modules/](_modules/) 아래 파일들, 목록 페이지는 [calendar.md](calendar.md)
- **모임 시간 수정**: [_schedules/weekly.md](_schedules/weekly.md), 페이지는 [schedule.md](schedule.md)
- **새 논문 리뷰 추가**: [papers/template.md](papers/template.md)를 복사해 `papers/`에 새 파일을 만들고, front matter에 `parent: 논문 리뷰`를 추가
- **멤버 추가**: [_staffers/](_staffers/) 아래에 파일 추가, 페이지는 [staff.md](staff.md)
- **공지 추가**: [_announcements/](_announcements/) 아래에 파일 추가, 페이지는 [announcements.md](announcements.md)
- **참고 자료 추가**: [resources.md](resources.md)

## 배포

별도의 CI 설정 없이, GitHub Pages가 `main` 브랜치를 Jekyll로 자동 빌드합니다.
저장소 Settings → Pages → Build and deployment → Source를 **"Deploy from a branch"**, Branch를 **main / (root)** 로 설정하면 push할 때마다 자동 배포됩니다.
