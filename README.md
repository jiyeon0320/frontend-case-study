# Frontend Case Studies

실서비스에서 사용자 문제를 구조화하고, 실험과 운영 가능한 구현으로 연결한 사례를 정리한 저장소입니다.

저는 React, Next.js, TypeScript 기반 서비스에서 온보딩, 인증, 결제, 계측, 개인화, 공통 UI 구조를 설계·개선하며 사용자 경험과 운영 안정성을 함께 높여 왔습니다.  
이 저장소에는 그중에서도 제품과 프론트엔드가 맞물리는 문제를 어떻게 정의하고, 어떤 판단을 내렸고, 어떤 결과를 만들었는지를 정리합니다.

## Focus

- Product-oriented frontend engineering
- User flows and state transitions
- SSR / data fetching / caching strategy
- Analytics and experimentation
- Hybrid app and WebView flows

## Case Studies

- [Onboarding Funnel Redesign](./case-studies/01-onboarding-funnel-redesign/01-onboarding-funnel-redesign.md)

## Development

Node.js 22 LTS와 npm을 사용합니다.

```bash
npm ci
npm run dev
```

브라우저에서 http://localhost:3000 을 엽니다.

```bash
npm run lint
npm run typecheck
npm run build
npm start
```

- `src/app/`: Next.js App Router 페이지와 레이아웃
- `src/features/`: 케이스별 기능 구현 시 추가할 컴포넌트와 로직
- `src/components/`: 여러 케이스에서 공유하는 UI가 생기면 추가
- `case-studies/`, `subscription/`: 기존 사례 문서와 프로토타입 원본

실행 앱의 TypeScript 검사 범위는 `src/`이며, 기존 프로토타입은 앱으로 옮길 때 통합합니다.

## Tech

React · Next.js · TypeScript · GraphQL · GA4/GTM · Playwright

## Notes

- 회사 내부 코드와 비공개 정보는 포함하지 않았습니다.
- 사례는 실무 경험을 바탕으로, 공개 가능한 수준에서 일반화해 정리했습니다.
