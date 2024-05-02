# 영화예매 웹 프로젝트

DEVELOPMENT MOTIVATION
---
> 영화 예매 사이트 -
> > -- 개발동기 적는부분<br> 
> > -- 에 의 불편함에 의해 ~~ <br> 
 

HISTORY
---
[TOTAL](DOCUMENT/HISTORY/TOTAL) | [이종일](DOCUMENT/HISTORY/이종일) | [정대민](DOCUMENT/HISTORY/정대민) | [강현우](DOCUMENT/HISTORY/강현우) | [이건무](DOCUMENT/HISTORY/이건무) | 


PLANS
---
 |LANGUAGE|PLAN|IMPLEMENT|DESCRIPTION|
 |-|-|-|-|
 |JAVA|-|-|-|
 |JSP/SERVLET|2024/04/24 ~ 2024/04/28|-|-|
 |SPRING STS3|-|-|-|
 |SPRING BOOT|-|-|-|
 
 

MEMBERERS
--- 
|NAME|ROLE|DETAILS|DESCRIPTION| 
|---|---|---|---|
|이종일|FN| FrontController / Docment 관리 / Dependencies  관리 |---|
|정대민|BN| USER - 회원가입 / 회원탈퇴 / 영화 CRUD|---|
|강현우|BN| 유저공통 - 로그인 / 로그아웃|---|
|이건무|BN| MANAGER 회원가입 회원탈퇴 영화 CRUD|---|

SKILLS
---

#### FN
---
<img src="https://img.shields.io/badge/HTML5-3366CC?style=for-the-badge&logo=htmlacademy&logoColor=white"> <img src="https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white"> <img src="https://img.shields.io/badge/JAVASCRIPT-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white"> <img src="https://img.shields.io/badge/JQUERY-0769AD?style=for-the-badge&logo=jquery&logoColor=white"> 


#### BN
---
<img src="https://img.shields.io/badge/JAVA-005571?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/JSP-1E8CBE?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/SERVLET-4B4B77?style=for-the-badge&logo=doubanread&logoColor=white"> <img src="https://img.shields.io/badge/SPRING-STS3-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/SPRINGBOOT-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> 

#### DATABASE
---
<img src="https://img.shields.io/badge/MYSQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white">  


#### DEVOPS
---
<img src="https://img.shields.io/badge/GIT-F05032?style=for-the-badge&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/GITHUB-181717?style=for-the-badge&logo=github2&logoColor=white"> <img src="https://img.shields.io/badge/AWS-EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"> <img src="https://img.shields.io/badge/DOCKER-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/DOCKERHUB-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/JENKINS-D24939?style=for-the-badge&logo=jenkins&logoColor=white"> 


END POINT DOC
---
|URI|REQUEST METHOD|REQUEST PARAMETER TYPE|RESPONSE VALUE TYPE|DESCRIPTION|
|---|---|---|---|---|
|/user/join|POST|---|---|---|
|/user/login|GET/POST|---|---|---|
|/user/logout|POST|---|---|---|
|---|---|---|---|---|
|/member/join|---|---|---|---|
|/member/remove|---|---|---|---|
|/member/resume/add|---|---|---|---|
|/member/resume/list|---|---|---|---|
|---|---|---|---|---|
|/admin/join|---|---|---|---|
|/admin/remove|---|---|---|---|
|/admin/company/read|---|---|---|---|
|---|---|---|---|---|

DEPENDENCIES LIST
---
|CAT|NAME|DESCRIPTION|LINK|-|-|
|-|-|-|-|-|-|
|FN|-|-|-|-|-|
|FN|-|-|-|-|-|
|BN|-|-|-|-|-|
|BN|-|-|-|-|-|
|DB|-|-|-|-|-|
|DEVOPS|-|-|-|-|-|


ERD[KoreaJobDb]
---
![20240425155554](https://github.com/jungwoogyun/EM-01-PROJECTS/assets/84259104/8631169d-3c85-4be4-a097-613bf1e5b7e0)


FILE TREES[JSP/SERVLET]
--- 
```
C:.
│  .classpath
│  .gitignore
│  .project
│  정리.txt
│
├─.settings
│      .jsdtscope
│      org.eclipse.core.resources.prefs
│      org.eclipse.jdt.core.prefs
│      org.eclipse.wst.common.component
│      org.eclipse.wst.common.project.facet.core.xml
│      org.eclipse.wst.jsdt.ui.superType.container
│      org.eclipse.wst.jsdt.ui.superType.name
│
└─src
    └─main
        ├─java
        │  └─com
        │      └─example
        │          └─app
        │              ├─controller
        │              │  │  FrontController.java
        │              │  │  HomeController.java
        │              │  │  SubController.java
        │              │  │
        │              │  └─user
        │              │      │  UserLoginController.java
        │              │      │  UserLogoutController.java
        │              │      │  UserAddController.java
        │              │      │  UserReadController.java
        │              │      │  UserUpdateController.java
        │              │      │  UserDeleteController.java
        │              │
        │              ├─domain
        │              │  ├─common
        │              │  │  ├─dao
        │              │  │  │  ├─common
        │              │  │  │  │  CommonDao.java
        │              │  │  │  │  ConnectionPool_ByHikari.java
        │              │  │  │  │  ConnectionPool.java
        │              │  │  │  
        │              │  │  │   
        │              │  │  │    MovieDao.java
        │              │  │  │    MovieDaoImpl.java
        │              │  │  │    SessionDao.java
        │              │  │  │    SessionDaoImpl.java
        │              │  │  │    UserDao.java
        │              │  │  │    UserDaoImpl.java
        │              │  │  │  
        │              │  │  │
        │              │  │  ├─dto
        │              │  │  │      Criteria.java
        │              │  │  │      MovieDto.java
        │              │  │  │      PageDto.java
        │              │  │  │      SessionDto.java
        │              │  │  │      UserDto.java
        │              │  │  │
        │              │  │  └─service
        │              │  │          MovieService.java
        │              │  │          MopvieServiceImpl.java
        │              │  │          UserService.java
        │              │  │          UserServiceImpl.java
        │              │  │
        │              │
        │              ├─filter
        │              │      RememberMeFilter.java
        │              │      UTF_8_EncodingFilter.java
        │              │
        │              └─type
        │                      ROLE.java
        │
        └─webapp
            ├─META-INF
            │      context.xml
            │      MANIFEST.MF
            │
            ├─resources
            │  └─static
            │      │
            │      ├─css
            │      │  │  common.css
            │      │  │
            │      │  └─member
            │      │          add.css
            │      │          login.css
            │      │
            │      ├─js
            │      │  │  common.js
            │      │  │  index.js
            │      │  
            │      │
            │      └─jsp
            │              footer.jsp
            │              link.jsp
            │              nav.jsp
            │              topHeader.jsp
            │
            └─WEB-INF
                │  web.xml
                │
                ├─lib
                │      commons-logging-1.3.1.jar
                │      HikariCP-5.1.0.jar
                │      jstl-1.2.jar
                │      logback-classic-1.5.3.jar
                │      mysql-connector-j-8.3.0.jar
                │      slf4j-api-2.0.12.jar
                │      spring-security-crypto-3.2.10.RELEASE.jar
                │
                └─view
                    │  index.jsp
                    │  login.jsp
                    │  template.jsp
                    │  template_aside.jsp
                    │
                    ├─movie
                    │      add.jsp
                    │      delete.jsp
                    │      list.jsp
                    │      update.jsp
                    │
                    │
                    └─user
                            join.jsp
                            login.jsp
```
