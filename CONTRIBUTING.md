## How to develop (for Contributor)

3 つのセッションを立ち上げてそれぞれで以下のコマンドを実行してください。

````console
$ # watch ビルドを立ち上げる
$ npm run dev

```console
$ # デモサーバーを立ち上げる
$ cd demo
$ npm run dev
````

```console
$ # デモ環境で eco-backstopjs-runner を実行する
$ cd demo
$ npm run backstop
```

## How to release (for Contributor)

```console
$ # Wait for passing CI...
$ git switch main
$ git pull
$ rm -rf dist && npm run build
$ yarn version
$ npm publish
$ git push --follow-tags
```
