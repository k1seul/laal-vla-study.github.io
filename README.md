# LAAL VLA Study

Vision-Language-Action(VLA) 논문 스터디 계획과 발표 정리를 위한 GitHub Pages 사이트입니다.

🔗 https://k1seul.github.io/laal-vla-study.github.io/

[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) 템플릿을 사용했고, 의존성 관리는 [uv](https://docs.astral.sh/uv/)로 합니다.

## 로컬에서 실행하기

```bash
# 의존성 설치 (uv가 .venv를 자동으로 만들어줍니다)
uv sync

# 로컬 서버 실행 (http://127.0.0.1:8000)
uv run mkdocs serve
```

## 콘텐츠 추가하기

- **스터디 계획 수정**: [docs/schedule.md](docs/schedule.md)
- **새 논문 리뷰 추가**: [docs/papers/_template.md](docs/papers/_template.md)를 복사해 `docs/papers/`에 새 파일을 만들고, [mkdocs.yml](mkdocs.yml)의 `nav` 항목과 [docs/papers/index.md](docs/papers/index.md) 목록에 추가
- **참고 자료 추가**: [docs/resources.md](docs/resources.md)

## 배포

`main` 브랜치에 push하면 [GitHub Actions](.github/workflows/deploy.yml)가 자동으로 빌드 후 GitHub Pages에 배포합니다.
(최초 1회, 저장소 Settings → Pages → Build and deployment → Source를 **GitHub Actions**로 설정해야 합니다.)

수동 배포가 필요하면:

```bash
uv run mkdocs build
```
