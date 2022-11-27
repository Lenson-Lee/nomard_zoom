#nomard_zoom

노마드 코더와 함께한 줌 클론코딩

babel : 자바스크립트 컴파일러(비교적 최신 문법으로 작성된 코드를 이전의 JS문법으로 변환)
nodemon : 코드를 실행해 주는 런타임
express : Node.js 환경에서 API 서버를 개발할 때 사용 할 수 있는 웹 프레임워크
ws : 웹소켓 규칙에 맞게 구현한 핵심 기능을 제공하는 패키지

- 뷰 엔진
  HTML을 이용해 페이지를 만드는 것보다 편하게 데이터를 전송하고 표현. 여기서는 pug를 사용

-HTTP와 비교하는 웹소켓
HTTP의 가장 큰 특징인 stateless: 사용자와 서버가 요청/응답을 주고받은 이후는 서버에 사용자가 남지 않아 서버는 다음 요청을 기다리기만 함. 사용자가 의도적으로 정보를 포함해서 요청하면 남긴 함. stateless 때문에 HTTP에서는 실시간 기능 구현이 어려움.
웹소켓은 서로 악수하듯 사용자와 서버를 연결함. 서버는 사용자가 누군지 알고, 서버가 사용자에게 메시지 보내기도 가능. 실시간 기능 구현이 훨 쉽다는 뜻.

- server.js에서 이미 express를 이용해 서버를 만들고 있지만 HTTP 기반 동작이기 때문에 ws와 프로토콜이 서로 다르다. 그래서 express 서버에 ws패키지 기능을 합치는 방식으로 서버를 완성할 예정.
