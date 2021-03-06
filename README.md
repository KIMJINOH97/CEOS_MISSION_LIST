# CEOS_MISSION_LIST
## :star: 미션 정리

### 1. 바닐라 JS로 todo-list
- html, css, javascript

### 2. React를 사용한 messenger(채팅화면)
- React hooks, styled-components

:runner: [react-chatting](https://react-messenger-12th-ten.vercel.app/)

### 3. 위 미션을 이용한 messenger만들기 (kakao, instagram등)
- React-routing

:seedling: [react-routing](https://react-router-inky.vercel.app/)
 
 ### 4. Get 방식으로 서버와 통신하기 (axios 활용)
 - Axios
 
 ### 5. Post 방식을 이용한 JWT 로그인 인증 (axios 활용)
 - Axios, querystring
 - `'content-type': 'application/x-www-form-urlencoded'`으로 하기 위해 querystring을 썼다.
 
---------------------------------------------------------

## 미션들을 수행하며 느낀점:droplet:

### todo-list
>클론 코딩만 한 나로써 혼자 코드를 짜는게 생각보다 시간이 많이걸리고 훨씬 힘들었다. 
미리 구조를 생각하지 않고 코드를 짜게되어 코드를 많이 고치게 됐다.
변수의 이름의 일관성이 없어 알아보기 힘들었으므로 간단한 변수도 그 역할을 생각하며 네이밍을 해야겠다.
JS에서는 lowercamelcase로 일관성 있게 한다.
CSS에서 중요한 요소인 flex에 대해 좀 명확히 알고 가야 할 것같다.

### react-messenger
>무엇보다 css가 가장 힘들었다. 기억해야 될 것들을 메모장에 적어가며 구현했다.
flexbox가 각각 어떻게 움직이는지 하면서 늘었다. react역시 클론코딩으로 배웠지만 
직접 해보는 것이 와 닿는것이 빠르고, 다음에도 할 수 있을 것 같은 자신감이 든다.
각 Component에서 props 전달 하는 것을 유동적으로 할 수 있게 됐다.
각자 코드를 공유 함으로써 피드백을 주고받으며 리팩토링 하는 과정에서 진짜 실력이 느는것 같다.


### messenger
> 여전히 변수 네이밍 시 어떤 역할을 하는 건지 정하기가 어려웠다. 간단하게 하면 다른 내용과 겹쳐
도중에 다른것을 바꿔야 할 때도 있었다. **user와 message의 내용들을 따로 파일을 두어 보관**하는 것
이 전 코드의 재사용에 있어 어떻게 활용하면 좋을지 생각 했던 것들이 앞으로 도움 될 것같다.
routing의 개념을 정확히 모르고 next라는 프레임워크를 얹어 썼지만 이제는 왜 쓰는지 조금이나마
알 수 있다. 코드량이 생각보다 많아져 각각의 Component로 잘게 쪼개어 파일 보관을 했다.
한결 익숙해진 css지만 아직 시간이 많이 걸렸다.


### async, await, axios(get)
> async()를 이용해 비동기로 서버와 통신하는 방법을 이용했다. url을 이용해 서버에서 받아온 데이터들을
map()함수를 활용해 뿌려보았다. async await을 이용하니 .then() 으로 이어가는 방식보다 훨씬 간편했을 뿐
아니라 코드량이 많이 줄어 편했다. 만약 서버로부터 통신이 많아질 경우 어떤식으로 코드를 나누고, 폴더를 구조화
할 지 한 번 생각해 보는 계기가 됐다. useEffect()함수의 작동방식을 정확히 알아보기 위해 사이트를 참고했다.
api의 정의가 정확히 뭔지도 알아보았으면 좋겠다.

:thumbsup: [React UseEffect](https://sgwanlee.medium.com/useeffect%EC%9D%98-dependency-array-ebd15f35403a)

### axios(post), jwt 토큰 인증
> axios의 post 방식을 통해 회원가입, 로그인을 front 단에서 주고 받아보았다. 로그인 정보가 일치하면 서버에서 
front로 token을 보내주고, 그 토큰을 header에 default값으로 넣어, 그 뒤 서버와 통신 할 수 있다.
서버 쪽에서 jwt를 이용해 코드를 짜 보았지만, front에서 한 건 처음이다. 이를 통해 front, back에서 
jwt를 이용해 어떻게 서로 정보를 주고 받는 지 알 수 있는 계기가 됐다. 로그인, 회원가입을 한 뒤, redirection을 위해
`history.push` 를 활용 해 보았는데, 이 과정이 더 궁금해 알아 보는게 좋을 것 같다.

---------------------------------------------------------

## 정리노트

### CSS 및 html
- rgba 에서 a(alpha)는 투명도를 의미한다.
- div에 width를 주지 않으면 div안 내용만큼 크기가 주어진다.
- input에 padding을 주면 입력 시작지점 조절 가능하다.
- navgation bar 해결을 위한 간단 방법: body에 padding을 주자.
- cursor(마우스 커서) : default값은 그냥 마우스 모양 <pointer 손모양>
- div[div                   ] 이런식으로 둘 때 박스 width를 100%하면 된다.
- span은 하위테그로 div, p 를 쓸 수 없으며 p는 div를 포함 할 수 없다.
- opacity를 사용해 투명도를 조절함.
- font-weight는 100단위로 인식한다 (반올림 한다 생각)
- position: fixed 사용시 화면이 겹칠 수 있음
- ```-webkit-user-select: none ```는 크롬에서 마우스 클릭 방지가 가능하다.



:octocat: flexbox
- flex: (flex-grow) (flex-shrink) (flex-basis) 세가지 설정가능
- align-item  flexbox안의 item들을 **수직(세로)** 으로 정렬 (start,center,end) default는 다 0
- justify-content 는 flexbox안의 내용(item)들을 **수평(가로)** 기준으로 정렬

:lollipop: styled component
- 원하는 component에 :hover과 같은 것을 쓰고 싶을 때 &:hover{}을 쓰면 가능하다. (& 는 자기자신을 가리킴)



### javascript

- let A = ''; 선언 했을 때 A의 값은 **undefined**이다.
- **lowCamelCase**로 변수명을 정한다. 함수는 **동사형**으로 써주는것이 좋다.

:whale2: 배열
- ```array.push(ary1)```와 ```ary.concat(ary1)``` 에서 **push()의 return 값은 배열의길이, concat()의 return 값은 합친 배열**이다.
- ```array.slice() ```를 통해 배열을 원하는 조건으로 자를 수 있다. ex) ary.slice(1) 맨 앞 정보 자름.
- ```array.map(v,index) ```를 통해 배열 안의 정보 ex) [{a}, {b}] 에서 {a} {b} 를 뿌린다?.
- ```array.filter((x) -=> {return x.length>2}``` 이런식으로 조건을 넣어줘 원하는 정보만 가질 수 있다.
- ```array.indexOf(x) ``` array에서 특정값 x가 있는지 판단한다.(틀리면 =-1) array가 **string**이 되어도 된다. (포함하는 index > 0반환)


### React
- setState()는 비동기로 작동한다. :point_up:
- ```onClick={onClick()}``` 틀린표현 onClick()으 반환값이 들어감 ```onClick={onClick}```이 맞는 표현
- inline으로 style을 넣을 때 ```style = {{backgroundColor : 'black'}}``` 이런식으로 넣어준다. (-기준 lowCamelCase)
- img 태그에서 src를 js로 넣을 때 같은 경로의 파일인 경우```src={./pengsu.png}``` 이런식으로 가능하지만 다른 폴더안의 img일 경우 ```src={require('../public/pengsu.png')}``` require로 감싸주어야한다.

:aerial_tramway: react-router
- Link 테그와 Route 테그는 Router테그 안에 있게한다. 즉 최상위는 ```<Router> </Router>```
- 중복 라우터를 허용하지 않기 위해서는 exact를 사용해 준다. ex) ```<Route exact path='/'> ```


:question: useEffect

:herb: history

react-router-dom에서 사용할 수 있다.  
위의 npm을 설치하게 되면 페이지의 기록들을 저장할 수 있게 된다.  
마치 stack처럼 경로가 저장된다고 보면 편하다.  

`push('경로', [states])` 함수 [states]는 생략 가능하다. 해당 경로를 스택에 넣고 이동한다.  
`goBack()` 함수 뒤로가기와 비슷하다.   
`goForward()` 함수 앞으로가기와 비슷하다.  


:hatched_chick: axios

**Get**
URL을 통해 서버와 통신을 주고 받는다. axios.get 시, parameter로 인자를 넘겨주게 되면 `URL/ .... prameter....` 이런식으로 서버에 전송된다.

```
// 1번째 방식
axios({
 method: 'get',
 url: 'URL',
 params: { },
 headers: { },
 data: { },
}

// 2번째 방식
axios.get("URL", { params: {  객체  } }, { headers: ' 헤더 정보 ' } );
``` 
params로 굳이 넣지 않고 URL뒤 바로 넣을 수 있다.

**Post**
해당 URL로 data에 객체를 넣어 서버와 통신을 한다.

```
// 1번째 방식
axios({
 method: 'post',
 url: 'URL',
 params: { },
 headers: { },
 data: { },
}

// 2번째 방식
axios.post("URL", {  객체  }, { headers: ' 헤더 정보 ' } );
// 순서 잘 지키기
``` 
* 헤더 값에 토큰 고정시키기: axios.defaults.headers.common['Authorization'] = AUTH_TOKEN;
* 헤더에 content-type default값 두기: axios.defaults.headers.post['Content-Type'] = 'application/x-www-form-urlencoded';
* baseURL 설정하기: axios.defaults.baseURL = 'https://api.example.com';

