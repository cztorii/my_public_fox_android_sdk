### Android Studioプロジェクトへの導入

Android StudioプロジェクトへAppAdForce.jarを追加する方法は以下の通りです。

* アプリケーションプロジェクトの「libs」フォルダー配下にAppAdForce.jarを配置します。


![integration01](./img01.png)


* AppAdForce.jarへのパスをbuild.gradleに追記します。

```
dependencies {
	compile files('libs/AppAdForce.jar')
}
```

![integration02](./img02.png)
