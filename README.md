# React×TS×MUI プロジェクトのテンプレ

プロジェクト作成手順を以下にまとめる。

クローンせず以下手順での作成を推奨。

## １：React × TS アプリの作成

`npx create-react-app 【project-name】 --template typescript`

『参考』
https://typescript-jp.gitbook.io/deep-dive/browser


## ２：MUIのインストール

`yarn add @mui/material @emotion/react @emotion/styled`


`yarn add @mui/icons-material`

『参考』
https://mui.com/getting-started/installation/


## ３：MUIスタイルシートの読み込み

public/index.htmlに以下２行を追加
    
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap"/>
    <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons"/>
    
『参考』
https://mui.com/getting-started/installation/


## ４：テスト

src/App.tsx

以下インポート文を追加

`import Button from '@mui/material/Button';`

App関数return内に以下を追記

`<Button variant="contained">Hello World</Button>`

ボタンが表示されていればOK！
