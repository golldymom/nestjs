<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://coveralls.io/github/nestjs/nest?branch=master" target="_blank"><img src="https://coveralls.io/repos/github/nestjs/nest/badge.svg?branch=master#9" alt="Coverage" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.



typesrit, node, nest.js, tyeorm, postgresql을 사용하여 회원(생성, 로그인(토큰생성))기능, 게시판(생성(private, public 구분), 확인, 삭제, 수정)기능, 에러처리, 로그를 구현했습니다.

## Installation

```bash
$ npm i
```
## pg 연결
포스트그래스와 연결이 되어야 서비스가 실행됩니다.
포스트그래스가 깔려있으시다면 
config 폴더의 default.yaml파일에서 포트 번호를 해당 컴퓨터에 깔린 포스트그래스의 포트번호로 맞춰주세요. 
데이터베이스 이름을 확인해서 포스트그래에서 같은 이름으로 만들어 주세요.
같은 폴더의 development.yaml 파일에서 호스트, 유저네임, 패스워드를 컴퓨터에 깔린 포스트그래스의 호스트, 유저네임, 패스워드로 바꿔주세요.



## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## 앱 시작 후
```브라우저에서 localhost:4000으로 들어갈것
 브라우저는 404 NOT FOUND라고 뜨지만 서버는 켜진 상태입니다.

```
## 앱 시작 후
postman을 이용해서 접근합니다.(경로 및 방식) 

로그인 후 토큰이 발생하면 토큰을 게시글 작업시 꼭 챙겨주세요


-회원가입(/auth) - create(post) -생성(/signup) "username, password"

          - read(post) -읽기(/signin) "username, password"


- 게시글(/boards)  - create(post) - 생성(/),"title,description,status"(status는 기본적으로 퍼블릭으로 걸려 있습니다.)

          - read(get)id로 - 모든 게시글 읽기(/)


          - read(get)id로 - 게시글 읽기(/:id)


          - update(patch) - 게시글 수정(/:id/status)


          - delete(delete) - 게시글 삭제(/:id)


Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)




