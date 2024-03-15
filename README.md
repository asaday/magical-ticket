# Magical入力補助

個人情報の入力だけでも楽をするためのスクリプトを生成します

## 必要なもの

Node.jsかPowerShell

## 情報入力

リネームして編集

`settings.default.json` -> `settings.json`

住所分割まわりは郵便番号入力時に自動で入るやつにうまく合わせてください。


## 実行

```
npm install
node app.ts
```

またはPowerShellで

```
./app.ps1 -ExecutionPolicy Bypass
```

出力されたJSを個人情報入力の画面で、ブラウザのDeveloper Tool（F12で出るやつ）のコンソールに貼り付けて実行します。

フォームを埋めるだけなので、適宜内容を確認してから送信ボタンを押してください

（
都道府県のselect順が都道府県コード順であると想定して作ってるので、もしかしたらずれるかも）


## Playwright

とりあえず個人情報入力までは動くはず。ボタンはまだおさない