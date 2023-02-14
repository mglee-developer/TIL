# Web Server
* 개념
  * client로부터 http 요청을 받아 정적인 컨텐츠(.html, .jpeg, .css) 제공
* 기능
  * http 프로토콜을 기반으로 client의 요청을 서비스하는 기능
  * 기능1
    * 정적인 컨텐츠 제공
    * was 거치지 않고 바로 자원 제공
  * 기능2
    * 동적 컨텐츠 제공을 위한 요청 전달
    * client의 요청을 was에 보내고 was가 처리한 결과를 client에게 전달(응답)
* 예
  * Apache Server, Nginx, IIS(Windows 전용 Web 서버)
* 필요한 이유❓ <br>
정적인 컨텐츠만 처리하도록 기능을 분배하여 서버 부담을 줄여줌

# Was Server
* 개념
  * DB 조회나 로직 처리를 요구하는 동적인 컨텐츠를 제공
  * HTTP 통해 컴퓨터나 장치에 애플리케이션 수행해주는 미들웨어
  * **웹컨테이너(Web Container)** 혹은 **서블릿 컨테이너(Servlet Container)**
    ```
    Container란 jsp, servlet을 실행시키는 소프트웨어
    was는 jsp, servlet 구동환경 제공
    ```
* 역할
  * WAS = Web Server + Web Container
  * Web 기능들을 구조적으로 분리하여 처리하고자하는 목적 (DB서버와 같이 수행)
* 기능
  * 프로그램 실행환경과 DB 접속 기능 제공
  * 여러개 트랜잭션 관리 기능
  * 비즈니스 로직 수행
* 예
  * Tomcat, JBoss, Jeus, Web Sphere    
* 필요한 이유❓ <br>
데이터를 DB에서 가져와 비즈니스 로직에 맞게 결과를 만들어서 제공하여 자원을 효율적으로 사용
