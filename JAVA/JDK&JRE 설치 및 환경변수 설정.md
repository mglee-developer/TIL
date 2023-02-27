# JDK와 JRE
- JDK란?
  - Java Development Kit의 약자, 자바로 개발하는데 사용된다.
- JRE란?
  - Java Runtime Environment의 약자, 자바로 만들어진 프로그램을 실행시키는데 사용된다.

# 설치방법
- 링크 : [JDK&JRE](https://www.oracle.com/java/technologies/downloads/archive/ "JAVA")
- JAVA SE 8(8u202 and earlier) 설치
  ```
  JAVA SE 8(8u211 and later) 버전 부터는 
  6개월 이후 보안 업데이트가 이루어지지 않아
  무료로 업데이트를 지원하는 버전을 사용한다.
  ```

# 환경변수 설정(윈도우)
- 설정 위치 : 홈 - 시스템 - 정보 - 고급시스템 설정
- 고급탭 > 환경변수
  ```
  사용자변수 : 로그인한 하나의 계정에만 권한 부여
  시스템변수 : 시스템에 권한 부여, 모든 사용자 사용 가능
  ```
- 시스템변수 추가
  - JAVA_HOME : C:\Program Files\Java\jdk1.8.0_202
  - JRE_HOME : C:\Program Files\Java\jre1.8.0_202
    - 톰캣 사용을 위해 등록
  - CLASSPATH : %JAVA_HOME%lib
  - Path 편집 : 실행 파일이 해당 위치에 없으면 Path 경로에서 찾아 실행
    - %JAVA_HOME%bin
    - %JRE_HOME%bin
- 실행확인
  - cmd
    ```cmd
    ## 자바 인터프리터, 자바프로그램(.class) 실행
    java -version
    ## 자바 컴파일러, 소스파일(.java)을 jvm이 인식하는 바이트코드(.class)타입으로 변환
    javac -version
    ```
