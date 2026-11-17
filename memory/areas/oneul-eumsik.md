---
name: oneul-eumsik
description: 오늘의 음식 — 날씨·계절·상황 반응형 외식 큐레이션 웹서비스, 5일 MVP 완성·배포 대기
aliases: [oneul-eumsik, 오늘의 음식, 오늘 뭐먹지]
---
- 날씨·계절·시간·이슈에 따라 AI가 메뉴 추천
- 유튜브 영상 연동: 집밥(요리영상·레시피+쿠팡) / 외식(식당 소개영상·네이버 위치·평점) — 외식 큐레이션 차별화에 무게
- 매칭 실패 식당은 상세페이지 댓글로 제보 유도(유튜브식 자유 댓글, 별도 제보 UI 없음)
- Next.js + Supabase + Vercel 5일 MVP (앱은 PMF 후 Expo)
- YouTube 수집: 화이트리스트 채널 uploads 플레이리스트(playlistItems.list + videos.list 배치), search.list 대량 발굴 제외
- 댓글 승격은 MVP에서 어드민 수동, 자동 파싱·교차검증은 v2
- 5일: D1 스키마·수집, D2 AI 큐레이션·네이버 플레이스 매칭, D3 화면+SEO, D4 댓글, D5 수익·배포
- UI 당근마켓 스타일(오렌지 #FF6F0F), 모바일1열→태블릿2열→PC3열
- D1~D5 구현, 프로덕션 빌드 통과 — Supabase 스키마 적용·env·배포는 사용자 실행 대기 (YouTube 임베드, 댓글, 어드민 승격, SEO sitemap, 쿠팡 제휴 포함)
