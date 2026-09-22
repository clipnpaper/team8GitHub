# 🎡 재밌는 사이트 모음

깃 · 깃허브 특강 팀 프로젝트용 예제 저장소입니다.

![GitHub last commit](https://img.shields.io/github/last-commit/clipnpaper/team8GitHub?color=2ea44f)
![GitHub contributors](https://img.shields.io/github/contributors/clipnpaper/team8GitHub)
![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/clipnpaper/team8GitHub?color=blue)
![GitHub repo size](https://img.shields.io/github/repo-size/clipnpaper/team8GitHub)

> 팀원 각자가 추천하는 사이트를 카드로 등록하고, PR로 합치면서 Git 협업을 연습하는 프로젝트입니다.

---

## 📌 이 저장소는 무엇인가요

우리 8팀이 각자 추천하는 사이트를 모아두는 링크 모음 사이트입니다.

- **홈**(`index.html`) — 추천 사이트가 카드로 나열됩니다
- **상세 페이지**(`sites/*.html`) — 그 사이트가 어떤 곳인지 소개하고, 원래 사이트로 가는 링크를 둡니다

## 📁 파일 구조

```
.
├── index.html                        홈 — 카드 목록 (팀원 모두가 고칩니다)
├── style.css                         공통 스타일 (아무도 고치지 않습니다)
└── sites/
    ├── neal-fun.html                 상세 페이지 예시 — 새 사이트를 추가할 때 이 파일을 복사해서 쓰세요
    ├── animej_js.html                김현준 추천 — anime.js
    ├── DG_recommand.html             노동균 추천 — Raphael Segerman
    ├── film-grab_recommand.html      세람 추천 — Film-Grab
    └── jacksonpollock_recommand.html 세람 추천 — JacksonPollock.org
```

## ✏️ 내 사이트를 추가하는 방법

1. `main` 브랜치로 이동한 뒤 `user/<내이름>` 브랜치를 만듭니다 (예: `user/seram`)
2. `sites/neal-fun.html` 을 복사해 `sites/<사이트이름>.html` 로 저장하고 내용을 채웁니다
3. `index.html` 의 카드 블록(`▼▼▼ 카드 하나 시작` ~ `▲▲▲ 카드 하나 끝`)을 복사해
   목록 아래에 붙이고, 링크·제목·소개·이모지·색을 내 것으로 바꿉니다
4. 커밋하고 푸시한 뒤 풀 리퀘스트를 보냅니다 (`main`은 보호 브랜치라 PR로만 반영됩니다)

## 🧠 이 프로젝트로 배운 GitHub 사용법

실제로 커밋 히스토리를 따라가 보면 팀 협업에서 자주 쓰는 Git/GitHub 흐름을 그대로 연습했다는 걸 알 수 있어요.

- **브랜치 분리** — 팀원마다 `user/<이름>` 브랜치를 따로 만들어 서로의 작업을 건드리지 않고 진행했습니다
- **Pull Request 기반 병합** — 직접 main에 반영하지 않고, PR을 열어 리뷰 후 병합하는 흐름을 12번 넘게 반복했습니다
- **보호 브랜치(Protected Branch)** — main은 직접 push가 막혀 있어서(`GH006: Protected branch update failed`), 모든 변경은 반드시 PR을 거쳐야 합니다
- **머지 충돌 해결** — 여러 명이 `index.html`의 같은 카드 목록 위치를 동시에 고치다 보니 충돌이 자주 났고, 이를 직접 풀어보는 경험을 쌓았습니다
- **되돌리기(Revert)** — 한 번 병합한 변경도 문제가 있으면 `Revert` 커밋으로 안전하게 되돌릴 수 있다는 걸 실제로 확인했습니다 (`Revert "index.html 디자인 리뉴얼..."`)
- **커밋 그래프 읽기** — `Merge pull request #n`, `Merge branch 'main' into user/xxx` 같은 메시지로 브랜치가 어떻게 갈라지고 합쳐졌는지 그래프에서 추적했습니다

## 👥 참여자

| 이름 | 담당 |
|---|---|
| 박세람 | Film-Grab, JacksonPollock.org 카드 |
| 김현준 | anime.js 카드, 디자인 리뉴얼 |
| 노동균 | Raphael Segerman 카드 |
| 정현 | 이슈 템플릿, 초기 세팅 |

## ⚠️ 주의

- `index.html` 은 팀원 모두가 같은 자리를 고칩니다. **충돌이 나는 것이 정상입니다.**
- HTML 을 실제로 구현하는 과제가 아닙니다. 파일을 만들고 링크를 연결하는 것까지가 범위입니다.
