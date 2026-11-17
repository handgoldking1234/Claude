---
name: webtooncut
description: 웹툰보드(이전 웹툰컷·웹툰 컷 편집실) — 웹툰 컷 편집기, 출시·상용화 (iux-webtoon, toon.iux.kr)
aliases: [웹툰보드, 웹툰컷, 웹툰 컷 편집실, 웹툰 컷]
---
- 이름: 웹툰 컷 편집실 → 웹툰컷 → 웹툰보드
- 상용화 검토(게스트 사용·회원가입·AI 비용·수익성) — 우선 무료 오픈, 반응 보고 결제 연결
- 무료 오픈 시 AI 이미지 맛보기 10장(가입 시 지급)
- 웹툰보드 v2·어드민을 GitHub handgoldking1234/iux-webtoon에 보관
- 실서비스: Next.js + Supabase + Vercel, iux-webtoon dev 브랜치 — DB(Supabase 구성)는 본인이 직접 정의
- Vercel 프로젝트(iux-webtoon) Production 브랜치 = dev
- iux-webtoon은 Vercel 하루 배포 한도 때문에 작은 수정마다 올리지 않고 묶어서 푸시 (다른 저장소는 작업 끝나면 바로 푸시)
- Supabase 무료 프로젝트 4개 생성·2개 사용 — Pro 전환 고민, iux-cloud에 계속 붙일지 새로 팔지 고민
- 도메인: 우선 iux.kr 서브도메인, 성공하면 iuxtoon.com
- 「연재하기」 → 독자용 연재관(네이버 웹툰 참고) 바로 게시 — toon.iux.kr/read 경로, 나중에 분리 가능하게
- 연재관 디자인: 넷플릭스·카카오웹툰 참고 → 스포티파이식 + 프리텐다드
- AI API 결제, 키 3개(Anthropic·Gemini·OpenAI) Vercel에 등록, 이미지는 나노바나나(Gemini)
- 정책: 편집기는 누구나, AI는 회원만 → 추후 결제자만 / 현재는 테스트로 로그인 없이 AI 열어 둠
- 단계적 오픈: 회원 없이 통계 먼저 + AI API 테스트
- 시놉([[synopsis-tool]])을 기획 부분에 통합
