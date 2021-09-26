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
    -   POST
    -   PUT
    -   DELETE
-   async, await
    -   async : function() 함수 앞에 키워드 추가(await 키워드가 비동기 코드를 호출 할 수 있게 해주는 함수)
    -   추가가 되고 나면 Promise 를 반환하게 한다.
    -   await : 웹 API 를 포함하여 Promise 를 반환하는 함수를 호출 할 때 사용
-   Promise 로 axios 사용해 보기
-   axios 환경 설정
