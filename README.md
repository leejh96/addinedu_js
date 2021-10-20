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

- 변수(데이터) / 연산자
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
```
