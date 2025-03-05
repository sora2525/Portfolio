
# タスクエールでがんばるもん！
![キービジュアルOGP.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/893015ef-4100-4bc2-8523-79f8fb04f31d.png)



## 目次
- [サービス概要](#サービス概要)
- [サービスURL](#サービスURL)
- [サービス開発の背景](#サービス開発の背景)
- [機能紹介](#機能紹介)
- [技術構成について](#技術構成について)


# サービス概要
Web アプリ「タスクエールでがんばるもん！」はオリジナル美少女キャラクター「蓮実メロ」がLIVE２Dで動きタスクをこなしたら褒めてくれたりチャットやSNSでコミュニケーションを取ることができるサービスです。
タスクの完了やチャットなど、さまざまなアクションに対してキャラクターが音声や動作で反応するため、楽しみながらタスクを進めることができます。

# サービスURL
## https://www.task-yell.jp


# サービス開発の背景
私たちがこのサービスを作ろうと思ったのは、普段の生活で「褒められる」経験がなく、自分なりに頑張っても誰にも評価されない孤独な気持ちになってしまうことが多いからです。
周りにその存在を認めてもらえず、ふと寂しさを感じる男性たちにも、タスクをこなすたびにちょっとした喜びや自信を持ってほしいと考えました。
そんな思いから、美少女キャラクターがそっと寄り添い、励ましの言葉や温かい反応で支えてくれるサービスを企画しました。
## ユーザー層
- 二次元キャラクターが好きな方
- 自分が行ったことに対してリアクションが返ってくることが好きな方
- 孤独感を感じやすく、キャラクターとの対話や応援で日々のタスクを乗り越えたい方


# 機能紹介
| ログイン、新規登録 |
|------------------------------------|
| <img src="https://github.com/user-attachments/assets/7f65ec5d-6346-4abf-9403-ab3f8f0edeea" width="24%"> <img src="https://github.com/user-attachments/assets/685fc2e6-7e26-4989-b0be-4ad2b3f7bc77" width="24%"> <img src="https://github.com/user-attachments/assets/5bba2307-0618-411b-bdec-3c6481b77667" width="24%"> |
|『名前』『メールアドレス』『パスワード』『確認用パスワード』を入力してユーザー登録を行います。ユーザー登録後は、自動的にログイン処理が行われるようになっており、そのまま直ぐにサービスを利用する事が出来ます。また、Google,LINEアカウントを用いてログインを行う事も可能です。|

| タスク管理 |
|------------------------------------|
| <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/6f719c87-7ffa-4e67-addb-6f041a5d442b.jpeg" width="24%"> <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/c61b65fb-efe1-480d-9fe0-a974611b7546.jpeg" width="24%"> <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/3bb5eb2a-6885-4990-be3e-9e2ab4d14acd.jpeg" width="24%"> <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/300e55bf-fd6c-4179-bc2a-129c737ae7ad.jpeg" width="24%"> |
|『タイトル』『詳細の』『優先度』『期日』『リマインダー時間』を設定してタスクを追加できます。タスクにはタグを5つまで登録できます。タスク一覧では作成日、期日、優先度、タグ、完了状態でのソートができ目的のタスクを検索できます。カレンダーからのタスク管理もできドラッグアンドドロップすることで期日の変更を簡単にできます。タスクを完了状態にすると蓮実メロからの労いメッセージが届き音声で楽しむことができます。|

| チャット |
|------------------------------------|
| <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/102975b7-cda8-4c11-af73-19f9e6d5d7de.jpeg" width="24%"> <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/d25f634b-b778-44a0-a27d-660a9ae9afb1.jpeg" width="24%">  |
|チャット機能では蓮実メロとの会話を楽しむ事ができます。フォームに蓮実メロに伝えたいメッセージを入力し送信することで内容に応じた返答が来ます。蓮実メロからのメッセージはクリックすることで音声で再生されリップシンク機能によってキャラクターモデルの口が対応した動きを見せます。過去のチャット履歴は普段は閉じており自由に表示切替をできます。またチャット履歴はいつでも削除することができます。|

| 日記 |
|------------------------------------|
| <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/18025beb-eeb6-419f-85ab-c5c0d1b5e193.jpeg" width="24%"> <img src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/4022842/a17be398-1e38-4229-99bf-50c23319ce35.jpeg" width="24%">  |
|日記では蓮実メロからのリプライが届くSNSのような使い方ができます。プライベート日記と公開日記に分かれておりユーザー全体に見せたい日記の場合は公開設定にして投稿することによって他のユーザーも観ることができます。|




# 技術構成について

## 使用技術

| カテゴリ | 技術 |
|----------|----------------------------------|
| **フロントエンド** | Next.js 14.2.5 |
| **バックエンド** | Rails API 7.1.4.2 |
| **データベース** | MySQL |
| **インフラ** | Heroku・Vercel |
| **フロントエンド関連** | Auth.js・FullCalendar・PWA（Progressive Web App） |
| **認証・通信** | devise_token_auth・Mailgun・LINE Message API |
| **ストレージ** | AWS S3（クラウドストレージ） |
| **検索・フィルタリング** | Ransack |
| **アニメーション・音声** | Live2D SDK・にじボイスAPI・VOICEVOX |
| **AI・API** | OpenAI API |


## サービスの差別化ポイント・推しポイント

- **タスク管理アプリの独自性**: 多くのタスク管理アプリが存在する中で、Live2Dキャラクターによるリアクションが最大の差別化ポイント。タスクを完了したときにキャラクターが褒めたり励ましたりする機能が、他にはない独自の魅力です。
- **競合との差別化**: 「Todo Girl」などの美少女キャラクターアプリとの差別化として、Live2D、ChatGPT、にじボイスを組み合わせて動的でインタラクティブな体験を提供。リアルタイムで反応するキャラクターとの交流が可能です。


### 画面遷移図
Figma：
https://www.figma.com/design/5cLGxpFtDWaefTpKAy3KVt/Untitled?node-id=0-1&node-type=canvas&t=qnxHnhcyWxgzX3fg-0

### ER図
![ER2 drawio](https://github.com/user-attachments/assets/232cc7ed-3ca2-45e7-84b3-f60790ed027d)


