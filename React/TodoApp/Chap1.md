# Todoアプリの作成
## 導入
Reactの一番はじめの作品として簡単なタスク管理アプリを作成します.  
エンジニア界隈ではよくTodoアプリと呼ばれており, フロントエンド技術者が初めてのフレームワークや言語を触る際, よく作成するアプリです.  
なぜTodアプリを作成するのか.  
それは, CRUD(クラッド)というソフトウェアの基本機能を全て持つアプリだからです. 以下の表にその説明を示します.  

| 名前 | 操作 |
|----|----|----|
| Create | 生成 |
| Read | 読み取り |
| Update | 更新 |
| Delete | 削除 |  

これらの機能からTodoアプリはチュートリアルに最適と考えられています.  
それでは実際に作成していきましょう.  

## 開発環境
以下のバージョンで開発を行います.  
予め以下のコマンドが使用できることを確認してください.  
- **node** v12.8.0
- **yarn** v1.21.0
- **create-react-app** v3.3.0

## 雛形の作成
任意のディレクトリで以下のコマンドを実行してください.
```zsh
$ create-react-app todo-app
$ cd todo-app
$ yarn start
```
うまくいくとサーバが立ち上がりブラウザに表示されます.  

## コードの編集
todo-appフォルダ内の構成は以下のようになっています.
```
.
├── README.md
├── package.json
├── public
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
├── src
│   ├── App.css
│   ├── App.js
│   ├── App.test.js
│   ├── index.css
│   ├── index.js
│   ├── logo.svg
│   ├── serviceWorker.js
│   └── setupTests.js
└── yarn.lock
```  
主となるファイルは src 内に存在しており
index.jsでApp.jsを呼び出して public/index.html に表示しています.  
App.jsを編集していくことでTodoアプリを作成していきます.  

App.jsを以下のように変更してみてください.
ブラウザの表示が変わると思います.  
このようにreactにはホットリロードという機能がありコードが変更されセーブされると自動的に表示を更新してくれます.  

```js:app.js
import React from 'react';
import './App.css';

function App() {
  return (
    <div className="App">
      <header className="App-header">
        <p>Hello Tommy</p>
      </header>
    </div>
  );
}

export default App;
```

## コードの説明
