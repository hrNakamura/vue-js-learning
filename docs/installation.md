# Nuxt.jsのインストール
- [Nuxt.jsのインストール](#nuxtjsのインストール)
  - [create-nuxt-appによるNuxt.js環境構築](#create-nuxt-appによるnuxtjs環境構築)
    - [npxコマンドの実行](#npxコマンドの実行)
    - [開発環境設定](#開発環境設定)
    - [アプリケーションの実行](#アプリケーションの実行)

## create-nuxt-appによるNuxt.js環境構築

### npxコマンドの実行
npxコマンドを実行できない場合は、NPM 5.2.0以上をインストールする。
（NPMは[Node.js](https://nodejs.org/ja/)インストールと同時にインストールされる）
```bash
npx create-nuxt-app <project-name>
```

### 開発環境設定

構築する環境についていくつか質問をされるので好みの方式で回答する。このマニュアルでは以下のように回答した。すべての質問に回答するとパッケージのインストールが開始される。

| 質問                                 | 回答          |
| ------------------------------------ | ------------- |
| パッケージ管理ツールの選択           | Npm           |
| UIフレームワークの選択               | None          |
| サーバーサイドのフレームワークの選択 | None          |
| Nuxt.jsのモジュールの選択            | axios         |
| Lintツール選択                       | ESLint        |
| テストフレームワークの選択           | None          |
| レンダリングモードの選択             | SSR           |
| 開発ツールの選択                     | jsconfig.json |

- パッケージ管理ツールの選択（npm or yarn）

```
? Choose the package manager (Use arrow keys)
> Yarn
  Npm
```
- UIフレームワークの選択

```
? Choose UI framework (Use arrow keys)
> None
  Ant Design Vue
  Bootstrap Vue
  Buefy
  Bulma
  Element
  Framevuerk
  iView
  Tachyons
  Tailwind CSS
  Vuetify.js
```

- サーバーサイドのフレームワークの選択

```
? Choose custom server framework (Use arrow keys)
> None (Recommended)
  AdonisJs
  Express
  Fastify
  Feathers
  hapi
  Koa
  Micro
```

- Nuxt.jsのモジュールの選択

```
? Choose Nuxt.js modules (Press <space> to select, <a> to toggle all, <i> to invert selection)
>( ) Axios
 ( ) Progressive Web App (PWA) Support
```

- Lintツール選択

```
? Choose linting tools (Press <space> to select, <a> to toggle all, <i> to invert selection)
>( ) ESLint
 ( ) Prettier
 ( ) Lint staged files
```

- テストフレームワークの選択

```
? Choose test framework (Use arrow keys)
> None
  Jest
  AVA
```
- レンダリングモードの選択
```
? Choose rendering mode (Use arrow keys)
> Universal (SSR)
  Single Page App
```

- 開発ツールの選択

```
? Choose development tools (Press <space> to select, <a> to toggle all, <i> to invert selection)
>( ) jsconfig.json (Recommended for VS Code)
```

### アプリケーションの実行

プロジェクトのフォルダに移動して以下のコマンドを実行するとhttp://localhost:3000でアプリケーションが起動する

```
npm run dev
```