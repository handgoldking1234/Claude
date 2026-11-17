---
name: issuemoa
description: 이슈모아 — 한국 커뮤니티 애그리게이터(AI 클러스터링·요약)
aliases: [issuemoa, 이슈모아]
---
- 디시·펨코·클리앙 등에서 제목/링크/메타데이터 수집
- pgvector 임베딩으로 같은 주제 묶고 Claude Haiku로 요약
- 스택: Expo Router + Supabase + pgvector + OpenAI text-embedding-3-small + Claude Haiku
- 전체 Expo 프로젝트 + 6단계 Claude Code 파이프라인 프롬프트 제작(2026-07 초)
- 로그인 보류; 쓰기 기능만 Supabase Auth 카카오 OAuth 예정
