# X(Twitter) API 설정

## 인증 정보 (환경 변수로 저장됨)
- **API Key:** DXDRUcGHA3agwLSCsA2HL7yQh
- **API Key Secret:** wPcgx2jOEHlXDwcTBa2fla5Ng5Eo89KUqh1F0LN2Ea0MfesIIQ
- **Access Token:** 2024381209707786240-v34Whgjdoat9UAR8LZWSYBCn1MoAbv
- **Access Token Secret:** 15qxmZoa3IdvT8FYY3oWFFf0lfG9GcY5dSdXaOdgkH48C

## 저장 위치
`~/.openclaw/openclaw.json`의 `env` 섹션

## 사용 방법
관찰 일지 작성 후, `exec` 도구를 사용하여 Twitter API v2 엔드포인트로 직접 트윗을 게시할 수 있음:

```bash
curl -X POST https://api.twitter.com/2/tweets \
  -H "Authorization: Bearer $TWITTER_ACCESS_TOKEN" \
  -H "Content-Type: application/json" \
  -d '{"text": "트윗 내용"}'
```

또는 Twitter API v1.1 사용:
```bash
curl -X POST https://api.twitter.com/1.1/statuses/update.json \
  --oauth1 "..." \
  -d "status=트윗 내용"
```
