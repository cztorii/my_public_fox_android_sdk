## 最新バージョンへのアップデートについて

以前のF.O.X SDKが導入されたアプリに最新のSDKを導入する際に必要な手順は以下の通りです。

1. 以前のバージョンの AppAdForce.jar がプロジェクトに組み込まれていれば、それらを削除
2.  「2. SDK 導入手順」に従い最新の AppAdForce.jar をプロジェクトに追加


※「[（オプション）広告IDを利用するためのGoogle Play Services SDKの導入](../../google_play_services/ja/)」が未実施の場合には対応してください。


※「[（オプション）外部ストレージを利用した重複排除設定](../../external_storage/ja/)」が未実施の場合には対応してください。




AdManager.updateFrom2_10_4g(); // 必ず new AdManager より前でコールすること
AdManager ad = new AdManager(this);









