# nekarose.github.io

개발자 웹사이트 루트.

`app-ads.txt` 는 광고 인벤토리 사칭을 막는 IAB 표준 선언 파일이다. AdMob 크롤러가
스토어 등록정보에서 개발자 웹사이트의 **도메인만** 가져다
`https://nekarose.github.io/app-ads.txt` 를 읽기 때문에, 하위 경로가 아니라 이
저장소(사용자 사이트)의 루트에 있어야 한다.

원본은 앱 저장소의 `store/app-ads.txt` 에 함께 관리된다.

## 앱별 페이지

- `jigeum-caffeine/version.json` — 지금, 카페인 업데이트 안내용 최신 버전.
  앱이 실행 시 이 파일을 읽어 설치 버전과 비교한다. 원래 Supabase 테이블
  (`app_version_config`)에 있었는데, 읽기 전용 정적 데이터에 DB와 service_role 키가
  필요한 게 과해서 옮겼다. 스토어에 실제로 풀린 뒤에 올릴 것.
- `jigeum-caffeine/support.html` — 지금, 카페인 지원 페이지.
  App Store Connect의 '지원 URL'과 Play 등록정보가 여기를 가리킨다. 개인정보처리방침은
  지원 정보가 아니므로 이 둘을 같은 주소로 두면 안 된다(가이드라인 1.5).
- `jigeum-caffeine/privacy.html` — 지금, 카페인 개인정보처리방침.
  원본은 `nekarose/jigeum-caffeine-ops` 의 `docs/privacy_policy.md` 이고, 이 HTML은
  거기서 변환해 둔 사본이다. 방침을 고칠 때는 원본을 먼저 고치고 이쪽에 반영할 것.

다른 앱(Dumbo Drop, Dumbo Jump)은 각자 별도 저장소의 Pages 를 쓴다.
지금, 카페인은 페이지가 하나뿐이라 여기에 함께 둔다.
