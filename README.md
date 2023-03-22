# SpringBoot Project
### SpringBoot와 JPA를 활용한 쇼핑몰 웹 애플리케이션 개발

#### 버전 및 라이브러리
- SpringBoot ver 2.7.9
- Java 11
- spring-boot-starter-web 
  - spring-boot-starter-tomcat: 톰캣 (웹서버) 
  - spring-webmvc: 스프링 웹 MVC
- spring-boot-starter-thymeleaf: 타임리프 템플릿 엔진(View) 
- spring-boot-starter-data-jpa
  - spring-boot-starter-aop 
  - spring-boot-starter-jdbc
    - HikariCP 커넥션 풀 (부트 2.0 기본)
  - hibernate + JPA: 하이버네이트 + JPA
  - spring-data-jpa: 스프링 데이터 JPA
- spring-boot-starter(공통): 스프링 부트 + 스프링 코어 + 로깅 
  - spring-boot
    - spring-core 
  - spring-boot-starter-logging
    - logback, slf4j
    
    
### 도메인 분석 설계

#### 요구사항 분석
<img width="479" alt="image" src="https://user-images.githubusercontent.com/108318465/226782626-a1eeba8b-7ac8-4aad-ae67-93b1446d706a.png">

##### 기능목록
- 회원 기능
  - 회원 등록
  - 회원 조회
- 상품 기능
  - 상품 등록
  - 상품 수정
  - 상품 조회
- 주문 기능
  - 상품 주문
  - 주문 내역 조회
  - 주문 취소
- 기타 요구사항
  - 상품은 재고 관리가 필요하다.
  - 상품의 종류는 도서, 음반, 영화가 있다.
  - 상품을 카테고리로 구분할 수 있다.
  - 상품 주문시 배송 정보를 입력할 수 있다.
  

#### 도메인 모델과 테이블 설계
<img width="513" alt="image" src="https://user-images.githubusercontent.com/108318465/226783024-e1bcbae1-5538-4482-ae8d-e44134213598.png">

#### 회원 엔티티 분석
<img width="513" alt="image" src="https://user-images.githubusercontent.com/108318465/226783043-f438ee61-fe57-4814-b405-254bea341f95.png">

#### 회원 테이블 분석
<img width="506" alt="image" src="https://user-images.githubusercontent.com/108318465/226783079-bc1b9b90-55f2-4dfd-a004-d9f546efd678.png">


