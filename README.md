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
