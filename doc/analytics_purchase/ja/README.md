## アクセス解析による課金計測

アクセス解析機能を利用し、自然流入経由を含めた広告別の課金計測を行うことができます。アクセス解析による課金計測を行うために、下記の処理を実装してください。尚、LTV計測においても課金を成果地点としている場合には、同一の箇所にLTVとアクセス解析のそれぞれの計測処理を実装してください。


```java:
import jp.appAdForce.android.AnalyticsManager;

// LTV計測による課金計測
LtvManager ltv = new LtvManager(ad);
ltv.addParam(LtvManager.URL_PARAM_PRICE, "9.99");
ltv.addParam(LtvManager.URL_PARAM_CURRENCY, "USD");
ltv.sendLtvConversion(成果地点ID);

// アクセス解析による課金計測AnalyticsManager.sendEvent(this, action, null, null, orderId, sku, itemName, 9.99, 1, "USD");
```

