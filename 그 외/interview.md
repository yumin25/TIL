- [REST API](#rest-api)
- [MSA](#msa)
- [JWT](#jwt-json-web-token)
- [git flow](#git-flow)
- [Spring](#spring)
- [Spring Security](#spring-security)
- [QueryDSL](#querydsl)
- [ORM](#orm-object-relation-mapping)

<br>

### REST API

Representational state transfer API의 약자. <br>
자원을 HTTP URI로 표기하고 HTTP 프로토콜을 통해 요청 및 응답을 정의하는 아키텍처. <br>

- 리소스 (resource, URI)
- 메소드 (HTTP Method)
  - GET : 자원 조회
  - POST : 자원 생성
  - PUT : 자원 전체 교체
  - DELETE : 자원 삭제
  - ( PATCH : 자원 일부 교체 )
- 메세지 (message)

특징

- Stateless (무상태성) : 상태정보를 저장하고 관리하지 않는다.
- Uniform : 특정 언어나 기술에 종속되지 않고 모든 플랫폼에서 사용 가능하다.
- Cacheable
- self-descriptiveness
- client - server 구조
- 계층형 구조

<br>

### git flow

master 브랜치가 코드의 직접적인 배포와 핵심이 되고, develop 브랜치에서 개발하는 코드들을 기능에 따라 feature 브랜치를 분기시켜 기능을 추가, 제거한다.
feature들이 merge된 develop브랜치를 release 브랜치에 빼고 배포 버전을 명시한 뒤 master, dev 브랜치에 병합하며 배포한다.
버그로 안한 긴급 수정이 필요할 때는 master 코드에서 직접적으로 hotfix 브랜치를 분기해 버그를 수정한 뒤 master에 병합한다.

<br>

### MSA

하나의 기능을 하는 서비스 단위로 쪼갠 구조. <br>
장점 : 서비스별 독립적 배포가 가능하다.<br>
단점 : 서비스가 모두 분산되어 있어 상대적으로 복잡하다.

- SOP : 모듈의 의존성을 줄이되 내부에서 최대한 공유

<br>

### JWT (Json Web Token)

인증에 필요한 정보들을 Token에 담아 암호화시켜 사용하는 토큰.

구성 요소 (.으로 구분)

- Header
- Payload
- signature

<br>

- HS512 : HMAC <sup>[1](#hmac--암호화-해시-함수와-기밀-암호화-키를-수반하는-메세지-인증-코드)</sup> using SHA-512<sup>[2](#sha-512--암호-해시-함수-512비트의-해시-값-생성)</sup>. 대칭키 암호화 알고리즘.

<br>

### 세션

서버의 메모리, 데이터베이스 등의 자원을 사용하여 사용자의 정보를 유지시킨다.

<br>

### MVC

- model
- view
- contoller

<br>

### Spring

자바 기반의 웹 개발 프레임워크이다.
장점 : 편리한 MVC 구조, WAS에 종속적이지 않은 개발 환경, 트랜잭션 관리 용이

- AOP : 관점 지향 프로그래밍. 공통 관심사를 모아 모듈화하여 중복 코드를 줄임.
- DI : 의존성 주입. 객체를 외부에서 생성한 후 주입시켜주는 방식.
- IOC : 제어의 역행. 인스턴스 생성부터 소멸까티 컨테이너가 관리.

요청 - dispatcher servlet - handler mapping. 요청을 처리할 수 있는 컨트롤러 찾기 - 컨트롤러에서 요청 처리, 응답받을 view의 이름 리턴 - view resolver 검사 후 view로 보냄 - view에서 처리 - dispatcher servlet - 결과 응답
[참고](https://blackaaron.tistory.com/3)

**Spring과 Spring Boot의 차이점** : 스프링부트는 스프링 프레임워크를 사용하기 위한 설정의 많은 부분을 자동화한다. 컴포넌트 스캔, bean 설정, dispatcher servlet 설정, view resolver, JDBC 설정, 웹 jar 설정 등. 또한 내장 서블릿 컨테이너인 tomcat이 자동 설정.

<br>

### Spring Security

보안(인증, 권한, 인가 등)을 담당하는 스프링 하위 프레임워크.

- bcrypt : 단방향 해쉬 함수

<br>

### JAVA vs PYTHON

같은 점 : 객체지향 언어.

**JAVA** <br>
정적타이핑 언어 <br>
코드를 미리 컴파일한 뒤 byte code를 배포 - 속도가 비교적 빠르다
<br>

**PYTHON** <br>
동적타이핑 언어(변수 유형을 선언할 필요 x) <br>
인터프리터 언어. 라인 별로 컴파일을 한다. 실행될 때마다 코드를 컴파일한다. <br>
코드 가독성이 비교적 좋다.
<br><br>

### ORM (Object Relation Mapping)

객체와 관계형 데이터베이스의 데이터를 자동으로 매핑해주는 것

### JPQL

직접 쿼리문을 작성하여 객체를 조회
@Query("쿼리문")

### QueryDSL

문자가 아닌 코드로 쿼리 작성
동적인 쿼리 작성이 편리하며 코드의 재사용성이 증가한다.
정적 타입(Q 클래스)를 기반으로 쿼리 작성.

### JPA Specification

JPA가 제공하는 Criteria로 이루어지는데 조금만 복잡해져도 사용하기 어려워진다.

### Criteria

JPQL을 자바 코드로 작성하도록 도와주는 빌더 클래스 API

#### HMAC : 암호화 해시 함수와 기밀 암호화 키를 수반하는 메세지 인증 코드

#### SHA-512 : 암호 해시 함수. 512비트의 해시 값 생성.
