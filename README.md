해당 프로젝트
--------
#### The Movie Database Api를 사용한 웹입니다.
기능 :
상영작, 개봉예정작, 명작, 장르별, 키워드별, 검색

+ #### mvoie_app
    * ###### [무비앱 참고코드](https://github.com/seonyoung1/movies)
    * ###### [무한 로딩](https://velog.io/@killi8n/Dnote-6-1.-React-무한-스크롤링-기능-구현.-79jmep7xes)
    * ###### [리액트 라우터](https://velopert.com/3275)
    * ###### [리덕스](https://velog.io/@velopert/Redux-3-리덕스를-리액트와-함께-사용하기-nvjltahf5e)
    * ###### [scss 연결](https://velog.io/@jungsw586/React-%EA%B0%9C%EB%B0%9C%ED%99%98%EA%B2%BD-%EC%84%B8%ED%8C%85%ED%95%98%EA%B8%B0-3.-Sass-%EC%84%A4%EC%B9%98)
    * ###### [style props로 주기](https://stackoverflow.com/questions/39195687/setting-a-backgroundimage-with-react-inline-styles)
    * ###### [useMemo, useCallBack 을 사용해야할 때](https://rinae.dev/posts/review-when-to-usememo-and-usecallback)
    * ###### [react on wordpress 1~5 chapter](https://www.youtube.com/watch?reload=9&v=m2uoYzUlBsg&list=PLD8nQCAhR3tTzWA8K5XQQps4u5kMFJjIG)
    * ###### [워드프레스 REST API](https://developer.wordpress.org/rest-api/reference/post-revisions/#create-a-post-revision)
    * ###### [package.json에서 script의 역할(create-react-app의 react-scripts package 살펴보기) ](https://velog.io/@rlaqltmxm/create-react-app-%EC%82%B4%ED%8E%B4%EB%B3%B4%EA%B8%B0)
    * ###### [wordpress jwt Auth plugin(react)](https://www.npmjs.com/package/wordpress-jwt-auth)
    * ###### [wordpress jwt Auth plugin(wordpress git)](https://github.com/Tmeister/wp-api-jwt-auth)
    * ###### [How to: Make JWT-authenticated requests to the Wordpress API](https://wordpress.stackexchange.com/questions/299542/how-to-make-jwt-authenticated-requests-to-the-wordpress-api)
    * ###### [Using the WordPress REST API with JWT Authentication](https://firxworx.com/blog/wordpress/using-the-wordpress-rest-api-with-jwt-authentication/)


  
PPT 폴더는 js 및 React의 기본 문법을 정리한 것입니다.

[웹 구경하기](https://cocky-montalcini-1434be.netlify.com)

코드 실행 방법 : 
1. Node.js 및 git 다운로드
2. 폴더 생성 및 해당 폴더로 cmd 창(또는 git bash)
3. git init
4. git config 등의 설정
5. git remote add [git url]
6. git pull [remote name] [branch name]
7. npm install -g yarn
8. yarn 
9. yarn start
10. 서버 종료를 원할 시 ctrl + c

+ 에러
    - There might be a problem with the project dependency tree. It is likely not a bug in Create React App, but something you need to fix locally.
        * 해결법은 C:\Users\doje1( 사용중인 사용자 )에 node module을 삭제하면 됨
    - index.js:1406 Warning: Cannot update a component from inside the function body of a different component.
        * react의 자체 버전 에러인듯 함. 이전 버전을 쓰라고함
        
+ 추후 변경사항
    - useMemo, useCallBack으로 최적화 해보기.   
    - ~~스크롤 이벤트를 history라는 파일을 만들어서 제어해보기 (참고 코드 보면서) & withModeChange 파일도 없애기~~
        * history 폴더를 만들어서 해봤는데 큰 merit 없음, 지금과 같이 각 container 에서 redux를 불러야함
        * 참고 코드 와의 차별점으로 withModeChange 놔두는게 좋다고 판단함   
    - ListContainer 에 코드를 줄이는 방향으로 수정해보기
    - jwt 보안 문제점 해결 
    
    
워드프레스 jwt 인증 플러그인으로 받은 값을 워드프레서의 REST API로 요청을 보낼 떄 해더의 값으로 넘기면 되는 것으로 추정
<br>
=> 확인을 위해 <br> 
   + 해더의 값만 넣을 경우
   + 토큰도 값이 보낼 경우
   + 토큰 값이 이상한 경우