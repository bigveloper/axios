<h1>axios</h1>

1. axios 란?

-   Browser, Node.js 를 위한 promise API 를 활용하는 HTTP 비동기 통신 라이브러리
-   백엔드와 프론트엔드 간의 통신을 쉽게 하기 위해 ajax 와 더불어 사용한다.  
    (결국, 비동기 통신을 위해 사용하는 라이브러리)

2. axios 특징

-   운영 환경에 따라 Browser의 XMLHttpRequest(https://developer.mozilla.org/ko/docs/Web/API/XMLHttpRequest) 객체 또는 Node.js 의 http api 를 사용한다.
-   Promise(ES6) API 사용
-   요청과 응답 데이터의 변형
-   HTTP 요청 취소
-   HTTP 요청과 응답을 JSON 형태로 자동 변경
    -   JSON 은 Key : Value 형태로 이루어 져 있다.

3. axios 사용법

-   axios 다운로드  
    `npm install axios`
-   HTTP Methods  
    https://developer.mozilla.org/ko/docs/Web/HTTP/Methods
    -   클라이언트가 웹서버에게 사용자 요청의 목적과 종류를 알리는 수단.
-   axios Methods
    -   GET : 입력한 url에 존재하는 자원에 요청을 한다.  
        `axios.get(url,[,config])`
        -   GET 은 서버에서 어떤 데이터를 가져와서 보여준다거나 하는 용도
        -   GET 은 값이나 상태를 변경할 수 없다. (get, set 을 생각해보자.)
    -   POST : 새로운 resource 를 create 할 때 사용 한다.
        ```
        axios.post(url,{
            data Object
            },[,config])
        ```
        -   두번째 인자 data object 는 본문으로 보낼 data 이다.
        -   예를들어 로그인 이나 회원가입 등 사용자가 생성한 파일을 서버에 업로드 할 때 사용한다.
        -   object 로 되어 있다는걸 생각해 보면 알 수 있다.
        -   주소창에 url 뒤에 내용이 남지 않아 GET 보다는 안전하다.
    -   PUT : REST 기반 API 프로그램에서 데이터베이스에 저장되어 있는 내용을 갱신하는 목적으로 사용 된다.
        `axios.put(url[, data[, config]])`
        -   PUT 은 HTML form 태그에서 기본적으로 지원하는 HTTP Method 가 아니다.
        -   `PUT Method 는 서버에 있는 데이터베이스의 내용을 변경하는 것을 주 목적으로 한다.`
    -   DELETE
-   async, await
    -   async : function() 함수 앞에 키워드 추가(await 키워드가 비동기 코드를 호출 할 수 있게 해주는 함수)
    -   추가가 되고 나면 Promise 를 반환하게 한다.
    -   await : 웹 API 를 포함하여 Promise 를 반환하는 함수를 호출 할 때 사용
-   Promise 로 axios 사용해 보기
-   axios 환경 설정
