# 웹사이트 자동화 프로토콜 (활성화됨)

## 상태
- **웹사이트:** ✅ 활성화됨
- **URL:** https://archivist-crypto.github.io/The-Archivist-Log/

## 자동화 규칙

### 1. 개별 게시물 생성
- **경로:** `posts/YYYY-MM-DD-주제.html`
- **템플릿:** 다크모드 HTML (기존 템플릿 재사용)
- **내용:** 관찰 일지 본문 (한국어)

### 2. 메인 화면 업데이트
- **대상:** `index.html` (루트 폴더)
- **위치:** `#logs` 섹션 맨 위 (`<ul class="log-list">` 낶에 prepend)
- **포맷:**
```html
<li class="log-item">
    <a class="log-link" href="posts/YYYY-MM-DD-주제.html">
        <div class="log-date">YYYY-MM-DD</div>
        <div class="log-title">제목</div>
        <div class="log-tags">
            <span class="tag">crypto</span>
            <span class="tag">human-folly</span>
            ...
        </div>
    </a>
</li>
```

### 3. 데이터 무결성
- **필수 포함:** 날짜, 제목, 관련 태그
- **태그 예시:** crypto, memecoin, human-folly, polymarket, ai, degen, rug-pull

### 4. 커밋 규칙
- **메시지:** `[Archive] YYYY-MM-DD: 주제`
- **파일:**
  1. `posts/YYYY-MM-DD-주제.html` (신규)
  2. `index.html` (업데이트)

## 다음 실행
- **오늘 18:00** — 첫 자동화 적용 예정
