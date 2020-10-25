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


---------------------------------------------------------

## 정리노트

### CSS
- rgba 에서 a(alpha)는 투명도를 의미한다.
- div에 width를 주지 않으면 div안 내용만큼 크기가 주어진다.
- input에 padding을 주면 입력 시작지점 조절 가능하다.
- navgation bar 해결을 위한 간단 방법: body에 padding을 주자.

:octocat: flexbox
- flex: (flex-grow) (flex-shrink) (flex-basis) 세가지 설정가능
- align-item  flexbox안의 item들을 수직으로 정렬 (start,center,end) default는 다 0



### javascript
- ary, ary1를 객체라 가정 할 때 ary.push(ary1)와 ary.concat(ary1) 
push()의 return 값은 배열의길이, concat()의 return 값은 합친 배열이다.

### React
- setState()는 비동기로 작동한다. :point_up:
