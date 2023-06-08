## 마크업 설명

### 로그인 폼
```
 <form action="/" method="post">

  - action : 폼을 전송할 서버쪽 스크립트 파일을 지정
  - method : 폼을 서버에 전송할 방법 지정 (GET 방식은 데이터가 외부에 노출되어 보안이 취약하기 때문에 개인정보나 보안을 해야 하는 경우에는 POST 방식을 씀)

 <fieldset>
          <legend>로그인 폼</legend>

  - fieldset : 로그인 폼 요소를 그룹으로 묶기 위해 사용
  - legend : fieldset의 제목을 달아주기 위해 사용
    => 사용자의 접근성을 높여줌

  <label class="loginForm__Label" for="id">아이디</label>
  <input class="loginForm__Input" id="id">

  - input 태그는 주로 label 태그는 함께 사용
  - label for="" 와 input id="" 는 태그가 연결되어 label의 "아이디" 부분을 클릭했을 때 input의 입력 영역으로 이동
    => 사용자의 접근성 고려

  <input class="loginForm__Input" id="id" type="text" name="userName" required="" placeholder="eudi@eudi.net">

  - type="text" : 기본값으로 텍스트를 입력
  - name="userName" : 폼 전송시 서버로 데이터 이름을 전송하기 위해 사용
  - required="" : 아이디를 필수적으로 입력하도록 지정
  - placeholder="eudi@eudi.net" : 입력칸에 사용자가 올바른 값을 입력할 수 있도록 도와주는 역할
  - type="password" : 패스워드를 입력받을 수 있도록 입력값이 화면에 노출되지 않도록 하는 역할

  <button class="loginForm__Button" type="submit">로그인</button>

  - type="submit" : 폼에서 입력 받은 데이터들을 서버로 전송하는 역할
```

### 회원가입, 비밀번호
```
  <div class="member__Box">
    <a href="/"><i class="bx bx-chevron-right"></i>회원가입</a>
    <a href="/"><i class="bx bx-chevron-right"></i>아이디 비밀번호 찾기</a>
  </div>

- 회원가입, 비밀번호는 클릭시 해당 페이지로 이동 해야 하기 때문에 a 태그를 사용
- i 태그를 사용해서 아이콘 출력
```

  ## CSS 설명

  ### 로그인 폼
  ```
  <h3>로그인</h3>

  - 처음 위치를 기준으로 top: -15px 이동

  <fieldset>

  - position : relative 를 주어  top: -18px; right: 2px 이동

  <div class="login__Container">

  - login__Box 밑 그림자 효과를 주기 위해 div 태그로 만들었고 login__Box 에 position : relative 속성,login__Container 에는 position : absolute 속성을 주어 login__Box 를 top: -6px/ right: 5px; 만큼 이동

  loginForm__Label

  - display: inline-block 속성을 사용하여 크기를 지정하면서 같은 라인에 label과 input이 위치하도록 함

  loginForm__Button

  - loginForm__Group을 position : relative 로 둔 뒤 absolute를 이용하여 오른쪽 끝인 top: 0/ right: 0 위치에 고정
```

  ### 회원가입, 비밀번호
  ```
  login__Box a:first-child, login__Box a:last-child

  - member__Box 에 position: relative 를 지정한 뒤 position: absolute를 사용하여 위치를 조정
```