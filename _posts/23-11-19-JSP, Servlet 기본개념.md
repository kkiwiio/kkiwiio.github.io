---
published: true
title: "JSP,Servlet 기본개념"
categories: Web
tag: [web,jSP,servlet]
---

전혀 공부하지 않았던 분야인 웹에 대해 공부를 시작하려니 개념부터 헷갈리기 시작 현재 공부하고 있는 웹프로그래밍 과목의 jsp와 servlet의 차이를 좀 알아둬야겠다고 생각했다. 

## Servlet
서블릿(Servlet)은 서버에서 웹페이지 등을 동적으로 생성하거나 데이터 처리를 수행하기 위해 자바로 작성된 프로그램이다. 

서블릿은 Java 코드안에 HTML 코드가 삽입되며, 자바언어로 되어있다.(즉 .java확장자) 
보통은 'doGet' 또는 'doPost' 매서드 안에 작성된다. 
![servlet 작동원리](https://gmlwjd9405.github.io/images/web/servlet-process.png)
출처:https://gmlwjd9405.github.io/2018/10/28/servlet.html
1. 사용자가 웹 페이지 form(HTML Form)을 통해 자신의 정보를 입력한다. (Input)

2. Servlet의 doGet() 또는 doPost() 메서드는 입력한 form data에 맞게 DB 또는 다른 소스에서 관련된 정보를 검색한다.

3. 이 정보를 이용하여 사용자의 요청에 맞는 적절한 동적 컨텐츠(HTML Page)를 만들어서 제공한다. (Output)

## JSP(Java Server Pages)
HTML 코딩을 하기 너무 어렵고 불편해서 반대로 HTML내부에 Java 코드를 삽입하는 방식이다. 
서블릿의 단점을 보안하고자 만든 서블릿 기반의 스크립트 기술
Java 코드를 <% %> 태그로 둘러싸서 표현한다. 