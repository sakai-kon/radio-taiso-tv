# Radio Taiso TV

ラジオ体操第一・第二を、ページ内のYouTube公式プレーヤーで再生するシンプルなWebサイトです。iPhoneやテレビのブラウザで見やすい大きなボタンと、画面いっぱいの再生画面を用意しています。

## 使い方

1. サイトを開く
2. 「ラジオ体操 第一」または「ラジオ体操 第二」を押す
3. ページ内のYouTubeプレーヤーで再生する
4. 必要に応じてプレーヤー内の全画面ボタン、またはページ上部の「全画面」を押す
5. 「メニュー」で選択画面に戻る

## 使用動画

かんぽ生命公式「ラジオ体操チャンネル」の実演動画です。

- 第一: https://www.youtube.com/watch?v=_YZZfaMGEOU
- 第二: https://www.youtube.com/watch?v=yi1TbzML2cU
- 公式チャンネル: https://www.youtube.com/@radiotaisou

## 公開（GitHub Pages）

1. リポジトリの **Settings** を開く
2. **Pages** を開く
3. **Deploy from a branch** を選択
4. Branch を `main`、Folder を `/(root)` にして保存

## 再生・全画面について

- 動画はYouTubeの公式埋め込みプレーヤーでサイト内再生します。通常の動画リンクへ移動する実装ではありません。
- 選択時に自動再生を試みますが、ブラウザやテレビの設定によって自動再生が制限された場合は、プレーヤー中央の再生ボタンを押してください。
- 再生画面はブラウザの表示領域いっぱいに広がります。ブラウザがFullscreen APIに対応していれば全画面化も試みます。iPhoneなど一部の環境ではブラウザ側の制限により自動でネイティブ全画面へ切り替わらないため、YouTubeプレーヤー内の全画面ボタンを使ってください。
- 全画面ボタンはYouTubeプレーヤー内にも表示されます（YouTube側の仕様・端末に依存）。
- このサイト自体がiPhoneからREGZAへのCast接続を直接制御するものではありません。

## 技術

- HTML / CSS / JavaScript
- YouTube公式IFrame埋め込みプレーヤー
- GitHub Pages（静的サイト）
