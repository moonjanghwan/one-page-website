one page여행 웹사이트 제작 사양서

1. 프로젝트 개요
    프로젝트명: One page 여행 웹사이트
    프로젝트 유형: 반응형 One Page 웹사이트
    개발 환경: Next.js, React

2. 기술 스택
    프론트엔드
    Next.js
    React
    CSS Modules
    Font Awesome (아이콘)
    Google Fonts (Noto Sans KR)

3. 데이터 구조
   3.1 여행 일정 데이터
        ```javascript
        const scheduleData = [
        { city: "프라하", arrival: "04/25(금)", departure: "05/01(목)", nights: 6 },
        { city: "자그레브", arrival: "05/01(목)", departure: "05/05(월)", nights: 4 },
        { city: "Ljubljana", arrival: "05/05(월)", departure: "05/10(토)", nights: 5 },
        { city: "Piran/Rovinj", arrival: "05/10(토)", departure: "05/12(월)", nights: 2 },
        { city: "Plitvicka", arrival: "05/12(월)", departure: "05/16(금)", nights: 4 },
        { city: "Zadar", arrival: "05/16(금)", departure: "05/18(일)", nights: 2 },
        { city: "Split", arrival: "05/18(일)", departure: "05/21(수)", nights: 3 },
        { city: "Dubrovnik", arrival: "05/21(수)", departure: "05/25(일)", nights: 4 },
        { city: "Istanbul", arrival: "05/25(일)", departure: "05/30(금)", nights: 5 },
        { city: "인천", arrival: "05/31(토)", departure: "", nights: 1 }
        ];
        ```

    3.2 예산 데이터


        const budgetData = [
        { 
            category: "항공권", 
            foreignAmount: "", 
            koreanAmount: "₩2,117,151", 
            moonShare: "₩2,117,151.00", 
            yangShare: "₩3,181,400.00", 
            note: "" 
        },
        { 
            category: "렌트카", 
            foreignAmount: "$1,789.00", 
            koreanAmount: "₩2,415,150", 
            moonShare: "₩1,207,575.00", 
            yangShare: "₩1,207,575.00", 
            note: "미확정" 
        },
        { 
            category: "숙소", 
            foreignAmount: "", 
            koreanAmount: "₩4,840,861", 
            moonShare: "₩2,762,394.00", 
            yangShare: "₩2,078,467.00", 
            note: "" 
        }
        // ... 기타 예산 항목
        ];

4. 컴포넌트 구조

    4.1 Header 컴포넌트
        - 반응형 네비게이션 바
        - 메뉴 항목: 홈, 여행 계획, 최근 여행지, 블로그, 연락처
        - 스크롤 시 배경색 변경 효과
        - 모바일 햄버거 메뉴 지원

    4.2 Hero 컴포넌트 
        - 전체 화면 이미지 캐러셀
        - 자동/수동 이미지 슬라이드 기능
        - 중앙 정렬된 설명 텍스트 오버레이
        - 페이지 내용 소개 자막
        - 캐러셀 네비게이션 컨트롤
        - 반응형 디자인 지원


    4.3 Home 컴포넌트
        전체 화면 배경 이미지
        중앙 정렬된 타이틀과 서브타이틀
        CTA 버튼


    4.4 TravelPlan 컴포넌트
        여행 일정 테이블
        예산 계획 테이블
        반응형 레이아웃

    4.5 TravelHistory 컴포넌트
        여행지 카드 그리드 레이아웃
        이미지 갤러리
        필터링 기능

    4.6 Blog 컴포넌트
        블로그 포스트 목록
        카테고리 필터
        검색 기능

    4.7 Contact 컴포넌트
        연락처 정보
        소셜 미디어 링크
        문의 양식

5. 파일 구조
   
    one-page-website/
    ├── components/
    │   ├── Header/
    │   │   ├── index.js
    │   │   └── Header.module.css
    │   ├── Home/
    │   │   ├── index.js
    │   │   └── Home.module.css
    │   ├── TravelPlan/
    │   │   ├── index.js
    │   │   └── TravelPlan.module.css
    │   ├── TravelHistory/
    │   │   ├── index.js
    │   │   └── TravelHistory.module.css
    │   ├── Blog/
    │   │   ├── index.js
    │   │   └── Blog.module.css
    │   └── Contact/
    │       ├── index.js
    │       └── Contact.module.css
    ├── pages/
    │   └── index.js
    ├── styles/
    │   └── globals.css
    └── public/
        └── images/

6. 반응형 디자인
    모바일: 360px ~ 767px
    태블릿: 768px ~ 1023px
    데스크톱: 1024px 이상

7. 성능 최적화
    이미지 최적화
    CSS Modules 사용
    컴포넌트 코드 분할

8. 브라우저 지원
    Chrome (최신 버전)
    Firefox (최신 버전)
    Safari (최신 버전)
    Edge (최신 버전)

9. 배포
    Vercel 또는 GitHub Pages

10. 추가 기능
    다크 모드 지원
    스크롤 애니메이션
    반응형 이미지 처리
    웹 접근성 준수



    