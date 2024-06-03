# 조성은 백엔드 개발 과제

### 사용기술

- Java 17
- SpringBoot
- Docker
- Spring Security
- Spring Batch
- Jwt
- MySQL
- Redis
- JPA


### API 명세

- 유저 (http/Auth.http, http/User.http)
  - 회원가입
    - POST /auth/signup
  - 로그인
    - POST /auth/login
  - 정보
    - GET /user
    

- 찜 서랍 (http/LikeStore.http)
  - 생성
    - POST /like/store
  - 삭제
    - DELETE /like/store/{id}
  - 목록
    - GET /like/store  


- 찜 (http/ProductLike.http)
  - 생성
    - POST /product/like
  - 삭제
    - DELETE /product/like/{id}
  - 목록
    - GET /product/like/{id}


### 실행방법

1. Docker Desktop 실행합니다.
2. AblyApiApplication 을 실행합니다.


### 최종 구현된 범위

제시된 요구 사항 모두 구현했습니다.  
사용자 인증에서 jwt 토큰을 이용했습니다.  
Redis 를 사용하여 찜한 상품 id들을 저장했습니다.  
- 찜한 상품이 내 다른 찜 서랍에 있을경우 찜할 수 없습니다. 


