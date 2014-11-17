## 最新バージョンへのアップデートについて

以前のF.O.X SDKが導入されたアプリに最新のSDKを導入する際に必要な手順は以下の通りです。
1. 以前のバージョンのライブラリファイル及びヘッダファイルがプロジェクトに組み込まれていれば、それらを削除 
1. 最新バージョンのファイルをプロジェクトに追加1. Xcodeの「Product」→「Clean」を実行

F.O.X iOS SDK v2.12以降では、ライブラリファイルはlibAppAdForce.aのみ提供されます。v2.11以前は個別に分かれていたライブラリは全てlibAppAdForce.aに含まれます。アップデートの際に以下のファイルが組み込まれている場合には全て削除してください。

* libLtv.a
* libAnalytics.a
* libNotify.a

最新版が確実に導入されているかどうかは、setDebugModeメソッドをコールすることで確認できます。

```objectivec
[[AppAdForceManager sharedManager] setDebugMode:YES];
```
以下の出力にバージョン番号がありますので、最新のものと一致しているかを確認してください。

```
 [5160:c07] ===== FORCE OPERATION X DEBUG DESCRIPTION ===== [5160:c07] Force Operation X SDK v2.13.4g
```
setDebugModeメソッドは、リリース時には削除してください。

SDKのアップデート後は、必ず疎通テストを実施し、計測及びアプリケーションの動作に問題ないことを確認してください。

## v2.11.1以前からのアップデート

v2.11.1以前のSDKからのアップデートでは、iAd.frameworkを追加で組み込む必要があります。

## v2.8.1以前からのアップデート
v2.8.1以前のSDKからのアップデートにおいては、AdSupport.frameworkを追加で組み込む必要があります。

[TOP](https://github.com/cyber-z/public_fox_ios_sdk)
