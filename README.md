# 카운터 앱

React와 TypeScript를 사용하여 구현한 간단한 카운터 애플리케이션입니다. 버튼 클릭 시 카운트를 증가시키는 기능을 제공합니다.

## 기술 스택

- React 19.1.0: 컴포넌트 기반 UI 라이브러리
- TypeScript: 타입 안정성을 위한 정적 타입 언어
- Vite: 빠른 개발 서버 및 빌드 도구
- Biome: 코드 포맷팅 및 린팅 도구

## 주요 기능

카운터 기능
- useState 훅을 사용한 상태 관리
- 버튼 클릭 시 카운트 증가
- 실시간 카운트 값 표시

## 구현 세부사항

App 컴포넌트에서 useState 훅을 사용하여 count 상태를 관리합니다. 버튼 클릭 시 setCount 함수를 호출하여 카운트 값을 증가시키며, 함수형 업데이트 패턴을 사용하여 이전 상태를 기반으로 새로운 값을 계산합니다.

main.tsx에서는 React 19의 createRoot API를 사용하여 애플리케이션을 렌더링합니다. StrictMode로 감싸서 개발 모드에서 잠재적인 문제를 감지할 수 있도록 했습니다.

프로젝트는 Vite를 사용하여 빠른 개발 서버와 최적화된 프로덕션 빌드를 제공합니다. TypeScript 설정은 tsconfig.json을 통해 관리되며, Biome을 사용하여 코드 품질을 유지합니다.

## 프로젝트 구조

```
template_copy/
├── src/
│   ├── App.tsx
│   ├── main.tsx
│   └── vite-env.d.ts
├── public/
├── vite.config.ts
├── tsconfig.json
└── package.json
```
