## View 환경설정

### Welcome Page 만들기
`resource/static/index.html`
```html
<!DOCTYPE HTML>
<html>
<head>
  <title>Hello</title>  
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
</head>
<body>
  Hello
  <a href="/hello">hello</a>
</body>
</html>
```

- spring boot가 제공하는 Welcome Page 기능
  - `static/index.html`을 올려두면 Welcome Page 기능을 제공한다.

### thymeleaf 템플릿 엔진
 - thymeleaf 공식 사이트 : https://www.thymeleaf.org/
 - spring 공식 튜토리얼 : https://spring.io/guides/gs/serving-web-content/
 - spring boot 매뉴얼 : [https://docs.spring.io/spring-boot/docs/2.3.1RELEASE/reference/html/spring-boot-features.html#boot-features-spring-mvc-template-engines](https://docs.spring.io/spring-boot/docs/2.3.1.RELEASE/reference/html/spring-boot-features.html#boot-features)

![image](https://user-images.githubusercontent.com/70195171/223116387-1b239967-e74b-400d-8e91-ad24495902c9.png)
- 컨트롤러에서 리턴 값으로 문자를 반환하면 view resolver가 화면을 찾아서 처리
  - `resource:templates/`+{ViewName}+`.html`
