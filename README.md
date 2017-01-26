# Cordovaプロジェクトの構築

## 前提条件
1. Cordovaを使用できるようになっていること。下記README.mdの「Cordovaを使ってapkファイルを作成」ができていること

 [tba-app-client](https://github.com/YosukeSasaoka/tba-app-client)

2. tba-app-clientを元にしたclientであること

## Android端末での動作まで
※ clientアプリ(tba-app-clientとします)と、このtba-app-client-cordovaが、同一のディレクトリにあるとします。

※ また、カレントディレクトリは tba-app-client-cordova にいるとします。

### [1] シンボリックリンク作成

下記のコマンドを実行して、シンボリックリンクを作成します
(tba-app-client/wwwをtba-app-client-cordova/wwwとしてアクセスできるようにします。

ln -s ../tba-app-client/www www

### [2] プロジェクトの準備
下記のコマンドプラットフォームとプラグインをインストールします)

cordova prepare

### [3] Android 端末での動作確認
Android端末(ロック解除済み)を接続して、下記コマンドを実行します。

cordova run android

