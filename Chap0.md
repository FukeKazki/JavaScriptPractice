# 基本的な構文
### htmlに組み込むとき
```html
<!doctype html>
<html lang='ja'>
<head>
    <meta charset='utf-8'>
    <title>タイトル</title>
</head>
<body>
    <script>
    //ここにJavaScriptを書く
    </script>
    <!-- 外部ファイルにするときは -->
    <script src='path'></script>
</body>
</html>
```
### ログで確認する
```js
console.log('Hello World');
```
### GoogleChrome デベロッパーツールの表示
```
MAC: command + option + i
```
### 四則演算
| 構文 | 意味 | 
| --- | --- | 
| + | 数値の加算を行う |
| - | 数値の減算を行う |
| * | 数値の乗算を行う |
| / | 数値の除算を行う |
| % | 除算の余りを求める |
| ** | 数値のべき乗を計算する |

```js
console.log(100 + 200); //300
console.log(200 - 80); //120
console.log(100 * 3); //300
console.log(400 / 5); //80
console.log(402 % 5); //2
console.log(2 ** 3); //8
```

### 変数を使う
```js
let 変数名 = 値;

let a = 100;
let b = 200;
let c = a + b;
console.log(c);
```

### 定数を使う
```js
const 定数名 = 値;
```
