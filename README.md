# FastCampus Site

## Contributor

## Tech Requirement (Tech Stack)

- Create-next-app
- Next.js
- Typescript
- ESLint
- Babel 설정 (IE 11 대응)

  Babel 설정은 IE11 때문에 필요합니다.
  Next 에서 기본으로 IE11 을 지원하기는 하지만 Babel 설정을 했을 때 Build 되는 결과물이 달라집니다.
  Babel 설정을 반드시 해야 IE11 에 대한 대응이 Default 로 이루어집니다.
  최근에 나온 스펙들의 경우 built in 시점에 지원을 안하는 경우가 있습니다.
  그런걸 방지하기 위해서도 babel 설정은 해두는 것이 좋습니다.

https://nextjs.org/docs/advanced-features/customizing-babel-config  
babel 설정을 바꾸게 되면 ES2015 이전 문법으로 지원을  
해주기 때문에 IE11 에서도 동작하는 것을 .next 폴더에서 살펴볼수 있습니다.

## Docker

- Dockerfile을 이용해서 Docker Container 를 생성합니다.
- Docker Compose 를 사용하고 있습니다.

## Script

```
$ yarn dev
```

```
$ yarn build
$ yarn deploy
```

## 테스트

- Jest
- npm run test
