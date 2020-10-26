# CEOS_MISSION_LIST
## :star: 미션 정리

### 1. 바닐라 JS로 todo-list
- html, css, javascript

### 2. React를 사용한 messenger(채팅화면)
- React hooks, styled-components

[react-chatting](https://react-messenger-12th-ten.vercel.app/)

### 3. 위 미션을 이용한 messenger만들기 (kakao, instagram등)
- React-routing

---------------------------------------------------------

## 미션들을 수행하며 느낀점

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
도중에 다른것을 바꿔야 할 때도 있었다. user와 message의 내용들을 따로 파일을 두어 보관하는 것
이 전 코드의 재사용에 있어 어떻게 활용하면 좋을지 생각 했던 것들이 앞으로 도움 될 것같다.
routing의 개념을 정확히 모르고 next라는 프레임워크를 얹어 썼지만 이제는 왜 쓰는지 조금이나마
알 수 있다. 코드량이 생각보다 많아져 각각의 Component로 잘게 쪼개어 파일 보관을 했다.
한결 익숙해진 css지만 아직 시간이 많이 걸렸다.

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


:octocat: flexbox
- flex: (flex-grow) (flex-shrink) (flex-basis) 세가지 설정가능
- align-item  flexbox안의 item들을 **수직(세로)** 으로 정렬 (start,center,end) default는 다 0
- justify-content 는 flexbox안의 내용(item)들을 **수평(가로)** 기준으로 정렬

:lollipop: styled component
- 원하는 component에 :hover과 같은 것을 쓰고 싶을 때 &:hover{}을 쓰면 가능하다. (& 는 자기자신을 가리킴)



### javascript
- ary, ary1를 객체라 가정 할 때 ary.push(ary1)와 ary.concat(ary1) 
push()의 return 값은 배열의길이, concat()의 return 값은 합친 배열이다.
- let A = ''; 선언 했을 때 A의 값은 undefined이다.
- ```array.slice() ```를 통해 배열을 원하는 조건으로 자를 수 있다. ex) ary.slice(1) 맨 앞 정보 자름.
- ```array.map(v,index) ```를 통해 배열 안의 정보 ex) [{a}, {b}] 에서 {a} {b} 를 뿌린다?.
- ```array.filter((x) -=> {return x.length>2}``` 이런식으로 조건을 넣어줘 원하는 정보만 가질 수 있다.


### React
- setState()는 비동기로 작동한다. :point_up:

:aerial_tramway: react-router
- Link 테그와 Route 테그는 Router테그 안에 있게한다. 즉 최상위는 <Router> </Router>
- 중복 라우터를 허용하지 않기 위해서는 exact를 사용해 준다. ex) <Route exact path='/'> 
- 


