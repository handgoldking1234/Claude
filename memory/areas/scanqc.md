---
name: scanqc
description: ScanQC — 스캔 이미지 검수·보정 프로그램(HP Review v4.1 대체), 원본/보정본 폴더 비교 (설치형 + 웹 iux-qc)
aliases: [ScanQC, 스캔 검수 프로그램, HP Review, 검수 프로그램, 스캔 검수 도구, scan-review-tool]
---
- 원본 폴더 vs 보정본(HP) 폴더 스캔 이미지를 한 장씩 비교·검수, 크롭·회전·크기·색보정 — 기록물 DB구축 현장 HP Review v4.1(Streamlit, 포터블 Python) 대체
- 용량이 커서 한 번에 다 불러오지 않고 다음 버튼으로 한 장씩
- 디자인시스템 스포티파이, 아이콘 Lucide
- 오프라인 동작 필수
- 흐름: 불러오면 자동 보정 → 작업자는 검수만, 제대로 안 된 장만 수정
- '원본 수정' 시 원본 폴더 파일도 실제 저장 — 원본 백업은 일단 불필요
- 현장 폴더 보통 5,000~10,000장, 주로 설치형 사용, TIF에서 속도 문제(JPG는 OK), PC 메모리가 작을 수 있음
- 웹버전: 로그인 없이 범용(내 PC 폴더), 로그인 시 팀 작업 등 추가, 관리자 페이지에서 비로그인 사용 통계(어떤 파일로 몇 개 변경) — Supabase + Vercel, GitHub handgoldking1234/iux-qc
- 웹버전 고치면 iux-qc 저장소에 자동으로 올리기
