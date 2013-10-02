こんにちは。2週間くらい前に、ブイン基地に新規着任した下川です。  
前回AndroidStudioのインストールなど、一通りの環境構築を行いました。  

いよいよ今回からは、アプリ開発に入っていきます。  
ちなみに本記事執筆時(10/02)には、AndroidStudio Ver0.2.10がアップデート可能となっていますので、確認してみてはいかがでしょうか？

[Android Tools Project Site](http://tools.android.com/recent)

## 新規プロジェクトの作成

AndroidStudioを起動した後に表示される、"Quick Start"から"New Project…"を選択しましょう。
図1

すると新規プロジェクト作成ウィザードに切り替わります。  
ほとんど項目は、初期設定のままで問題ありません。
アプリ名などは適当に入れます。（ここでは、SDKの最小バージョンを4.0に変更しています。）

"The prefix 'com.example.' is meant as a placeholder and should not be used"と警告が出ていますが、Androidプロジェクトではお馴染みの「パッケージ名にcom.exampleは使わないで」なので、無視しても問題ありません。  
（※厳密には問題あるのですが、ここでは省略します。）
図2

次はアプリのアイコン・ジェネレーターです。  
ここも初期状態のままで進みます。
図3

次はプロジェクトと一緒に作成するActivityのタイプを、設定出来ます。  
今回は"Blank Activity"を選択します。
図4

最後にActivityやLayoutの名称を指定します。  
ここもそのままの状態で、"Finish"を選択します。
図5

Gradle(AndroidStudioで採用しているビルドツール)の準備が終わると、作成したプロジェクト画面になります。  
好みではありますが、初期状態ではプロジェクトのツリー表示が非表示になっているので、あった方がいい場合は、"View -> Tool Windows -> Project"で表示出来ます。他にもAndroid DDMSなどのViewも配置出来ます。
図6

またLayoutファイルを選択すると、Previewが表示されます。表示されない時は、"View -> Tool Windows -> Preview"で表示出来ます。  
これはAndroidStudioの目玉機能の一つですので、ぜひ表示してみて下さい。
図7

特筆すべきは、複数の画面サイズを一覧で確認出来る機能がある点です。やり方は、Previewの中にデバイスを選択出来るプルダウンがありますので、その中から"Preview All Screen Sizes"を選択します。すると、下図のようなたくさんの画面サイズでのPreviewが、一度に表示されます。
図8

## Volleyライブラリを設定する

## 試しにVolleyで通信してみる