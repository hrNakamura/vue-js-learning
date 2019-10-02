# Ch.03 Build & Deploy

## Build and Serve the Nuxt.js App

https://vueschool.io/lessons/builde-and-serve-the-nuxtjs-app

- ビルド
  - yarn build
- 起動
  - yarn start
  - localhost:3000で起動する

## How to Deploy Nuxt.js to Heroku

https://vueschool.io/lessons/how-to-deploy-nuxtjs-to-heroku

- Herokuへのデプロイ方法
  - https://jp.heroku.com/

1. herokuアカウント取得
2. 無料プランを選択
3. リポジトリに従って以下の手法を実施
   1. github：直接デプロイできる
   2. git：heroku-cliをインストールする
      1. heroku-cliの説明に従ってherokuにコードをpush
      2. いかに従って設定を行う
         1. https://nuxtjs.org/faq/heroku-deployment/
      3. heroku用の実行コマンドを追加してコードをコミット

## How to Deploy Nuxt.js to Netlify

https://vueschool.io/lessons/how-to-deploy-nuxtjs-to-netlify

- NetlifyやGithub pagesに対して静的なページをデプロイする方法
- yarn generateでhtmlを生成
- distフォルダに出力される
- nuxt.config.jsでルーティングを設定すればindex以外のページも生成できる
- Netlifyで公開する場合はリポジトリを指定して静的ページの生成コマンド（yarn generate）を指定する
