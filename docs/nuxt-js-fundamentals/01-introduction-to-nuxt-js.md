# Ch.01 Introduction to Nuxt.js

## Sec.1 What is Nuxt.js?
https://vueschool.io/lessons/what-is-nuxtjs

- Server Side Rendering
  - javascript共通の問題：以下を扱うのが難しい
    - SEO(Search Engine Optimization)
    - メタタグ
  - 理由：データ取得をjavascriptに依存している
    - 初期ロード時はページが空である
    - javascriptが実行されるまでは、インデックス付けや解析されるコンテンツが存在しない
  - クローラーがjavascriptをサポートしていない
  - SSRによって解決する
    - SSR：サーバー側でHTMLを生成してクライアントやクローラーへのレスポンスとする
      - メタタグなども埋め込まれる
    - SSRによってパフォーマンスも改善する

- Pre Rendering
  - HTMLを事前に生成する
  - productionディレクトリに一つのHTMLファイルのみが含まれる

- code splitting
  - プロジェクトに応じて自動的にjsファイルを分割する

## Sec.2 Create Nuxt App

https://vueschool.io/lessons/create-nuxt-app

- Nuxt.jsのscalffolding（足場）ツール
  - npx or yarnで以下のコマンドを実行する

```
npx create-nuxt-app <prject name>
```
```
yarn create nuxt-app <project name>
```
- 質問される
1. デフォルトプロジェクト名についての質問
   1. デフォルト
2. デフォルトのプロジェクトdescriptionについての質問
   1. デフォルト
3. カスタムサーバーフレームワークの選択
   1. none
4. カスタムUIの選択
   1. none
5. モードの選択
   1. Universal
6. 以下スキップ（デフォルト）

## Sec.3 Guided Nuxt.js Project Tour

https://vueschool.io/lessons/guided-nuxtjs-project-tour

プロジェクトの各ディレクトリの説明
- assets
  - コンパイルしないアセットのフォルダ
    - 例：SASSファイル
      - [SASS](https://sass-lang.com/)とは：CSSを効率的に書くためのメタ言語
      - https://qiita.com/m0nch1/items/b01c966dd2273e3f6abe
    - 例：画像
    - 例：フォント
  - components
    - vue.jsのコンポーネントを格納するフォルダ
      - [vue.jsのコンポーネント](https://jp.vuejs.org/v2/guide/components.html)
  - layouts
    - ページの外観を変更するためのフォルダ
    - 例：サイドバー
  - middleware
    - ミドルウェアを格納するディレクトリ
    - ミドルウェアとは
      - 自分で定義した関数
      - ページが描画される前に実行できる
  - pages
    - アプリのビューとルートファイルを格納するディレクトリ
    - このディレクトリ中のすべてのvueファイルが読み込まれて、自動的にアプリのルートが生成される
  - plugins
    - javascriptのプラグインを格納するディレクトリ
    - vueのルートがインスタンス化される前に実行される
    - 使い方
      - グローバルコンポーネントの登録
      - 定数・関数の挿入
  - static
    - サーバーのルートに自動的に配置されるファイルを置くディレクトリ
      - 例："logo.png"のようなファイルを置くと、url/logo.pngでアクセスできる
  - store
    - vuexストアファイルを置くディレクトリ
    - vuexストアはNuxt.jsに付属しているが、デフォルトではOFFとなっている

各ディレクトリにはReadMeファイルが含まれている。
assetsやstoreのような必須でないディレクトリは削除してもよい。