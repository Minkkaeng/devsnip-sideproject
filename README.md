# DevSnip

React + TypeScript + JavaScript + CSS 실무 스니펫을 빠르게 검색하고 복사하는 원클릭 코드 치트시트입니다.

**라이브 데모:** https://minkkaeng.github.io/devsnip-sideproject/

개발 중 문법과 타입 선언을 다시 찾아야 할 때, 스택과 카테고리를 고르고 예제·주의점을 한 화면에서 확인한 뒤 필요한 언어의 코드만 복사할 수 있도록 만들었습니다.

## 실행

Node.js 22.12 이상 또는 24 LTS 환경을 사용하세요.

```sh
npm install
npm run dev
```

터미널에 표시되는 localhost 주소에서 확인할 수 있습니다.

```sh
npm run test    # 검색·상태·사용자 흐름·클립보드·스니펫 코드 검사
npm run lint    # 코드 정적 검사
npm run build   # 타입 검사 후 dist 생성
npm run preview # 빌드 결과 확인
npm run format # 코드·문서 포맷 정리
npm run format:check # 포맷 확인
```

## 구현된 기능

- 스택 & 카테고리 → 목록 → 상세의 데스크톱 3단 레이아웃
- 모바일 Drawer와 목록/상세 화면 전환
- 54개 스니펫: React 14개 / TypeScript 13개 / JavaScript 16개 / CSS 11개
- title, summary, tags 퍼지 검색과 카테고리 필터
- 항목별 JS / TS / CSS 코드 탭, JSX / TSX 포함 코드 하이라이팅
- 원클릭 복사, 성공/실패 토스트, 실무 Gotcha 아코디언
- 결과 없음 처리와 필터·선택 항목 동기화
- 키보드 조작과 reduced-motion 대응

## 검증과 다음 작업

GitHub Actions가 포맷·린트·테스트·빌드를 통과한 `dist`를 GitHub Pages에 배포합니다.
