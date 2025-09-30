# 백엔드 정규 스터디 1주차 과제

## 1. 1주차에 학습한 내용

1. 웹
- 웹 : 인터넷 위에서 동작하는 서비스로 사용자들이 서로의 정보를 공유
- 클라이언트 : 서버에 요청을 보내고, 응답 결과를 사용
- 서버 : 클라이언트의 요청을 처리하고, 응답을 반환
- URL : 웹 상에서 특정 자원의 위치를 나타내는 주소
- URL의 구조 : Host, Port, Path, Query, Scheme

2. HTTP
- HTTP : 웹에서 데이터를 주고받는 서버-클라이언트 모델의 프로토콜
- HTTP의 특징 : 무상태성, 비연결성
- 주요 메서드 : GET - 조회, POST - 등록, PUT - 교체, PATCH - 수정, DELETE - 삭제
- 상태 코드 : 200 성공, 201 성공 후 생성, 400 클라이언트 요청 오류, 404 리소스 없음, 500 서버 내부 오류

3. 프론트엔드와 백엔드
- 프론트엔드 : 사용자가 직접 보고 상호작용하는 화면, 사용자 인터페이스를 개발
- 백엔드 : 사용자의 요청을 받아 실제 동작을 처리하고 데이터를 저장 및 관리
- 데이터베이스 : 데이터를 체계적으로 모아둔 저장소

4. API와 REST API
- API : 한 프로그램이 다른 프로그램의 기능이나 데이터를 사용할 수 있도록 미리 정해놓은 약속이자 소통 창구
- REST : 자원 - URL, 행위 - 메서드, 표현 - JSON

5. Spring Boot
- Spring : Java 애플리케이션 개발에 사용되는 오픈소스 애플리케이션 프레임워크
- 프레임워크 : 애플리케이션 개발을 쉽고 효율적으로 할 수 있도록 필요한 기본 구조와 공통 기능을 제공하는 뼈대
- Spring Boot : 스프링 프레임워크를 아주 빠르고 쉽게 사용할 수 있게 해주는 도구

## 2. Whitelabel Error Page 스크린샷

![[screenshot.png]]

## 3. 온라인 쇼핑몰 프로젝트 API 명세서 작성

상품 기능
- 상품 정보 등록
	- POST
	- /products
- 상품 목록 조회
	- GET
	- /products
- 개별 상품 정보 상세 조회
	- GET
	- /products/{productsId}
- 상품 정보 수정
	- PATCH
	- /products/{productsId}
- 상품 삭제
	- DELETE
	- /products/{productsId}

주문 기능
- 주문 정보 생성
	- POST
	- /order
- 주문 목록 조회
	- GET
	- /order
- 개별 주문 정보 상세 조회
	- GET
	- /order/{productsId}
- 주문 취소
	- DELETE
	- /order/{productsId}
