# 공유주소

### github

https://github.com/edu-ministori/addinedu_10_js

### codesandbox

https://codesandbox.io/s/crazy-violet-v777c?file=/README.md

# Javascript

## JS Introduction

https://www.w3schools.com/js/js_intro.asp

- Javascript는 웹페이지 개발을 목적으로 하는 언어
- Front End 개발 영역에서는 `HTML, CSS를 제어하고, 효과(애니메이션)를 적용하는 기능 구현에 사용`

## JS 작성방식

- External, Internal, Inline 방식
- HTML 파일에서 Javscript 코드를 적용하는 script Element의 위치
  - HTML 파일이 모두 로딩(렌더링)이 된 이후에 Javascript가 적용
    (HTML Element보다 아래쪽에 위치)
  - head 태그 쪽 상단에 script를 분리해서 위치시키기 위한 방식
    - Internal 방식(javascript 코드를 직접 작성하는 방식)으로는 적용 불가능 ex) <script>...<script>
    - External 방식 : script 태그에 defer attribute를 사용
      - 상단에 위치하더라도 defer attribute를 사용하면, HTML Element가 모두 로딩된 이후에 javascript 코드를 실행

## Javascript 언어를 공부하는 방법(순서)

> 언어적 관점
>
> - 프로그래밍 언어 문법
> - 일반적 알고리즘
>
> 활용적 관점
>
> - 활용 목적 : 웹 개발, 소프트웨어 개발, 게임 개발 / 사용 소프트웨어의 목적

```
Ex)

웹 FrontEnd 개발 : Javascript
1) 언어적 관점 : Javascript 문법
2) 활용적 관점 : 브라우저, HTML, CSS 연관 관계 => 서비스 개발

게임 개발 => 유니티/언리얼엔진 게임엔진 소프트웨어 => C#/C++
1) 언어적 관점 : C#/C++ 문법
2) 활용적 관점 : 게임엔진 소프트웨어에 적용, 게임프로그래밍 최적화

```

## Javascript(ECMAScript) Version

- ES5
- ES6

## ES6에서 추가된 내용

- 변수 개념 확장
- class 개념 추가
- 함수 사용 방식 확장
- 프레임워크, 라이브러리(ReactJS, NodeJS)에 사용됨

## Javascript

### 문법

- 변수 / 데이터 / 연산자
- 명령문(구문)
- 함수
- 배열/객체/class
- 추가문법

### Javascript 활용

- 이벤트
- HTML, CSS 와의 관계(제어)

## Javascript 문법

### JS variables

https://www.w3schools.com/js/js_variables.asp

> 변수
>
> - 변하는 수
> - 수(값:데이터)가 저장되는 공간

```
변수정의(선언)키워드(예약어) 변수이름= 초기값;

var a = 10;
```

> var
>
> - 변수 선언
> - 변수 값 변경 가능

```
Naming 표기법
- 동일한 이름 여러번 사용될 수 없음
- 여러단어를 사용해서 네이밍을 할 때 단어와 단어를 구분 : 가독성

snake case : car_person_name - File/Folder
kebab case : car-person-name - HTML/ id, class
camel case : carPersonName - javascript 변수, 함수
pascal case : CarPersonName - javascript Class
```

### JS Let, Const

https://www.w3schools.com/js/js_let.asp
https://www.w3schools.com/js/js_const.asp

- ES6에서 추가된 변수 선언 키워드

```
let a = 0;

const b = 'a';
```

> let
>
> - 변수 선언
> - 초기화 변수 값 변경 가능

> const(constant)
>
> - 변수 선언
> - 초기화 변수 값 변경 불가능
> - 복잡한 데이터를 간단한 변수 이름으로 대체사용하기 위한 경우

### JS Data type

https://www.w3schools.com/js/js_datatypes.asp

- 숫자, 문자, 객체

> 숫자
>
> - 숫자 데이터 : 정수, 실수

> 문자
>
> - 문자 데이터 : 문자(character), 문자열(string)

> boolean(논리데이터)
>
> - 참(true), 거짓(false) 두 가지 결과 값을 가지고 있는 타입

> 배열
>
> - 데이터 여러개가 나열된 집합

> 객체
>
> - 데이터 집합

> Javascript 데이터 타입을 구분하지 않음
>
> - 변수 선언시 구분하지 않음
> - 데이터 상세 타입을 구분하지 않음

- js

```
var a = 1; // var - 값을 변경할 수 있는 변수 선언
let b = 1.5; // let - 값을 변경할 수 있는 변수 선언
let c = 'hello';
```

- java

```
int a = 1; // int - 정수형태의 값을 변경할 수 있는 변수 선언
short b = 1; // short - 2byte 크기의 정수형태의 값을 변경할 수 있는 변수 선언
float b = 1.1; // float - 실수형태의 값을 변경할 수 있는 변수 선언
String d = "hello" // String - 문자열 형태의 값을 변경할 수 있는 변수 선언
```

### JS operator(연산자)

> 할당 연산자

```
=
```

> 산술 연산자

```
+, *, /, -, %
% : 나머지 계산
Ex) 5 % 3 = 2

+ 연산자 활용
5 + 5 =  10
5 + 'a' = '5a' (연결연산)
```

> 비교 연산자
>
> - 결과값 : boolean(t/f)

```
== : 같다(크기)
=== : 같다(크기, 타입)
!= : 같지않다(크기)
!== : 같지않다(크기, 타입)
> : 크다
< : 작다
>= : 크거나 같다
<= : 작거나 같다
```

> 논리 연산자
>
> - 결과값 : boolean(t/f)

```
&& : AND
|| : OR ( | -> pipe)
! : NOT

a > 5 && a < 10 : a는 5보다 크고 10보다 작다
a < 5 || a > 10 : a는 5보다 작거나 10보다 크다
!(a < 5) : a가 5보다 작지 않다
```

> 산술 연산 + 할당 연산

```
a += 1 => a = a + 1
=> 변수 += 값 : 값만큼 일정한 증가 연산

a = a + 1;
a += 1;
a++; (증가연산)

a = a - 1;
a -= 1;
a--; (감소연산)

a++,a-- => 증감연산자
```

> 명령문(구문) : 프로그래밍 실행 흐름의 변화를 줄 수 있음
>
> - 분기문
> - 반복문

### JS Condition

https://www.w3schools.com/js/js_if_else.asp

> if : 조건문 / 분기문
>
> - 식의 결과값이 참이면 실행문 실행,

```
if(condition){
  실행문
}

condition : 결과값이 boolean 데이터인 식

if(a>10){} : a>10 => true/false

if(a+1){} : a+1 => 음수, 0, 양수 : 0(false) / 정수(true)

if(a){} : a => true / false or 0 / 정수

if(true){}

if(condition1) {
  실행문1
}else if(condition2){
  실행문2
}else{
  실행문3
}

else if : 필요시 사용, 여러번 반복 사용 가능
else : 필요시 사용, 마지막에 한번 사용 가능

```

### JS switch

https://www.w3schools.com/js/js_switch.asp

> switch : 분기문

```
switch(expresstion) {
  case 결과값1:
    실행문1;
    break;
  case 결과값2:
    실행문2;
    break;
  default:
    실행문3;
}

expresstion : 표현식, 결과값이 일반 데이터(숫자, 문자, 불리언)
```

### for loop (반복문)

https://www.w3schools.com/js/js_loop_for.asp

- for 반복문 : 반복 횟수를 정해서 반복 실행

```
for(statement1; statement2; statement3){

}

statement1 :  for 반복문 실행전 최소 1번 실행 구문
statement2 :  코드블럭을 실행하기 위한 조건식 구문
statement3 : 코드 블럭 실행 후 반복 실행되는 구문
=> 3개의 statement는 반복횟수를 결정하는데 연관되는 구문

for (let i = 0; i<3; i++){
  console.log('반복실행');
}

0) let i = 0 구문실행 => i = 0

1) i<3 비교식 실행 => true
2) 코드블럭 실행(1)
3) i++ 실행 => i = 1

1') i<3 => true
2') 코드블럭 실행(2)
3') i++ => i=2

1'') i<3 => true
2'') 코드블럭 실행(3)
3'') i++ => i = 3

1''') i<3 => false
반복 실행 종료

```

### break/ continue

- break

  - 루프 구문 바깥으로 빠져나가는 키워드(구문)

- continue
  - 해당 회차 실행을 건너뛰는 키워드(구문)

### while

- condition 이 true 일때만 반복실행하는 구문

```
while(condition){
  실행문
}
```

```
while 사용 예 : 로그인

** while(true){} => 무한루프
whlie(true){

  //로그인 시도
  if( 입력한 아이디 === 저장된 db 아이디 && 입력한 비밀번호 === 저장된 db 비밀번호){
    //로그인성공
    break;
  }
}
```

### JS function

https://www.w3schools.com/js/js_functions.asp

> 함수
>
> - 여러 실행 코드들을 하나로 묶어주는 역할
> - 특정 기능을 할 수 있는 코드 블럭 단위로 패키징
> - 특정 기능을 재사용하기 위해서 함수를 사용

> - 매개변수
>   - 함수에 넣어주는 재료
>   - 함수에 여러가지 매개변수를 넣어줌으로써 다양한 결과를 얻을 수 있음

> - return(반환값)
>   - 함수에서 처리된 결과 값
>   - 함수를 호출한 쪽으로 결과값을 되돌려줌

```
1. 함수선언
function 함수이름([매개변수]){
  // 실행 코드 블럭
  [리턴값]
}


2. 함수호출(실행)
함수이름();

** []: 생략가능
```

```
함수 선언 형식
function 함수이름(){
  // 코드블럭
}

let(const) 변수이름(함수이름) = function(){
  // 코드블럭
}

익명함수
function(){
  // 코드블럭
}

- 함수이름을 변수처럼 사용하는 경우
- 함수이름 필요없이 바로 실행하는 경우
```

### JS Array(배열)

https://www.w3schools.com/js/js_arrays.asp

- 개수가 많은 데이터를 대표되는 하나의 변수 이름으로 저장할 때 사용하는 데이터 타입

- 배열도 객체데이터

```
배열 선언
const cars = ['volvo','bmw','saab'];

// const 키워드를 사용해서 배열 선언시
// 배열 데이터의 원소는 변경, 추가, 삭제 가능
// 다른 배열 데이터로 변경은 불가능

ex) cars['hyundai', 'chevrolet', 'kia'] (X)
    cars[0] = 'hyundai' (O)

cars[0] => 'volvo'
cars[1] => 'bmw'
cars[2] => 'saab'

배열 접근(access)/ 변경 / 추가 / 삭제

변경
cars[0] = 'hyundai';

추가
cars.push('kia'); => 마지막 위치에 원소 추가

삭제
cars.pop(); => 마지막 원소 삭제

```

### JS Object

https://www.w3schools.com/js/js_objects.asp

- 데이터들을 어떤 대상에 가깝게 다루고자 할 때
- 객체데이터는 property, method
- 각각의 객체데이터는 name:value로 구성됨(key:value)
- 객체 메소드에 사용되는 this는 해당 객체를 의미함
- 객체 메소드에서 객체 프로퍼티를 사용할 땐 this를 사용해서 객체를 명시해야 함

```
객체 선언

const car = {
  type : 'Flat',
  model : '500',
  color : 'white',
  fullName : function(){
    return this.type + this.model
  }
}

객체 접근(access) / 추가 / 변경 / 삭제

console.log(car.type);

변경
car.type = 'kia';

추가
car.weight = '850kg';

삭제
delete car.model;
```

### JS Class(클래스)

https://www.w3schools.com/js/js_classes.asp

> Class
>
> - 객체 데이터를 생성하기 위한 설계도
> - 클래스를 사용해서 만든 객체 데이터 : Instance(인스턴스)
> - 클래스 이름은 대문자로 시작
> - this : 해당 클래스 객체를 의미

```
클래스 선언

class Car{
  constructor(name, year){ // 생성자 함수 => property 생성
    this.name = name; // this.name : 객체 property 이름 name
    this.year = year; // this.year : 객체 property 이름 year
  }

  printYear(){
    return this.year;
  }
}

let car1 = new Car('hyundai', 2021);
let car2 = new Car('Kia', 2022);

car1.name;
car1.printYear();

car2.year;
car2.printYear();
```

### JS scope

https://www.w3schools.com/js/js_scope.asp

> 변수 적용(접근) 범위
>
> - Block Scope : 블럭 범위 - 명령문/구문의 코드 블럭 영역
> - Function Scope : 함수 범위 - 함수 선언 영역
> - Global Scope : 전역 범위 - 프로그래밍 전체 영역

> 변수 Scope 적용 원리
>
> - 전역 영역, 함수 영역, 블럭 영역이 포함 관계로 되어 있을 때 적용가능
> - 포함하고 있는 큰 영역에서 선언된 변수는 포함되는 작은 영역에서는 사용 가능
> - 포함되는 작은 영역에서는 선언된 변수는 포함하는 큰 영역에서는 사용 불가능
> - 포함 관계로 되어 있지 않은 서로 다른 영역에서는 접근 불가능

### JS Arrow Function

https://www.w3schools.com/js/js_arrow_function.asp

```
let hello = function() {
  return 'Hello World';
}

let hello = () => {
  return 'Hello World';
}
```

> function으로 정의되는 일반함수와 화살표 함수는 this의 의미가 다름
>
> - 일반 함수는 최종적으로 함수를 호출한 대상의 객체 : this
> - 화살표 함수는 함수가 포함된 최상위 객체 : this

### JS JSON

https://www.w3schools.com/js/js_json.asp

### 내장객체

- javascript 언어 속에 미리 정의되어 있는 객체
- String, Array, Date, Math ...
- 내장객체의 property와 method를 사용해서 기능 실행

## Javascript 활용

### Event(이벤트)

https://www.w3schools.com/js/js_events.asp

- 사용자의 행동에 의해서 발생되는 변화의 신호
- 마우스, 키보드, 터치 관련 이벤트
- 이벤트 동작 흐름

  - 변화 발생
  - 변화와 관련된 이벤트(신호) 발생
  - 발생된 이벤트를 감지해서 상황에 맞는 기능/동작 실행

- 발생되는 이벤트 종류
- 이벤트 감지 함수
- 기능/동작 실행

> 이벤트 종류
>
> - 마우스 : click, mouse move, mouse over
> - 키보드 : key down(press), change

> 이벤트 감지 함수
>
> - addEventListener

```
사용방식
객체(DOM).addEventListener(이벤트 종류, 함수)
```

> 실행 함수
>
> - 함수 호출
> - 익명 함수

### HTML DOM(Document Object Model)

- Document(HTML 문서 : body 태그 안 모든 요소)
- HTML Element를 객체화 시킨 것
- DOM 사용해서 javascript가 HTML을 제어
  - DOM 객체에 포함된 property, method를 사용

> HTML Element 내용
>
> - HTML Element를 추가, 출력, 수정, 삭제
> - C(reate) R(ead) U(pdate) D(elete)
>
> HTML Element 효과
>
> - 시각적 효과 : 애니메이션, show/hide

> DOM(Document Object Model) 객체
>
> - document : HTML Element 중에서 가장 최상위 객체

> BOM(Browser Object Model) 객체
>
> - window : 브라우저 관련 최상위 객체

### DOM Access Method

> HTML4 API
>
> - id 이름으로 DOM Access : document.getElementById()
> - class 이름으로 DOM Access : document.getElementsByClassName()
> - tag 이름으로 DOM Access : document.getElementsByTagName()

> HTML5 API
>
> - 1개 DOM Access : document.querySelector('css 선택자 형식')
> - 여러개 DOM Access : document.querySelectorAll('css 선택자 형식')

### DOM Contents - CRUD

> Create(생성)
>
> - DOM 생성 : Javascript에서 HTML Element 동적(Dynamic) 생성
>
>   - HTML 직접 코딩 => 정적 코딩
>   - javascript로 HTML 코딩 => 동적 코딩
>
> - Text Contents 생성 추가 경우
>
>   - 1. HTML Element 동적 생성 => HTML Element 대상에 생성된 Element를 추가
>   - 2. Text 생성
>   - 3. 생성된 Element에 생성된 Text를 추가
>   - 4. HTML 문서에 있는 Element 대상에 생성된 Element를 추가
>
>   - 즉, 태그를 만들고, 콘텐츠를 만들고 태그에 콘텐츠를 넣고, HTML 문서에 특정부분에 만들어준 태그와 콘텐츠를 삽입

```
// Element 생성(1)
let pTag = document.createElement("p");

// Text 생성(2)
let text = document.createTextNode("Created Text Example");

// 생성된 Element에 생성된 Text를 추가(3)
pTag.appendChild(text);

// HTML 문서에 있는 대상에 추가(4)
const parent = document.querySelector(".parent");
parent.appendChild(pTag);
```

> Read

```
// 첫 번째 방법(createTextNode)
let paragraph = document.querySelector("p");
let sen = paragraph.innerHTML + "문장";
let text = document.createTextNode(sen);

const parent = document.querySelector(".parent");
parent.appendChild(text);


// 두 번째 방법(innerHTML)
const parent2 = document.querySelector(".parent2");
parent2.innerHTML = paragraph.innerHTML + "추가된 내용";
```

> Update

```
// innerHTML 사용
const paragraph = document.querySelector(".paragraph");
paragraph.innerHTML = "변경된 단락";
```

> Delete

```
//text만 제거
const para = document.querySelector(".paragraph");
para.innerHTML = "5";

//태그까지 제거(제거할 대상의 부모 요소를 통해서 제거)
const body = document.querySelector("body");
const para2 = document.querySelector(".paragraph2");
body.removeChild(para2);
```

### Form 요소

https://www.w3schools.com/html/html_forms.asp

- 클라이언트에서 작성한 내용을 서버에 전달할 때 사용하는 Element

> input
>
> - type='text'
> - type='button' / type="submit" / type='reset'

> button
>
> - input type button 과 사용 형식이 거의 같음
> - type="button" / type="submit" / type="reset"

```
<input type='button' value="버튼" /> // 일반 텍스트만 버튼 안에 넣을 수 있음
<button type='button'>버튼</button> // 이미지나 애니메이션을 버튼으로 변경할 수 있음

** 기능의 차이는 없음
** 활용도 측면에서 button 태그를 사용하는 것을 권장
```

> select
>
> - 숨겨진 목록에서 아이템 선택
