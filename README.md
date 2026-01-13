# 🚀 커리어 매칭 플랫폼 'Meet U, Career' - Backend

**Spring Boot 기반의 커리어 매칭 플랫폼 'Meet U, Career' 백엔드 API 서버입니다.**

총 6명의 팀원이 프론트엔드와 백엔드를 함께 개발하며, 실제 서비스 수준의 웹 애플리케이션 개발 전반을 경험하는 것을 목표로 진행한 프로젝트입니다.

---

## 👨‍💻 담당 역할 (My Contribution)

이 프로젝트의 백엔드 개발에 참여하여 다음과 같은 핵심 기능들을 설계하고 구현했습니다.

- 기업회원 JWT 로그인 및 회원가입
- 마이페이지 면접 현황 조회 및 리뷰 작성
- 커뮤니티 게시판 CRUD 및 외부 뉴스 API 연동
- 관리자용 공고관리 (조회, 승인, 반려)

---

## 🔧 Tech Stack

- **Backend**: Spring Boot, Spring Security, Java
- **Database & ORM**: MySQL, JPA/Hibernate, QueryDSL
- **API & Auth**: REST API, JWT (JSON Web Token), Swagger
- **Infra & CI/CD**: AWS EC2, Docker, Nginx, GitHub Actions
- **Build Tool**: Gradle
- **Collaboration**: Jira, Confluence, Slack, Figma

---

## 💡 주요 기능 및 기술적 특징

- **복잡한 동적 쿼리 구현**: `QueryDSL`을 활용하여 다양한 조건의 채용 공고 필터링 및 검색 기능을 구현했습니다. 컴파일 시점에 SQL 오류를 잡을 수 있어 안정성을 높였습니다.
- **토큰 기반 인증 시스템**: 세션 방식이 아닌 `JWT`를 도입하여, Access/Refresh 토큰 기반의 stateless 인증 시스템을 구축했습니다. 이를 통해 서버의 확장성과 보안을 확보했습니다.
- **자동화된 배포 파이프라인**: `GitHub Actions`와 `Docker`를 연동하여, main 브랜치에 코드가 푸시되면 자동으로 빌드 및 테스트, 배포가 이루어지는 CI/CD 파이프라인을 구축했습니다.
- **실시간 통신 기능**: `WebSocket`을 활용하여 사용자 간 실시간 채팅 기능을 구현했습니다.
- **소셜 로그인**: `OAuth2`를 도입하여 사용자가 카카오 계정으로 간편하게 로그인할 수 있도록 구현했습니다.

---

## 🏗️ 아키텍처

`Frontend (Next.js)` ↔ `Backend API (Spring Boot)` ↔ `Database (MySQL)` 구조로, 백엔드 서버는 MVC 패턴을 기반으로 설계되었습니다.

- **Controller**: API 엔드포인트를 정의하고 사용자의 요청을 처리합니다.
- **Service**: 비즈니스 로직을 수행하며, 트랜잭션을 관리합니다.
- **Repository & JPA/QueryDSL**: 데이터베이스와의 통신을 담당합니다.

---

## 🔗 관련 링크

- **프론트엔드 저장소**: [meet-u-career-frontend](https://github.com/dpdlcl01/meet-u-career-frontend)
- **API 명세서**: [Meet U - REST API 설계서](https://docs.google.com/spreadsheets/d/1h937tTBRhGLpmx_gNGGCkRQki3vEbtW5z_Nd3Rswu7s/edit?usp=sharing)
