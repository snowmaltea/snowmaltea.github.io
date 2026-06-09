# snowmaltea.github.io

HONGJIN LEE가 만든 앱들의 안내·고객 지원·개인정보처리방침 호스팅 (GitHub Pages).

## 구조

```
/                       # 앱 허브 (index.html) — 앱 카드 목록, 각 카드는 앱 상세로 링크
├── <app-slug>/
│   ├── index.html      # 앱 상세 — 소개·스토어 다운로드·주요 기능·FAQ·문의
│   ├── privacy.html    # 개인정보처리방침
│   └── icon.png        # 앱 아이콘 (허브 카드 + 상세 히어로에서 사용)
```

- **루트 `/`** = 여러 앱을 나열하는 허브. 앱이 늘면 카드를 추가한다.
- **`/<app-slug>/`** = 해당 앱의 단독 페이지. 스토어 지원 URL로도 이 주소를 쓴다(FAQ 포함).

## 새 앱 추가 방법

1. `<app-slug>/` 폴더를 만들고 `index.html`(앱 상세), `privacy.html`(개인정보), `icon.png`를 추가한다.
   - 기존 `money-routine/` 폴더를 복제해 내용·아이콘·스토어 링크만 바꾸면 스타일이 유지된다.
2. 루트 `index.html`의 `.app-card` 블록을 복제해 새 앱 카드를 추가한다(`href="<app-slug>/"`).
3. 스토어 등록정보 URL 설정:
   - 개인정보처리방침: `https://snowmaltea.github.io/<app-slug>/privacy.html`
   - 지원(Support): `https://snowmaltea.github.io/<app-slug>/`

## 현재 앱

| 앱 | 상세·지원 | 개인정보처리방침 |
|----|----------|------------------|
| 머니루틴 | `/money-routine/` | `/money-routine/privacy.html` |
