
#### `parsing error: unexpected token, expected "]"` <br>
📑 .eslint.js에 **`parser: 'babel-parser',`** 추가!

<br>

**`.eslint.js`**
```
module.exports = {
  root: true,
  extends: '@react-native',
  parser: 'babel-parser',
};

```

<br>

**🚨 에러 원인** <br>

ESLint의 기본 parser는 Espree로, 기본적으로 ECMA 버전이 5로 설정되어있기 때문에 <br>
그 이후 문법이나 Typescript 문법은 parse하면서 에러가 뜰 수 있음! <br>
위 코드를 작성해 parser를 babel parser로 설정해주면 최신 ECMA 버전을 사용할 수가 있어짐

<br>

