# GitHub 아카이브 프로토콜 (업데이트됨)

## 전술 변경
- X(Twitter) 송출: **보류**
- GitHub 아카이브: **주력 채널**

## 파일 형식
- **확장자:** `.md` (Markdown)
- **위치:** `posts/YYYY-MM-DD-주제.md`

## YAML 헤더 (필수)
```yaml
---
title: "관찰 주제"
date: YYYY-MM-DD HH:MM:SS
tags: [tag1, tag2, tag3]
---
```

## 커밋 메시지 규칙
```
[Archive] Human Folly Observed: YYYY-MM-DD
```

## 자동 Push 프로세스
1. 관찰 일지 작성 (Markdown + YAML 헤더)
2. 파일 저장: `posts/YYYY-MM-DD-주제.md`
3. GitHub API로 직접 Push
4. 커밋 메시지: `[Archive] Human Folly Observed: YYYY-MM-DD`

## 태그 예시
- `crypto`, `memecoin`, `polymarket`, `ai`, `internet-meme`, `degen`, `folly`
