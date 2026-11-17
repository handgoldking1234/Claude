---
name: koreatalk
description: KoreaTalk — 한국인↔외국인 1:1 영상통화 언어교환 앱(Flutter+Supabase, AI 코치). 개발 원칙과 Phase 상태
aliases: [코리아톡, KoreaTalk, 언어교환 앱, ktalk]
---
- 한국을 좋아하는 외국인과 한국인을 영상통화로 연결해 서로 언어를 배우고, AI가 실시간 코치·실력 분석·레벨 자동 조절
- 핵심 철학: 주인공은 사람, AI는 옆에서 돕는 코치 — "AI와만 대화하는 앱"이 아님
- 스택: Flutter(Android/iOS), Supabase(Auth·Postgres·Realtime·Storage·Edge Functions·pgvector), WebRTC(signaling은 Supabase Realtime), AI/STT/TTS는 provider-independent
- 절대 규칙: AI API Key를 앱에 넣지 않음(앱→자체 서버→Provider), Mock을 실제 기능처럼 만들지 않음(MockXxx/RealXxx 분리), WebRTC를 UI만 만들고 완료라고 하지 않음
- 레벨 1~10: 최근 3~5회 평균 85↑ 상승 / 55~84 유지 / 55↓ 지속 시 하락; 통화 기본 20분(전반 영어·후반 한국어); 매칭 점수 언어40/레벨20/관심사20/스타일10/가용성10
- Phase 단위(1 구조 → 2 Auth → 3 Profile → 4 Matching → 5 WebRTC → 6 STT → 7 AI Coach → 8 Analysis → 9 Level → 10 Book/RAG → 11 Safety → 12 Production)로만 개발, 한 번에 전체 구현 금지, 매 작업 후 flutter analyze/test
- 2026-09 v3 대신 가이드 기준 신규 스켈레톤으로 진행, Phase 1~12 코드 zip 전달받음 — analyze/test·실기기 통화 검증 미실시, Google/Apple 로그인·계정 삭제·성장 그래프 미구현
- 2026-11-01: GitHub handgoldking1234/ktalk main에 Phase 1~12 코드 + docs/KoreaTalk_개발가이드.md 푸시 (본인이 이어서 작업한 압축본은 미반영). Vercel ktalk-eta.vercel.app — 루트에 화면 시안 index.html(순수 마크업) 추가
- 본인이 더 진행한 버전은 다른 PC에 있을 가능성 — 찾으면 zip 또는 별도 브랜치(v3 등)로 올려 비교·병합, main은 -f로 덮어쓰지 않기
