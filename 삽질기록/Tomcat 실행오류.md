# Tomcat 실행오류

* 에러 발생
> ``java.net.BindException : Address already in use : bind``

* 에러 원인
> tomcat 기동 시, address 중복으로 발생한 오류(즉, 이미 사용중)

* 해결방법
1. cmd 실행
2. netstat -ano 명령어 입력 > process 정보 확인
3. :port에 8080이라고 되어 있는 부분의 PID 찾기
4. taskkill /f /pid 프로세스 ID 명령어 실행<br/>
ex) ``taskkill /f /pid 412``
