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

### ③

## Beginner's Campの開発背景
「時間を短縮し、目的に沿ったキャンプ場の選択ができる」ことをテーマに制作することを決めました。<br />

既存のキャンプサイトでは、さまざまな情報が豊富にあるがゆえに、<br />
そこから取捨選択し決めるのは時間が掛かり、結局断念した経験はキャンプに限らず誰もがあると思います。<br />

私もその一人でした。<br />

この課題を解決するため、あらかじめ初心者向けにオススメのキャンプ場を紹介。<br />
オススメだけではなく、ユーザー同士での情報の共有、ランキングがあることで、<br />
多角的に情報を共有でき、時間を短縮させます。<br />
その結果、サイトとユーザーが、より質の高いキャンプ情報を提供できるサービスになればと考えました。<br />

## 【機能一覧 / 詳細】

### 機能一覧まとめ
https://docs.google.com/spreadsheets/d/1OdpAQK21FwGG-HCSthLstctx_0l4XZ8ub2DcF6HWk_Q/edit#gid=0

  - ユーザー基本機能
    - ユーザー新規登録 / ログイン
    - ユーザー一覧、編集、詳細
    - ゲストログイン機能
    - マイページで下記表示可能<br />
（フォロー・フォロワー一覧、投稿一覧、いいねした投稿、予約一覧、ブックマーク一覧）
  - フォロー機能
    - ユーザー同士の「フォロー」機能（非同期通信 / Vue.js axios)
  - 投稿機能（みんなのキャンプ）
    - キャンプ情報投稿一覧、詳細表示、記事投稿、編集、削除機能
    - プレビュー機能
    - いいね機能（非同期通信 / Ajax）
    - コメント機能（非同期通信 / Ajax）
  - タグ付け機能
    - 中間テーブルの概念を学ぶため、gemを未使用
    - カンマで区切り、複数タグ付けができます
    - タグをクリックすると、同じタグの投稿一覧が表示されます
  - ランキング機能
    - みんなのキャンプのいいね数、キャンプ場、キャンプ用品はraty.jsの平均点のTOP3を表示
  ### キャンプ場に関する機能
  - 予約機能
    - DatetimePicker使用（カレンダーで予約日時を選択）
    - 過去の日付を選択できない（カレンダー、手入力も不可）
    - 重複予約できない（チェックイン、アウト日が被ると、エラーメッセージ表示）
    - 予約時間の制限（15～24時まで）
    - 予約日数に応じて利用料金を非同期通信で計算
  - 口コミ機能
    - 口コミ機能投稿、一覧、詳細（raty.js）
    - TOP画面のみ、ユーザーが評価した平均点を表示
（管理者が投稿した住所をgeocoderで緯度経度を読み取り、地図を表示）
  ### キャンプ用品に関する機能
  - 口コミ機能
    - 口コミ機能投稿、一覧、詳細（raty.js）
    - TOP画面のみ、ユーザーが評価した平均点を表示
### 管理者機能
  - ユーザー一覧表示、詳細
  - 予約一覧表示、詳細
  - 投稿機能
    - キャンプ場投稿
    - キャンプ場投稿一覧、詳細、編集、削除
    - 複数画像アップロード（refile）
  - キャンプ用品投稿
    - キャンプ用品投稿一覧、詳細、編集、削除
    - 予約機能（重複予約、過去日付の予約不可、予約時間の制限、利用日数に応じて料金の計算）

## 使用素材
【画像素材】<br />
https://o-dan.net/ja/<br />
https://www.photo-ac.com/<br />
