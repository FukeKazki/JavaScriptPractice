## JavaScript特有の書き方
### アロー関数
関数を簡略化して記述<br>
thisの束縛をしたいとき<br>
```js
(引数) => {処理内容}
//定義
const calcSum = (a, b, c) => {
    return a + b + c;
};
//呼び出し
calcSum(1, 2, 3);
```
