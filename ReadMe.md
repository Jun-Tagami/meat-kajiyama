# Beginner's butcher shop
**模擬的な精肉点店のECサイトです**

<br />
牛肉、豚肉、馬肉（そのほかの肉）にジャンルを分けてさらにそれぞれのに食肉について輸入、国産肉とカテゴリーに分けました。<br />

## URL
利用者画面:
https://tag-portfolio-production.herokuapp.com

オーナー管理画面:
https://tag-portfolio-production.herokuapp.com/owners/dashboard

## 使用技術
 ## フロントエンド
  - HTML / CSS
  - JavaScript

 ## バックエンド
  - ruby 2.6.5
  - Ruby on Rails 6.0.3.7（フレームワーク）
  - Rubocop（コード解析ツール）
  - Rspec（テスト）
 ## インフラ
  - MySQL 5.7.22 / Puma 
  - GitHub
  - heroku
  - AWS(S3)
 ## 開発環境
  - VScode

## ER図
<img width="1162" alt="ER図" src="https://user-images.githubusercontent.com/76899874/143732671-54ce314c-c828-42d2-9ed6-b62f36b40858.png">

## 特に工夫・意識した点

### ①Device機能で商品出品者管理画面と商品購入者画面のユーザー管理
商品出品者と商品購入者に対してそれぞれdevice機能を用いてユーザー管理をすることにしました。

### ②3種類の食肉に対して輸入、国産の2種類に分けて商品を表示
輸入、国産の製品の混同を防止するために輸入、国産のカテゴリーを分けて商品購入者にわかりやすく表示することを心がけました。


## Beginner's butcher shopの開発背景
「表品を間違えることなく、シンプルに購入・予約ができるECサイト」を目標に作成しました。<br />

きっかけは知り合いの紹介で「ECサイトを作りたい」という方と知り合い、精肉の通販を行いたいという<br />
お話を聞いたところからそのお手伝いができればと思いこのサイトを作成しようと思いました。<br />

## 【機能一覧 / 詳細】

### 機能一覧まとめ

## 商品予約機能
  - ユーザー基本機能
    - ユーザー新規登録 / ログイン
    - ユーザ-編集 / 退会　<br />
  - 予約機能
    - 数量、配送希望日、配送希望時刻、配送先入力
    - 購入内容確認（カテゴリー、産地、消費期限、保存方法、予約数量）
    - 支払い金額

## 商品出品者機能
  - 商品一覧/商品出品
    - 商品出品機能（画像選択、商品名、商品説明、商品内容量、税込価格、カテゴリー、産地、保存方法、消費期限）
  - 会員一覧
    - 会員一覧機能（ID、会社名、メールアドレス、郵便番号、都道府県、市区町村以下全て、電話番号）  
  - 予約一覧
    - 予約機能（重複予約、過去日付の予約不可、予約時間の制限、利用日数に応じて料金の計算）
  - owner_password編集
    - パスワード編集機能（Email、password、password confirmation,Current password)

## 使用素材
【画像素材】<br />
https://o-dan.net/ja/<br />
https://www.photo-ac.com/<br />
https://pixta.jp/?waad=u1vrgKa0&gclid=Cj0KCQiAnaeNBhCUARIsABEee8XT1WS7_6HOgsjSpmsIvGwYJMhS62cMkKo_FsMCbTNwMdHJV8WZBXUaAu7qEALw_wcB