# Master_React16

## reference urls
- 강의: [React 16 마스터하기](https://academy.nomadcoders.co/courses/enrolled/303208)
- 저장소: [nomadcoders/master-react16](https://github.com/nomadcoders/master-react16)

## 설정
### 저장소(github)

- 원격저장소 생성: [Master_React16](https://github.com/hopelife/Master_React16)

- 원격저장소 복제(로컬저장소 생성)
```
/Volumes/data/dev/SynologyDrive/training/lecture/nomadcoders$clone https://github.com/hopelife/Master_React16.git
```

- .gitignore 설정
```
# Yarn integrity file
.yarn-integrity

# dotenv environment variable file
.environment
dist

# git
.git

# node
node_modules

# OSX
.DS_Store
.AppleDouble
.LSOverride
```

## 강의 내용

### #1 Introduction and Project Setup
#### 참조
- [nomad](https://github.com/nomadcoders/master-react16/tree/9d8b152b1f61339be3d1756553d7546bc2ecbe46)
- [hopelife]()
- [강의 영상(nomadcorders)](https://academy.nomadcoders.co/courses/303208/lectures/4676466)
- [강의 영상(youtube)](https://www.youtube.com/watch?v=sM2p1EqTlw4&list=PL7jH19IHhOLOFTVD4R8FeZWkwpVi8-9Fv)

#### 개요
- 자바스크립트 기반 UI 라이브러리
- composition: 요소별, 컴포넌트별 작업 용이
- Unidirectional(단방향) 데이터 플로우: 데이터 변경 -> UI 변경

#### 내용

리액트 세계 입문을 환영한다.
리액트, 왜 쿨하고, 왜 전세계가 열광하는지 설명해볼께!
첫번째, 이건 다 자바스크립트 기반이기 때문이야.
별도로 다른 프레임워크를 배울 필요가 없어. 그냥 자바스크립트 활용하면 됨.
angular, vue js 처럼 다른 언어를 배울 필요도 없어.
리액트는 그냥 자바스크립트만 겁내 잘하면 됨. 그러니까 멋진 자바스크립트 개발자가 되는거지. 동시에!
예를 들면, 이게 리액트 모습인데.
내가 레스토랑 리스트를 보여주고 싶다. 그냥 map쓰면 되는거야. 자바스크립트 인것이지.
그리고 약간의 html 정도?
리액트로 하는 거의 모든 것은 자바스크립트 기반이야.
function, object, variable, ... 정도?
리액트를 배우면 다른 곳에선 필요 없는 기술을 배울 필요가 없어.
예를 들면, 너가 Angular를 배웠다고하자,
그리고 너가 Angular를 안쓰잖아? 그러면 해당 기술을 다른 곳에 쓸 수가 없어.
정말 빙구되는거지. 별도의 프레임워크를 배워서, 별도의 언어를 배우고.. 블라블라. 근데 안쓰면? 말짱 도루묵!
리액트는? 자바스크립트야! 새로운 것 배울 필요가 없어! 게다가 너를 더 뛰어난 자바스크립트 개발자로 만들어줄꺼야.
리액트를 하면서 동시에 자바스크립트 기술을 향상시키는 것이지.
슈퍼 퍼킹 쿨 인것이지.
두번째, composition, 구조가 겁내 쿨해
리액트 구조는 요소별, 컴포넌트별로 나눠서 작업할 수있게 되어있어.
먼말이냐? 일단 한번 보여줄께.
자 왼쪽에 있는건 우리가 보통 볼수있는 인스타그램 웹사이트야.
이걸 자세히 뜯어보면, nav, header, numbers, grid 요소들을 볼 수 있지.
얘네들을 우리가 요소(components)라고 하잖어? 리액트는 이렇게 요소별로 나눠서 볼수있어.
슈퍼 쿨해! 그룹별로 쪼개서, 작업할 수 있기 때문이야.
이런 구조(composition)가 멋진 것이지.
모든 걸 작은 요소(components)로 쪼개서 작업, 마무리하면 가져다가 다른 곳에 쓸 수 있으니까 말이야!
예를 들면, 내비게이션을 보자.
리액트로는 이렇게 생겼어.
자바스크립트 function, 약간의 jsx...
JSX가 뭐냐면, 리액트로 html 을 쓰는 방법이야. 복잡한거 절대아니고. 겁내 심플해.
걍 html에 살짝 뭐 붙여주면 되는 것임.
그다음 헤더를 살펴보자.
똑같지? function 쓰고, 블라블라...
이래서 내가 리액트를 좋아함. 컴포넌트별로 쓰고, 다른 곳에도 갖다 붙일 수 있고,
세번째, 리액트는 Unidirectional (단방향) 데이터플로우를 가지고 있어. 이게 먼말이냐.
데이터는 항상 일정한 장소에 위치해있고, 그 장소에서만 변경할 수 있어.
Angular의 경우, 데이터는 view 이나 model 으로 변해.
리액트의 경우, 데이터는 위치한 장소에 있고,
상태가 변했을 경우, 데이터는 그대로 있고, UI가 업데이트 되는 것임.
즉, 데이터가 UI를 변경시키는 것이지.
UI는 절대로 데이터를 변경시키지 않아.
즉, 단방향인것이야. 쌍방향 이런 것이 아니라. 데이터 -> UI로.
다시 한번, 데이터가 변하면 UI가 업데이트 됨.
데이터가 안변하면, UI도 안변하겠지?
데이터가 변하면, UI는 새로운 데이터와 함께 업데이트 되는 거야.
즉, UI에서 데이터를 바꿀 수는 없어.
항상 같은 방향이야. 데이터-> 데이터 변경 -> UI 변경
UI에서 데이터 변경은 있을 수 없어.
바로 이 3가지가 내가 그리고 세계가 리액트에 열광하는 이유인 것이지.
또다른 이유를 추가하자면,
커뮤니티가 정말 방대하고 커. 거대한 라이브러리, 오픈소스, 질문과 답... 최강이야!
하나 더! 리액트는 프레임워크가 아니라 UI 라이브러리야.
리액트는 angular, ruby .....
앗 죄송. angular랑은 쓸 수 없고, 파이썬이랑 쓸 수 있고.
(절대 angular랑은 쓸수없고) 루비랑 쓸 수 있고,
리액트는 view 이기 때문에 섞어서 쓸 수 있어.
model, view, controller에서 리액트는 view 이기 때문에, 나머지는 원하는대로 골라서 쓸 수 있지.
난 리액트를 장고, 루비온레일즈, nodejs랑 섞어서 쓰고 있어.
여기까지야! 다음 강의에서 보자고! (유튜브 구독은 사랑입니다!)

##### 

##### 
