---
title: Research & Study
date: 2023-11-06T21:26:48+09:00
toc: true
prev: docs/
next: docs/plog-back/
---
해당 페이지에서는 Plog를 구현하기 위한 기술 스택 정의 및 초기 기술 조사 시점에서 진행한 스터디 목록을 명세합니다.

# Stacks
Plog를 구현하면서 사용한 기술 스택은 다음과 같습니다.

## Frontend
#### Frontend Framework
- [ReactJS](https://ko.legacy.reactjs.org/)
#### UI Framework
- [Material UI](https://mui.com/)
#### Markdown Editor
- [Toast UI Editor](https://ui.toast.com/)

## Backend
#### Backend Framework
  - [Spring](https://spring.io/)

#### Authentication & Security
  - [Spring Security](https://spring.io/projects/spring-security)

#### Databases
- [PostgreSQL](https://www.postgresql.org/) ([AWS RDS](https://aws.amazon.com/ko/rds/))
- [Redis](https://redis.io/) ([AWS ElasticCache](https://aws.amazon.com/ko/elasticache/))

#### Container & Orchestration
- [Docker](https://www.docker.com/)
- [AWS ECS](https://aws.amazon.com/ko/ecs/)

#### CI/CD
- [Github Action](https://docs.github.com/ko/actions)


# Study
![image](./asset/images/_index-1699279733409.png)

Plog의 첫 기술조사 후 구성원들이 잘 모르는 기술을 공부하고 해당 기록을 Github Repository([plog-study](https://github.com/project-555/plog-study))에 문서화하였습니다.

## Frontend
- [Vue.js](https://github.com/project-555/plog-study/tree/main/vue.js)
  - [Vue 구동하기](https://github.com/project-555/plog-study/blob/main/vue.js/01.start-with-vue.md)
  - [SFC](https://github.com/project-555/plog-study/blob/main/vue.js/02.SFC.md)
  - [Vue 개요](https://github.com/project-555/plog-study/blob/main/vue.js/03.what-is-vue.md)
  - [Vue 기본 개념](https://github.com/project-555/plog-study/blob/main/vue.js/04.vue-overview.md)
  - [Vue 기본 문법](https://github.com/project-555/plog-study/blob/main/vue.js/05.vue-syntax.md)
  - [Vue 상태관리 패턴](https://github.com/project-555/plog-study/blob/main/vue.js/06.state-management-pattern.md)
## Backend
- [Spring](https://github.com/project-555/plog-study/tree/main/spring)
  - [Spring 개요](https://github.com/project-555/plog-study/blob/main/spring/01.what-is-spring.md)
  - [웹 개발 개론](https://github.com/project-555/plog-study/blob/main/spring/02.web.md)
  - [Spring Boot](https://github.com/project-555/plog-study/blob/main/spring/03.spring-boot.md)
  - [Controller 기본 동작](https://github.com/project-555/plog-study/blob/main/spring/04.server.md)
  - [IOC와 DI](https://github.com/project-555/plog-study/blob/main/spring/05.ioc-and-di.md)
  - [AOP](https://github.com/project-555/plog-study/blob/main/spring/06.aop.md)
  - [Object Mapper](https://github.com/project-555/plog-study/blob/main/spring/07.object-mapper.md)
  - [Validation](https://github.com/project-555/plog-study/blob/main/spring/08.validation.md)
  - [Exception](https://github.com/project-555/plog-study/blob/main/spring/09.exception.md)
  - [Filter & Interceptor](https://github.com/project-555/plog-study/blob/main/spring/10.filter-interceptor.md)
  - [Asynchronous](https://github.com/project-555/plog-study/blob/main/spring/11.asynchronous.md)
  - [Server to Server](https://github.com/project-555/plog-study/blob/main/spring/12.server-to-server.md)
  - [Spring Data JPA](https://github.com/project-555/plog-study/blob/main/spring/jpa.md)
  - [Junit Test](https://github.com/project-555/plog-study/blob/main/spring/junit.md)
  - [Swagger](https://github.com/project-555/plog-study/blob/main/spring/swagger.md)
- [Docker](https://github.com/project-555/plog-study/tree/main/docker)
  - [Docker 개요](https://github.com/project-555/plog-study/blob/main/docker/01.what-is-docker.md)
  - [Docker 기초 따라하기, `create`, `start`, `exec`, `run`](https://github.com/project-555/plog-study/blob/main/docker/02.getting-start-docker.md)
  - [Docker Storage](https://github.com/project-555/plog-study/blob/main/docker/03.docker-storage.md)
  - [Dockerfile](https://github.com/project-555/plog-study/blob/main/docker/04.dockerfile.md)
  - [Docker Compose](https://github.com/project-555/plog-study/blob/main/docker/05.docker-compose.md)
- [AWS ECS](https://github.com/project-555/plog-study/blob/main/aws/ecs.md)
- [Github Action](https://github.com/project-555/plog-study/blob/main/aws/github-action.md)