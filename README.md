# cursor-demo

**v1.0.0** — 사용자 목록에서 유효한 이메일만 추출·검증하는 이메일 모듈과 테스트 스위트를 추가했습니다.

## ✨ 기능

- **이메일 모듈** (`src/email.js`)
  - `extractEmails` — 사용자 배열에서 이메일 주소 추출
  - `isValidEmail` — 이메일 형식 유효성 검사
  - `getValidEmails` — 유효한 이메일만 필터링해 반환
- **검증 유틸** (`Docs/validator.js`)
  - `filterValid` — 배열 항목을 조건 함수로 걸러내는 공통 검증 함수
- **배열 유틸** (`src/utils.js`)
  - `unique` — 중복 제거(첫 등장 순서 유지)
- **테스트** (`src/email.test.js`)
  - Node.js 내장 테스트 러너(`node --test`)로 이메일 모듈 단위 테스트 추가
- **npm 스크립트**
  - `npm start` — `src/index.js` 데모 실행
  - `npm test` — 이메일 테스트 실행

## 🐛 버그 수정

- (해당 없음)

## 🧹 기타

- CommonJS → **ES Modules**(`"type": "module"`) 전환
- 진입점을 `index.js` → `src/index.js`로 이동
- `index.js` 데모를 이메일 유효성 검사 예제로 교체
