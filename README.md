# JWT 템플릿 구현

- [JWT 사이트](https://jwt.io/)
- 참고 : [인프런 jwt 튜토리얼](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8-jwt/dashboard)

## 목표
- JWT 이해 및 숙련도 향상
- SPA 에서 session 보다 jwt 가 더 많이 사용되는지 이해하기
- 다음 사이드 프로젝트에서도 보완해서 사용할만한 템플릿 구현

## 환경설정
- Java 11
- SpringBoot 2.7.10
- SpringSecurity
- Spring Data JPA
- H2 Database

## JWT란

### 장점
- 중앙의 인증서버, 데이터스토어에 대한 의존성 없음, 시스템 수평확장 유리
- Base64 url safe encoding => url, cookie, header 모두 사용가능

### 단점
- Payload의 정보가 많아지면 네트워크 사용량 증가, 데이터 설계 고려
- 토큰이 클라이언트에 저장, 서버에서는 클라이언트의 토큰을 조작할 수 없음
