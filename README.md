# [Spring Boot 기초](https://www.youtube.com/playlist?list=PLogzC_RPf25E-mfrKvl6jWHU8r1jxCZgq)
### [J101. Spring Boot 개발 환경 만들기]
#### - JAVA8 설치  
#### - MAVEN 설치
#### - STS 설치
#### - STS MAVEN 설정  
# <hr>

### [J102. Spring Boot 빌드하고 WEB 띄우기]
#### - Spring Boot 프로젝트 만들기
#### - 컨트롤러 만들기
#### - Html 만들기
#### - 포트 변경하기
#### - STS 에서 웹 기동 -> intelJ 로 변경
#### - 빌드 이후 명령어로 웹 서버 기동
# <hr>

### [J103. Docker 로 MYSQL, ORACLE 테스트 DB 구성]
#### - Docker MYSQL Container 설치와 사용자 만들기 
#### - STS DBeaver Plug-in 설치와 MYSQL 접속해서 확인하기
#### - Docker ORACLE Container 설치와 사용자 만들기  
#### - ORACLE 접속해서 확인하기
# <hr>

### [J104_1. Spring Boot JPA 기본 CRUD]
#### - Spring Boot 프로젝트 만들기 
#### - DB 연결 정보 만들기
#### - JPA DB 만들기
#### - JUnit DB CRUD
# <hr>

### [J104_2. Spring Boot JPA DEPT-EMP]
#### - EMP 만들기
#### - DEPT 수정하기 
#### - 테이블 구조 확인
#### - JUnit DEPT, EMP CRUD 
# <hr>

### [J104_3. Spring Boot JPA 검색과 페이징 처리]
#### - Repository Method 만들기
#### - 부서명 검색
#### - 부서명 오름차순 검색
#### - 부서명 검색 결과 개수
#### - 부서명 검색 페이징을 위한 데이터 입력
#### - 부서명 검색 페이징 처리
# <hr>

### [J105. Spring Boot UI Thymeleaf Layout]
#### - 단일 화면
#### - 단일 데이터 / 복수 데이터 표현
#### - Layout 적용하기
# <hr>

### [J106_1. Spring Boot Security]
#### - Spring Boot Project 만들기
#### - Security 기본 
#### - Security Customizing
#### - Security Customizing Test
#### - 사용자 정보 화면에 나오게 하기
#### - 권한별로 화면 보여주기
#### - 세션에서 사용자 정보 보기
# <hr>

### [J106_2. Spring Boot Security + REDIS]
#### - Spring Boot Project 빌드
#### - 포트 8080 기동 후 로그인
#### - 포트 8081 기동 후 로그인 세션 공유 안 됨 확인 
#### - REDIS Docker 설치  
#### - Spring Boot REDIS 설정
#### - Spring Boot Project 빌드
#### - 포트 8080 기동 후 로그인
#### - 포트 8081 기동 후 로그인 세션 공유 확인
# <hr>

### [J106_3. Spring Boot Security + Security + JWT]
#### - pom.xml 라이브러리 추가
#### - Token 사용 상수 정의
#### - JwtService 정의
#### - UserDetailServiceImple 수정
#### - JwtHandlerInterceptor 구현
#### - SecurityConfig 수정
#### - 리턴 값에 사용하는 ResultDTO 생성
#### - ApiController 정의
# <hr>

### [J107. Spring Boot SSL 인증서 무료로 적용하기]
#### - Spring Boot Project 생성
#### - https://www.sslforfree.com/ 도메인으로 인증서 요청
#### - 도메인 인증을 위한 인증파일 다운로드
#### - 서버에 인증파일 업로드 후 웹에서 인증하고 인증서 다운로드 
#### - OpenSSL 설치
#### - OpenSSL 이용하여 인증서 변환  
#### - application.yml 인증서 등록 
#### - 서버에서 빌드 이후 접속 후에 https 확인
<pre><code>
openssl pkcs12 -export -in certificate.crt -inkey private.key -out springcloud.pfx

openssl pkcs12 -in springcloud.pfx -clcerts -nokeys -out springcloud.crt

keytool -import -alias springcloud -file springcloud.crt -keystore trust.jks
</code></pre>
# <hr>