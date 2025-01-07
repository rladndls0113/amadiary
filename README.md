

#### 경고문 (WRAING)
- - -
1. 이 문서는 25.01.07 작성된 문서입니다.
2. amadiary를 cafe24 --> aws 이동을 위해 git에 포함했습니다.
3. 이 README.md는 마크다운 문법으로 작성 되었습니다.
4. 이 문서와 폴더 구조는 vue,php 기준으로 작성되었습니다.
5. 마이그레이션 혹은 리팩토링 시 폴더 구조와 시스템적인 변경이 필요합니다.


#### 파일별 설명
- - -
- public                    # 정적 파일들을 저장합니다.
    - favicon.ico           # 메인 HTML 파일입니다.
    - index.html            # 웹사이트의 파비콘 아이콘입니다.
- src                       # 소스 코드를 저장하는 디렉터리입니다.
    - config                # 콘픽(환경설정)
        - global.js         # 전역 js
        - devlop.js         # 개발 환경 설정
        - production.js     # 배포 환경 설정
    - services              # 서비스 폴더(상시 돌아가는)
        - api.js            # API 호출 로직
        - auth.js           # 인증 관련 로직
        - utils.js          # 공통 유틸리티
    - assets/resource       # 이미지, CSS 파일 정적파일들을 저장합니다.
    - components            # 재사용 가능한 UI 컴포넌트들을 저장합니다.
    - test                  # 테스트 코드를 저장합니다.
    - bootstrap             # 프레임워크 초기화, path & 환경 설정 등 framework boot
    - config/global         # 앱 전체에 적용되는 설정
    - App.vue               # 최 상위 컴포넌트
    - main.js               # 애플리케이션 진입점
- storages                  # 업로드, 캐시 등 파일을 저장합니다.
    - uploads               # 업로드
    - cache                 # 캐시
    - temp                  # 템프
- docs                      # 문서를 저장합니다.
    - guides                # 가이드 문서 폴더
        - api.md            # API 명세
        - setup.md          # 설치
        - basic.md          # 기본설명
        - patch.md          # 패치 로그
- vue.config.js             # vue에 대한 설정(웹팩 등)을 하기 위한 환경설정 파일
- .gitignore                # 깃 검열 파일
- package-lock.json         # package-lock.json
- package.json              # 로젝트 정보와 의존성(dependencies)을 관리하는 문서
- Readme.md                 # 프로젝트에 대한 설명


#### GIT 컨벤션
- - -
0. 구조
    - type(타입) : subject(제목)
    - body(바디)
    - footer(푸터)
1. 커밋 타입
    - feat: // 새 기능 추가
    - fix: // 코드(버그) 수정
    - docs: // 문서 수정
    - style: // 코드 포맷팅, 세미콜론 누락, 코드 미 변경
    - refactor: // 코드 리펙토링
    - test: // 테스트 코드, 리펙토링 테스트 코드 추가
    - chore: // 빌드 업무 수정, 패키지 매니저 수정
2. 제목 작명
    - 최대 50글자 마침표 및 특수기호 X
    - 영문 표기시 동사(원형)이 맨앞, 첫글자는 대문자 (과거 시제는 X)
    - 제목은 개조식 구문으로 작성한다. (즉, 간단하고 요점만.)
    - 예시
        1. Fixed --> Fix
        2. Added --> Add
        3. Modified --> Modify
3. 바디
    - 줄당 72자 이내로 작성
    - 양은 무관 최대한 상세히 기제
    - 어떻게 바꿨는지 X --> 무엇을 왜 바꿧는지 기제
4. 푸터
    - 꼬리말은 optional 이고, 이슈 트래커 ID를 작성한다
    - 꼬리말은 "유형:#이슈번호" 형식으로 작성한다
    - 여러개의 이슈 번호는 쉼표(,)로 구분한다
    - 이슈 트래커의 유형은 다음 중 하나로 사용한다
        1. Fixes: 이슈 수정중 (아직 미해결)
        2. Resolves: 해결완료
        3. Ref: 참고 이슈
        4. Related to: 해당 커밋 이슈번호 (아직 미해결)
        - ex: Fixes: #45 Relate to #34, #23


#### 사용중 (API, 라이브러리, 언어 등)
1. 언어
2. API
3. 라이브러리


#### 작업파일 및 링크
- - -
1. 프로그램
    1. 메인 작업파일
    2. 서브 작업파일
    3. 기타 (API 등)
2. 개발 디자인
    1. UX/UI
    2. IMG/AESSET
    3. 기타
3. 기타
    1. 기획 문서 (오더)
    2. 참고 자료 및 문헌
    3. 기타


#### 참고 Git Emogi
- 🎨 // 새 코드의 형식 및 구조 개선
- 📰 // 새 파일 생성
- 📝 // 사소한 코드 혹은 언어 변경시
- 🐎 // 성능 향상시
- 📚 // 문서 작성시
- 🐛 // 버그 리포팅 @FIXME 주석 태그 삽입
- 🚑 // 버그 픽스 때
- 🔥 // 코드 또는 파일을 제거 시 @CHANGED 주석 태그와 함께
- 🚜 // 파일 구조를 변경할 때 🎨와 함께
- 🔨 // 코드를 리펙토링 할 때
- 💄 // UI/STYLE 개선시
- ♿️ // 접근성을 향상 시킬 때
- 🚧 // WIP(작업중)에 커밋 @REVIEW 주석 태그와 함께
- 💎 // NEW Release
- 🔖 // 버전 tag
- ✨ // 새 기능 소개 시
- ⚡️ // 도입 할 때 이전 서버와 호환되지 않는 특징 @CHANGED 주석 태그와 함께
- 💡 // 새로운 아이디어 @IDEA 주석 태그
- 🚀 // 배포 / 개발 작업과 관련된 모든 것