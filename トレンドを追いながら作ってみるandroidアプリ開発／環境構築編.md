# トレンドを追いながら作ってみるAndroidアプリ開発／環境構築編

前回は開発環境準備編ということで、以下の3つを中心に進めていくこととしました。

1. IDEにはAndroidStudioを使う
2. 作成するアプリはQiitaクライアント
3. 通信処理にはVolleyを組み込む

今回は、実際にアプリ開発が始められる状態まで持っていけるよう、環境構築を行なってみたいと思います。  
なお、ここで紹介する手順等は、Macの場合となっています。WindowsやLinuxをお使いの方は、各環境に置き換えて確認して下さい。

## AndroidStudioをインストールする

最初に、IDEであるAndroidStudioを使えるようにします。慣れ親しんだEclipseやIntelliJ IDEA達に別れを告げ、しばし新たなパートナーを迎え入れます。（といっても、AndroidStudioはIntelliJ IDEAベースですが…）  
手順は以下のようになります。

#### 1. AndroidStudioをダウンロードする

下記公式サイトより、.dmgファイルをダウンロードします。他にもwindows用に.exeファイル、Linux用に.tgzファイルが用意されてるようです。  
http://developer.android.com/sdk/installing/studio.html

ちなみに、AndroidStudioにはAndroid SDKがバンドルされています。そのため、別途Android SDKをインストールしたり、パスを設定したりなどの手順は不要です。AndroidStudioさえインストールすれば、そのままアプリ開発が始められます。現状に比べて、かなり環境構築が楽になりそうですね。

#### 2. アプリケーションフォルダにドラッグ＆ドロップする

ダウンロードした.dmgファイルを展開すると、AndroidStudio.appが表示されますので、あとはこれをApplication FolderにDrag&Dropすれば、インストール完了です。

注意点として、AndroidStudioではバンドルされているAndroid SDKを使おうとします。AndroidStudioが使うAndroid SDKは以下の場所にありますので、中を確認する際などは間違わないように気をつけなければいけません。  
例：/Application/Android/Studio.app/sdk/

#### 3. AndroidStudioを起動してパッケージをインストールする

まずは、インストールしたAndroidStudioを起動します。初回起動時は、以下のようなWelcomeメッセージが出るようです。