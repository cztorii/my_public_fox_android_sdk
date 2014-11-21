## Google Playデベロッパープログラムへの準拠

Force Operation X Android SDKはGoogle Playデベロッパープログラムポリシーに準拠しています。本SDKはポリシーに準拠するために、永続的なデバイス ID（IMEI、MACアドレス及びAndroidID）が取得される場合には広告IDが取得されません。2014年8月1日から、Google Playストアにアップロードされたすべての更新や新着アプリには、広告目的で使用する端末IDには広告ID を利用する必要があります。本ポリシーに準拠するために、以下の手順を行ってください。


## Google Play Services SDKの導入


広告IDを利用できるようにするために、Google Play Services SDKが組み込まれている必要があります。
アプリケーションにGoogle Play Services SDKが組み込まれていない場合には、次のサイトの手順に従い、導入を行ってください。

[Setting Up Google Play Services | Android Developers](https://developer.android.com/google/play-services/setup.html)