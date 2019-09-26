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
- ポストを表示するpost pageを作成する
  - 