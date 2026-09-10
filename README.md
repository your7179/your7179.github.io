# your7179.github.io — 전체 재업로드용 패키지

이 압축 파일은 **저장소 루트(맨 위) 구조 그대로** 정리되어 있습니다.
GitHub에서 기존 파일을 모두 지우신 뒤, 이 안의 내용을 통째로 올리시면 됩니다.

## 이 압축 파일에 들어있는 것

```
(저장소 루트)
├─ _config.yml              ← Jekyll 설정 (루트에 정확히 위치)
├─ _layouts/
│   ├─ default.html
│   └─ post.html
├─ _posts/
│   ├─ 2026-09-10-hwacheon-gaeul.md
│   └─ 2026-09-09-geulsseugi.md
└─ book/
    ├─ index.html            ← '신광태 작가의 서재' 메인 페이지 (Home 메뉴가 여는 화면)
    └─ ssul/
        └─ index.html        ← 작가SSUL 목록 페이지 (자동 카드)
```

## ⚠️ 반드시 다시 넣으셔야 하는, 기존 파일

아래 파일들은 원래 저장소에 있던 것인데, 제가 내용을 갖고 있지 않아 이 압축 파일에는
**포함되어 있지 않습니다.** 기존 파일을 모두 지우고 다시 올리실 계획이라면, 지우기 전에
아래 파일들을 먼저 컴퓨터에 내려받아 두셨다가, 이 압축 파일 내용과 함께 올려주세요.

- `book/iknow.html`
- `book/kboard.html`
- `book/mybrand.html`
- `book/myhomepage.html`
- `index.html` (저장소 맨 위, book 폴더 밖에 있던 것)
- `google5d6ca01af913ce74.html` (구글 서치콘솔 인증 파일)
- `naver65b079611a60625006dfba8ebd3a0356.html` (네이버 서치어드바이저 인증 파일)
- `robots.txt`
- `sitemap.xml`

이 파일들은 검색엔진 인증이나 다른 책 소개 페이지처럼, 이번 작업과 무관하게 계속 필요한
파일들이라 실수로 빠뜨리면 검색 노출이나 다른 페이지 링크가 깨질 수 있습니다.

## 올리는 순서 (추천)

1. 위에 나열된 '기존 파일'들을 먼저 GitHub에서 내려받아 컴퓨터에 백업해 두세요.
2. GitHub 저장소의 기존 파일을 모두 지웁니다.
3. 이 압축 파일의 내용(`_config.yml`, `_layouts`, `_posts`, `book/`)을 저장소 루트에 그대로 올립니다.
4. 1번에서 백업해 둔 기존 파일들을 원래 있던 위치(`book/` 폴더 안 또는 루트)에 맞춰 함께 올립니다.
5. 잠시 후 `https://your7179.github.io/book/`(Home)과 `https://your7179.github.io/book/ssul/`(작가SSUL)이
   정상적으로 열리는지 확인합니다.

## 이후 새 글 추가 방법

`_posts` 폴더에 `연도-월-일-이름.md` 형식으로 파일을 새로 만들고, 맨 위에

```markdown
---
layout: post
title: "글 제목"
description: "카드에 보일 한두 줄 요약"
---
```

을 넣은 뒤 본문을 적으면, `book/ssul/index.html`을 손대지 않아도 자동으로 카드가 생깁니다.
