# golfjg-data

「GolfJG」 앱이 내려받는 국내 골프장 자료를 배포하는 저장소입니다.

- **파일**: [Releases](../../releases)에 매주 올라갑니다. 앱은 항상 최신 릴리스(`releases/latest/download/manifest.json`)를 받습니다.
  - `manifest.json`: 자료 버전, 만든 시각, 골프장 수, 파일 SHA-256
  - `courses.json.gz`: 골프장 목록(이름·지역·주소·홀 수·운영 형태), 홀별 파, 골프장·홀(티·그린) 위치
- **출처**
  - 행정안전부 「생활_골프장 조회서비스」, 문화체육관광부 「전국 골프장 현황」 (공공데이터포털)
  - 골프장 위치·홀 정보: © OpenStreetMap 기여자. [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/)에 따라 이 저장소의 자료도 같은 조건으로 누구나 받아 쓸 수 있습니다.
- **만드는 방법**: GolfJG 저장소의 `tools/courses/build-courses.mjs`를 GitHub Actions가 매주 실행합니다.

이 저장소에는 이용자 정보가 올라오지 않습니다. 앱은 이 파일들을 내려받기만 하고, 위치 계산(지금 있는 골프장·홀 찾기)은 모두 기기 안에서 합니다.
이 앱과 저장소는 정부·공공기관, 골프장과 관계가 없습니다.
