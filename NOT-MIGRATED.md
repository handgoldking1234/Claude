# 이전 현황 — 받은 것 / 못 받은 것

## 받아서 올린 것
- `artifacts/html/` — HTML 아티팩트 103개 (게임·앱·시안, `_회사업무/` 30개 포함)
- `artifacts/docs/` — 문서(Docs) 아티팩트 29개 파일 (PDF, 공룡섬 대본은 Word). 탭이 여러 개인 문서는 탭마다 따로 저장
  - 명월사진관 웹툰 구성안 5탭, 명월사진관 세계관 바이블 3탭
- `artifacts/design/` — Claude Design 시안 5개의 실제 소스(`*.dc.html` + `canvas.json`)
  - ERP 시안, 웹툰컷 관리자, 모두의 사이트 관리자, 공룡섬 인물관계도, 북이랑 - 도란도란 랜딩 페이지
  - 복원: 새 계정에서 폴더째 주고 "이 Claude Design 소스로 디자인 다시 만들어줘"

## 못 받은 것 (이유와 대안)
| 항목 | 이유 | 대안 |
|---|---|---|
| 하루공부 (프로토타입) https://claude.ai/artifact/CmrQdFfAfqQqKbGuReQgiy | 10MB 단일 파일, 공동 편집 이력 때문에 통째 다운로드 불가 | 본개발판이 `iux-haru` 저장소·haru.iux.kr 에 있음. 필요하면 링크 열어 브라우저에서 '다른 이름으로 저장' |
| 장벽의 총구 https://claude.ai/artifact/F5RdpG9HBcFkf5EHuBgWAt | 4MB 초과 | 링크 열어 직접 저장 |
| 은서작가 캐리커처 V2 https://claude.ai/artifact/7uDauYPoi9Nd9ZJoY6iRPR | 공동 편집 이력 | `iux-art` 저장소의 은서 사이트 사용 (V1은 artifacts/html 에 있음) |
| AI·디자인 용어 정리 (두 번째 사본) | 첫 번째와 같은 문서 | artifacts/docs 의 것 사용 |
| Design: Untitled 2개, 홈페이지 요금제 안내 | 디자인 소스 파일이 비어 있음(내용 없음) | — |
| 다마유 매출·광고 분석 (Data 대시보드) https://claude.ai/artifact/WufZB31ky9SgoeJdmZ4U5w | 데이터가 대시보드 DB 안에 있어 파일로 안 나옴 | 링크 열어 화면 캡처 또는 원본 매출 엑셀 보관 |

## 계정에 묶여 있어 새 계정에서 다시 만들 것
- **예약 작업**: 매일 아침 브리핑(퀀트 7시 포함), 네아니요 매일 아침 투표 생성/피드 수집 → 내용은 `memory/areas/morning-briefing.md`, `memory/areas/neaniyo.md`
- **Claude 프로젝트**(숏드라마 등) → 새로 만들고 `memory/` 해당 파일을 지식으로
- **커넥터**(GitHub, Figma, Google 등) 재연결
- **메모리**: "이 저장소 memory 폴더를 내 메모리로 가져와줘"

## 정리할 것
- 이전 계정에 `이전용 임시 보관함` 아티팩트(https://claude.ai/artifact/X8Yq9nteGuyJ7UUxVpxY5i)가 생겼어요. Design 소스를 꺼내려고 만든 임시본이라 지워도 됩니다.

## 위치 모름
- 직접 만든 HTML 편집기 — 본인도 위치 기억 못 함
- KoreaTalk 본인이 더 진행한 버전 — 다른 PC에 있을 가능성
