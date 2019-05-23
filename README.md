# Frontend.sasslib
社内共通のSassライブラリです。

## Install
```bash
$ npm install --save-dev @gmo-media/sasslib
```

## How to use
必要なファイルを import します。
[node-sass-package-importer](https://www.npmjs.com/package/node-sass-package-importer) を使うのが便利です。

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

npmに公開するときは、Organizationメンバーのアカウントで

```bash
$ npm run update:minor
```

バグフィックスなどの場合は

```bash
$ npm run update:patch
```
