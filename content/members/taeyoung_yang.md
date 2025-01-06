---
title: Members
type: about
---

## Taeyoung Yang

![image](/asset/images/taeyoung_yang_profile.jpeg)

편리한 세상을 위한 불편한 개발자, 양태영입니다. 

현직 3년차 백엔드 엔지니어로 유한회사 일루미나리안에서 재직 중입니다.

### About Me
{{< cards >}}
{{< card link="https://github.com/YangTaeyoung" title="Github" icon="user" >}}
{{< card link="https://yangtaeyoung.github.io" title="기술 블로그" icon="home" >}}
{{< card link="mailto:0130yang@gmail.com" title="이메일 보내기" icon="mail" >}}
{{< /cards >}}

### Role in Project 555
#### 팀 리딩
- 매주 수요일, 일요일에 이루어지는 프로젝트 스크럼를 통해 진행상황을 팀원과 공유하고, 개발 및 의사결정이 필요한 부분에 대해 토론하고, 팀원들의 의견을 수렴하여 프로젝트를 진행하였습니다.
- 회의 내용을 정리하여 [Github Discussion](https://github.com/project-555/project-555/discussions/categories/scrum)에 공유하고, 팀원들의 의견을 수렴하였습니다.
- 기술조사가 필요한 부분에 대해 [스터디](https://github.com/project-555/plog-study)를 선제적으로 진행하여, 팀원들이 공통의 이해선상에서 개발을 진행할 수 있도록 노력하였습니다.
- 전반적인 개발사항에 대한 이슈잉, 코드 리뷰를 통해 Plog가 퀄리티 높은 개발을 진행할 수 있도록 하였습니다.

#### 백엔드 파트
- 백엔드 파트의 전반적인 아키텍처를 설계하고 방향성을 제시하였습니다.
- AWS의 리소스 책임자로서, ECS, RDS, ELB, VPC, S3 등을 구성하여 Plog의 백엔드 서버를 배포하였습니다.
    - AWS RDS를 구성하고, PostgreSQL 데이터 베이스의 내부 스키마를 설계하였습니다.
    - AWS ECS를 구성하고, Dockerfile을 작성하여 Plog의 백엔드 서버를 배포하였습니다.
    - AWS ELB를 구성하여, Plog의 백엔드 서버에 SSL 인증서를 적용하였습니다.
- Spring 백엔드 서버 개발을 담당하였습니다.
    - 초기 서버 세팅을 담당하였고, 다음과 같은 작업을 수행하였습니다.
        - JPA datasource 및 연동을 담당하였습니다.
    - Redis(ElasticCache)를 통해 이메일 인증 파트를 구현하였습니다.
    - Spring Security를 통해 JWT 인증 구현하였습니다.
    - Spring Data JPA, QueryDSL을 통해 데이터베이스 연동하였습니다.
    - AWS S3 Pre-Signed URL을 통한 파일 업로드 구현하였습니다.
    - Spring AOP를 통한 로깅 라이브러리 보완하였습니다.
    - Spring Filter를 통한 로깅 라이브러리 보완하였습니다.
    - Spring Exception Handler를 통한 전반적인 에러 핸들링을 구현하였습니다.
        - Enum을 통해 에러 코드 및 에러 메시지에 대한 명세를 단순화하여 작성할 수 있도록 컴포넌트를 표준화 하였습니다.
    - Spring Validation을 통한 데이터 유효성 검사를 구현하였습니다.

#### 프론트 파트
- 유저 블로그 홈 페이지 및 관련 컴포넌트를 구현하였습니다.
    - `X시간 전`, `X분 전`과 같이 상대 시간을 표시하는 컴포넌트를 구현하였습니다.
    - 카테고리 리스트, 필터링 컴포넌트를 구현하였습니다.
    - 태그 리스트, 필터링 컴포넌트를 구현하였습니다.
- 유저 블로그 포스팅 작성 페이지 및 관련 컴포넌트를 구현하였습니다.
    - [NHN Toast UI Editor](https://ui.toast.com/tui-editor)를 통한 블로그 게시글 작성 마크다운 에디터 컴포넌트를 구현하였습니다.
- 유저 인증 JWT 토큰 리프레시 로직을 구현하였습니다.

#### 문서화 파트
- Hugo를 통해 해당 블로그를 Github Pages를 활용하여 배포하였습니다.
- [_"Plog Back"_](/docs/plog-back/) 문서를 작성하였습니다.
- [_"Plog의 백엔드 서버 배포 시퀀스 읽어보기"_](/docs/plog-back/backend_deploy_sequence/) 문서를 작성하였습니다.
- [_"Plog의 인증은 어떻게 구현되었을까?"_](/docs/plog-back/authorization/) 문서를 작성하였습니다.
- [_"S3 Pre-signed URL로 구현한 파일 업로드 읽어보기"_](/docs/plog-back/file_upload_with_s3/) 문서를 작성하였습니다.
- [_"Spring 테스트 커버리지, 모두 볼 수 있도록 리포트를 공유해보자"_](/docs/plog-back/testing_report/) 문서를 작성하였습니다.
- [_"Plog의 이메일 인증 Redis와 함께 이렇게 구현했습니다!"_](/docs/plog-back/email_verification) 문서를 작성하였습니다.
- [_"Plog의 데이터베이스와 서버의 연결 구성 살펴보기"_](/docs/plog-back/db_server_design/) 문서를 작성하였습니다.
- [_"Convention"_](/docs/convention/) 문서를 작성하였습니다.
- [_"Scrum Convention"_](/docs/convention/scrum_convention/) 문서를 작성하였습니다.
- [_"Study Convention"_](/docs/convention/study_convention/) 문서를 작성하였습니다.
- [_"Github Convention"_](/docs/convention/github_convention/) 문서를 작성하였습니다.
