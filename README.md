# Frontend.sasslib
社内共通のSassライブラリです。

## Install
```bash
$ npm install --save-dev @gmo-media/sasslib
```

## How to use
必要なファイルを import します。

[node-sass-package-importer](https://www.npmjs.com/package/node-sass-package-importer) を使い、

```scss
@import "~@gmo-media/sasslib";
```

とすると `src/` 以下の `utility/` 以外のファイルが全て読み込まれます。

`utility/` 以下のファイルは必要に応じて１つ１つ読み込んでください。

```scss
@import "~@gmo-media/sasslib/src/utility/fix-ios";
```

## Development
```bash
$ git clone git@github.com:gmo-media/Frontend.sasslib.git
$ npm install
```

ファイルを追加修正したら

```bash
$ npm test
```

機能追加したらレビュー依頼してください。

- 必要最低限の要素しか定義しないこと
- 各ファイルは単独で`@import`されても動くこと
- 引数やデフォルト値について十分に検討すること
- `@content`を使って拡張しやすいようにすること

npmに公開するときは、Organizationメンバーのアカウントで

```bash
$ npm run update:minor
```

バグフィックスなどの場合は

```bash
$ npm run update:patch
```
