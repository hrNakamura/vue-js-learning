# Ch. 02 Working with Nuxt.js

## Customize the home page

https://vueschool.io/lessons/customize-the-home-page

- scalffolding（足場）ツールで生成されたページについて
  - ホームページはpagesディレクトリのindex.vueファイルから生成される
  - いくつかのヘッダやリンクから構成される
  - いくつかのスタイル（CSS）も付随している
- ロゴを変更したい場合はcomponentsディレクトリのLogo.vueを以下のように変更する
  - 変更してブラウザを参照すると変更が反映されている
```html
<template>

  <img src="https://vueschool.io/img/favicons/apple-touch-icon.png" alt="the logo">

</template>
```

## Nuxt.js Page Components

https://vueschool.io/lessons/nuxtjs-page-components

- Nuxt.jsで新しいページを作成するためには、pagesディレクトリ内にコンポーネントを作成しなくてはならない
- Nuxtではルートは自動的に作成される
- ポストを表示するpost.vueを作成する
- \<article\>html5のタグ

## Global CSS

https://vueschool.io/lessons/global-css

- layoutフォルダで全体のスタイルを定義する
- 他フォルダのCSSファイルを指定できる
  - ~：ルートディレクトリ
- 適用するには再ビルドが必要

## Adding a Navbar to Nuxt Apps

https://vueschool.io/lessons/adding-a-navbar-to-nuxt-apps

- ナビバー（サイドバー）を追加したい場合は\<nav\>を追加する
- ナビバーのコンポーネントをcomponentフォルダに作成する

## Dynamic Routes

https://vueschool.io/lessons/nuxtjs-dynamic-routes

- 動的ルーティングはNuxt.jsでは自動的に生成される
  - 動的ルーティング：表示したいコンテンツのidを以下のようにURLで指定できる
    - https://domain/post/{id}
  - ファイル名を_id.vueとする
    - idで動的ルーティングする場合

