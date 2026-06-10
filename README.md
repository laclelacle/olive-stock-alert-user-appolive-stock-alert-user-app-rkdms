# 올영세일 모바일 앱형 데모 - AWS Products API 연결 버전

## 구성
- `index.html`: GitHub Pages에 바로 올릴 메인 파일

## 적용 방법
1. GitHub repository 최상단의 기존 `index.html`을 백업합니다.
2. 이 폴더의 `index.html`을 업로드해서 기존 파일을 덮어씁니다.
3. GitHub Actions의 Pages 배포가 초록 체크로 완료될 때까지 기다립니다.
4. 브라우저에서 `Ctrl + F5` 또는 URL 뒤에 `?v=aws1`을 붙여 새로고침합니다.

## AWS 연결
기본 API 주소:
`https://ukxqcqhsr9.execute-api.ap-northeast-2.amazonaws.com`

앱 시작 시 아래 API를 호출합니다.
`GET /products/rankings?category=전체`

카테고리 버튼 클릭 시 해당 카테고리 API를 시도하고, 데이터가 없으면 전체 랭킹 데이터에서 로컬 필터링합니다.
