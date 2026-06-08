# snowmaltea.github.io

HONGJIN LEE가 만든 앱들의 고객 지원 · 개인정보처리방침 호스팅 (GitHub Pages).

## 구조

```
/                       # 앱 허브 (index.html) — 앱 목록 카드
├── <app-slug>/
│   ├── index.html      # 고객 지원 (FAQ + 이메일 문의)
│   └── privacy.html    # 개인정보처리방침
```

## 새 앱 추가 방법

1. `<app-slug>/` 폴더를 만들고 `index.html`(고객 지원), `privacy.html`(개인정보처리방침)을 추가한다.
   - 기존 `money-routine/` 폴더를 복제해 내용만 바꾸면 스타일이 일관되게 유지된다.
2. 루트 `index.html`의 `.app-card` 블록을 복제해 새 앱 카드를 추가한다.
3. 스토어(Play Console / App Store Connect) 등록정보의 개인정보처리방침 URL을
   `https://snowmaltea.github.io/<app-slug>/privacy.html` 로 설정한다.

## 현재 앱

| 앱 | 고객 지원 | 개인정보처리방침 |
|----|----------|------------------|
| 머니루틴 | `/money-routine/` | `/money-routine/privacy.html` |
