# GOLDKING 작업 인수인계 — 새 Claude 계정용

이 저장소는 회사 Claude 계정에서 개인 계정으로 옮기면서(2026-11-18) 만든 이전 패키지다.
새 세션에서 작업을 시작하면 먼저 이 파일을 읽고, 해당 프로젝트의 `memory/areas/*.md` 를 읽은 뒤 이어서 작업한다.

## 사용자
- GOLDKING(손금왕) — 20년+ UI/UX 디자이너 겸 1인 개발자. 상세는 `memory/profile.md`, 이력은 `memory/topics/resume.md`
- 한국어로 대화하고 설명도 한글로

## 반드시 지킬 작업 규칙 (memory/preferences.md)
1. 퍼블리싱 요청이면 개발 소스 넣지 말고 순수 마크업 + 간단한 스크립트만
2. 게임은 파일로만 준다(아티팩트·에이전트로 올리지 않음). 민왕게임월드(game.iux.kr)에는 요청할 때만 넣는다
3. GitHub 푸시 → Vercel 자동 배포: 작업 끝나면 바로 푸시. 예외: `iux-webtoon` 은 묶어서 푸시(Vercel 하루 배포 한도)
4. 네아니요는 매번 묻지 말고 main 에 머지해 배포
5. 새 앱·서비스는 경쟁사 분석 → 실현 가능성 → 타깃 → 기간 → 비용 → 이름 순으로 먼저 검토
6. 자주 쓰는 디자인 지정: 아이콘 Lucide, 폰트 Pretendard, 스포티파이 스타일 디자인시스템

## 공통 인프라
- 도메인 `iux.kr`(가비아, 네임서버 Vercel) — 서비스별 서브도메인: art / studio / game / haru / book / toon / neaniyo / ocr / naeilo / handgold …
- 메일: help@ / hello@ (공통), art@ (IUX ART 영업) → ImprovMX 로 handgoldking@gmail.com 전달
- Supabase: 무료 플랜 활성 2개 한도 → 대부분 공유 프로젝트 `iux-cloud`(IUX Cloud, iux-studio) 사용. 하루5분·북이랑은 하루5분 프로젝트 공유
- AI 키(Anthropic·Gemini·OpenAI)는 각 Vercel 프로젝트 환경변수에 있음 (이 저장소에는 없음)

## 폴더 안내
- `memory/` — 이전 계정 Claude 메모리 전체 (profile, preferences, areas=프로젝트별, people, topics)
- `REPOS.md` — GitHub 저장소 ↔ 프로젝트 ↔ 배포 주소 대응표
- `artifacts/` — 이전 계정 아티팩트 소스(HTML) 백업과 목록. 문서형 아티팩트는 목록만 있음
- `NOT-MIGRATED.md` — 자동으로 못 옮긴 것과 직접 할 일
