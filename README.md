# React에 대한 공부한 내용을 기록하는 저장소 입니다.

## React CDN 

### 개발용으로 적합하며 배포용 버전에는 적합하지 않습니다.
```js
<script crossorigin src="https://unpkg.com/react@17/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"></script>
```

### React의 용량 및 성능 최적화된 배포용 버전은 아래와 같이 제공되고 있습니다.
```js
<script crossorigin src="https://unpkg.com/react@17/umd/react.production.min.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@17/umd/react-dom.production.min.js"></script>
```

<hr>

## JSX 다루기

JSX란? 
문자도 HTML도 아닌 JavaScript의 확장 문법입니다.

```js
    const element = <h1>hello,world</h1>
```

### Babel
Babel은 compiler로,특정 언어를 다른 프로그래밍 언어로 옮기는 프로그램입니다.
Babel을 쓰는 이유는 JSX를 JavaScript도 알아들을 수 있도록 바꿔주기 위해서입니다.

### install
```js
Use it via UNPKG: 
  https://unpkg.com/@babel/standalone/babel.min.js. 
This is a simple way to embed it on a webpage without having to do any other setup.

Install via NPM: 
  npm install --save @babel/standalone
```

JavaScript가 읽을 수 있도록
```js
    <script type="text/babel"></script> //이렇게 작성을 해주셔야 됩니다.
```

JSX의 장점은 모든 것을 변수화 할 수 있다는 것 입니다.

### Spread 연산자

```
    ...props 
```
만약 변수가 객체로 할당을 했을 경우 스프레드 연산자를 이용해서 사용을 할 수 있습니다.

<hr>

## 멀티 Element 생성하기

Fragment 를 이용해서 Reac.Fragment Or <></> 빈 태그를 사용할 수 있습니다.

```js
    const element = {
        <React.Fragment>
            <h1>1</h1>
            <h3>3</h3>
            <h5>5</h5>
        </React.Fragment>
    }

    const element ={
        <>
            <h1>1</h1>
            <h3>3</h3>
            <h5>5</h5>
        </>
    }
```