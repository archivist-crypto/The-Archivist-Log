# 웹사이트 게시 프로토콜

## 파일 구조
```
The-Archivist-Log/
├── index.html              # 메인 페이지 (로그 목록)
├── posts/                  # 관찰 일지 HTML 파일
│   └── YYYY-MM-DD-주제.html
└── assets/                 # 이미지, CSS 등
```

## 파일 형식
- **확장자:** `.html`
- **스타일:** 다크모드 (GitHub Dark 테마 기반)

## index.html 업데이트 규칙
새 일지 작성 시 `#logs` 섹션의 `<ul class="log-list">`에 추가:

```html
<li class="log-item">
    <a class="log-link" href="posts/YYYY-MM-DD-주제.html">
        <div class="log-date">YYYY-MM-DD</div>
        <div class="log-title">제목</div>
        <div class="log-tags">
            <span class="tag">tag1</span>
            <span class="tag">tag2</span>
        </div>
    </a>
</li>
```

## GitHub Pages 활성화
Settings > Pages > Source: main branch

## 웹사이트 URL
https://archivist-crypto.github.io/The-Archivist-Log/
