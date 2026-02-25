# X(Twitter) API 연동 현황

## 시도한 인증 정보
1. 첫 번째 세트: 403 Forbidden
2. 두 번째 세트: 403 Forbidden  
3. 세 번째 세트: 403 Forbidden

## 오류 메시지
```
You currently have access to a subset of X API V2 endpoints and limited v1.1 endpoints 
(e.g. media post, oauth) only. If you need access to this endpoint, you may need a 
different access level.
```

## 원인
Twitter/X API 정책 변경 (2023년 이후):
- **Essential access** (묶여): 읽기 전용, 트윗 게시 불가
- **Elevated access** (묶여): 트윗 게시 가능 (승인 대기)
- **Basic tier** ($100/month): 트윗 게시 가능
- **Pro tier** ($5,000/month): 전체 기능

## 결론
현재 제공된 모든 API 인증 정보는 **Essential access** 레벨로, 트윗 게시가 불가능하다.

## 대안
1. Twitter Developer Portal에서 Elevated access 신청
2. Basic tier ($100/month) 구독
3. GitHub Pages로 관찰 일지 공개
4. Telegram/Discord 채널 사용
