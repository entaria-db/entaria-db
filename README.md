# ENTARIA DB

메이플스토리 월드 **엔타리아** 비공식 팬 데이터베이스입니다.
서버·DB·로그인 없이 정적 파일만으로 동작하며, GitHub Pages로 배포합니다.

## 파일 구성

| 경로 | 내용 |
|---|---|
| `index.html` | 첫 화면. 보안 정책(CSP) 포함 |
| `assets/app.js` | 데이터(룬워드·룬·큐브·지도)와 화면 로직, 한국어 문구 |
| `assets/icons.js` | 아이템·룬·몬스터 아이콘 묶음 |
| `assets/eq-data.js` | 장비 데이터 (아이템·검색·패치 내역 화면에서 불러옴) |
| `assets/eq/` | 장비 아이콘 1,860개 (화면에 보이는 것만 불러옴) |
| `assets/i18n-*.js` | 영어·일본어·중국어 번역 (언어를 고를 때 불러옴) |
| `assets/style.css` | 스타일 |
| `assets/map.webp` | 대륙 지도 |
| `_headers` | Cloudflare Pages용 보안 헤더 (GitHub Pages는 무시해도 됨) |
| `robots.txt` | 검색엔진 수집 허용 |
| `.nojekyll` | GitHub Pages가 파일을 가공 없이 그대로 배포하도록 함 |

## 배포 (GitHub Pages)

1. 저장소 루트에 위 파일을 그대로 올립니다 (zip 파일 자체가 아니라 압축을 푼 내용). 파일이 1,800개가 넘어 웹 업로드 대신 git으로 push하세요.
2. Settings → Pages → Build and deployment → Source: **Deploy from a branch**,
   Branch: **main** / **(root)** → Save
3. 1~2분 뒤 `https://<아이디>.github.io/<저장소 이름>/` 에서 열립니다.
4. 업데이트는 새 파일로 덮어쓰고 커밋하면 자동 반영됩니다.

## 데이터 출처와 저작권

- 게임 내 명칭과 이미지의 권리는 NEXON 및 Entaria 크리에이터 그룹에 있습니다. 비영리 팬 사이트입니다.
- 룬워드·룬·큐브 데이터: 게임 내 툴팁과 공식 다국어 룬워드 자료
- 원석·보석·포션·화살 아이콘과 장비 데이터: 원작 메이플스토리 GMS v83 WZ 공개 덤프
  (github.com/andrenogrib/gms_v83_wztoweb)
- 몬스터 이미지: 같은 GMS v83 공개 덤프의 Mob 이미지 (엔타리아 고유 몬스터는 이미지 없음)
- 장비 한국어 이름: 메이플랜드 DB 공개 저장소 (github.com/JooYoung1121/maple_db)
- 장비 중국어 이름: TMS v62 문자열 (간체는 자동 변환), 일본어는 영어 이름 표시
- 장비 데이터는 원작 기준이라 엔타리아 실제 능력치·드랍과 다를 수 있습니다.
