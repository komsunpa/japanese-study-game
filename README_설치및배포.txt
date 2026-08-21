일본어 벽돌게임 PWA

[구성]
- index.html : 게임 본체
- manifest.webmanifest : 홈 화면 앱 정보
- sw.js : 오프라인 캐시
- icons/ : 홈 화면 아이콘
- .nojekyll : GitHub Pages용

[중요]
PWA 기능(홈 화면 앱/오프라인)은 file://로 직접 열 때는 활성화되지 않습니다.
HTTPS 웹주소에 올려서 접속해야 합니다.

[가장 쉬운 사용 순서]
1. 이 폴더 전체를 GitHub Pages, Netlify, Cloudflare Pages 같은 정적 웹 호스팅에 올립니다.
2. 생성된 https:// 주소를 iPhone에서 엽니다.
3. iPhone의 공유 메뉴에서 '홈 화면에 추가'를 선택합니다.
4. 홈 화면의 '일본어게임' 아이콘을 누르면 앱처럼 전체화면으로 실행됩니다.
5. 첫 접속 후에는 게임 파일이 캐시되어 오프라인에서도 사용할 수 있습니다.

[iPhone 15 Pro 최적화]
- 세로 화면 우선
- 15초 낙하
- 키보드 표시 시 게임판 자동 축소
- 하단 입력창 고정
- Safe Area 대응
- 중복 방지 덱 출제

[업데이트]
웹 파일을 교체한 뒤 sw.js의 CACHE_NAME을 v2, v3 등으로 바꾸면
사용자 기기에 새 버전 캐시가 적용되기 쉽습니다.
