# 작가SSUL — 설치 안내

이 폴더를 그대로 `your7179.github.io` 저장소(repo)의 **맨 위(루트)**에 올려 넣으시면 됩니다.
(기존에 있던 `book/index.html` 등 다른 파일은 그대로 두고, 아래 파일들만 "추가"하는 것입니다.)

## 1. 올려야 할 파일 위치

```
your7179.github.io/            ← 저장소 맨 위
├─ _config.yml                 ← (신규) Jekyll 설정
├─ _layouts/
│   ├─ default.html            ← (신규) 공통 틀
│   └─ post.html                ← (신규) 글 한 편 화면
├─ _posts/
│   ├─ 2026-09-10-hwacheon-gaeul.md   ← (신규) 예시 글
│   └─ 2026-09-09-geulsseugi.md       ← (신규) 예시 글
└─ book/
    ├─ index.html               ← 기존 파일 (그대로 둠)
    └─ ssul/
        └─ index.html           ← (신규) 작가SSUL 목록 페이지
```

`_config.yml`이 저장소에 **이미 있다면** 통째로 덮어쓰지 마시고, 그 안의 내용을 열어서
`permalink`, `plugins` 항목만 참고해 추가해 주세요.

## 2. GitHub에서 확인할 것

`your7179.github.io` 저장소의 **Settings → Pages**에서
- Source가 `Deploy from a branch`
- Branch가 `main`(또는 `master`) / `/ (root)`

로 되어 있으면 별도 설정 없이 자동으로 Jekyll이 작동합니다. (GitHub Pages는 `_config.yml`이
있으면 자동으로 Jekyll로 빌드합니다.) 혹시 저장소에 `.nojekyll` 이라는 빈 파일이 있다면,
그 파일만 삭제해 주세요. (Jekyll을 못 쓰게 막는 파일입니다.)

## 3. 새 글은 이렇게 올리면 됩니다

`_posts` 폴더 안에 아래 이름 규칙으로 파일 하나만 새로 만들면, **작가SSUL 페이지에 자동으로 카드가 생깁니다.**
따로 목록 페이지를 손댈 필요가 없습니다.

- 파일명 규칙: `연도-월-일-아무이름.md` (예: `2026-10-01-첫눈.md`)
- 파일 맨 위에 아래 형식을 꼭 넣어주세요.

```markdown
---
layout: post
title: "글 제목"
description: "카드에 보일 한두 줄 요약"
---

여기부터 본문 내용을 자유롭게 적으시면 됩니다.
```

이렇게 저장하면:
- `https://your7179.github.io/book/ssul/` 페이지에 새 카드가 맨 위에 자동으로 나타납니다.
- 카드를 누르면 `title`과 본문이 담긴 글 페이지로 연결됩니다.
- `description`을 안 적으면, 본문 앞부분이 자동으로 요약되어 카드에 보입니다.

## 4. 메인 페이지(아울이르) 쪽

`신광태 작가의 서재` 상단 메뉴의 **'작가SSUL'** 항목은 이미
`https://your7179.github.io/book/ssul/` 로 연결해 두었습니다. 이 폴더만 올리시면 바로 작동합니다.
