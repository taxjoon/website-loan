# (주)제이유 금융대부 공식 웹사이트

부동산담보대출 및 전당포대출 전문 대부업체 (주)제이유 금융대부의 공식 홈페이지입니다.

- **상호** (주)제이유 금융대부
- **대표이사** 김형준
- **대부업등록번호** 2025-서울강남-0054(대부업)
- **대부업등록기관** 강남구청 지역경제과 (02-3423-5522)
- **대표전화** 010-3094-5516

## 구조

```
.
├── index.html             메인 페이지
├── css/style.css          스타일
├── js/main.js             모바일 메뉴 토글
├── images/                등록증 이미지
├── docs/                  약관 7종
│   ├── service-terms.html        서비스 이용약관
│   ├── privacy.html              개인정보처리방침
│   ├── no-spam.html              이메일무단수집거부
│   ├── credit-info.html          신용정보활용체제
│   ├── illegal-collection.html   불법채권추심 대응요령
│   ├── collection-process.html   채권추심업무 처리절차
│   └── expired-debt.html         소멸시효완성 채권 안내
├── docker-compose.yml     로컬 nginx 컨테이너 (포트 8081)
├── nginx.conf
└── .github/workflows/     GitHub Pages 자동 배포
```

## 로컬 실행

```bash
docker compose up -d
```

브라우저에서 http://localhost:8081 접속.

중지:
```bash
docker compose down
```

## GitHub Pages 배포

`main` 브랜치에 push하면 `.github/workflows/pages.yml`이 자동으로 사이트 전체를 GitHub Pages에 배포합니다.

### 최초 설정

1. GitHub repository 생성 후 `main` 브랜치로 push
2. Repository **Settings → Pages → Source** 항목에서 **GitHub Actions** 선택
3. Actions 탭에서 워크플로 완료 확인 → 발급된 URL로 접속

## 필수 게시 정보 (대부업법 준수)

- 대출금리 : 연 20% 이내
- 연체금리 : 약정이자율 + 3% 이내 (연 20% 이내)
- 부동산담보대출 부대비용 : 등록면허세, 지방교육세, 등기신청수수료, 국민주택채권매입비, 주소변경비용, 확인서면비용, 근저당말소비용 등
- 전당포대출 부대비용 : 없음
- 조기상환 조건 : 없음
- 개인정보 관리책임자 : 대표이사 김형준
