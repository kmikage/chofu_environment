# 調布の天気
調布飛行場から500m圏内の温度・湿度を返すAPIです。

## URL
HTTP  
``http://api.mikalab.info/environment/``

HTTPS  
``https://api.mikalab.info/environment/``

## Format
```
{
  "status_code": 100,
  "body": {
    "humidity": 51, # 湿度(%)
    "temperature": 34.4 # 温度(摂氏)
  },
  "message": "success"
}
```

## 呼出し制限
呼出し回数の制限はありません。  
取得後、30秒間はキャッシュを返します。  
リアルタイムの値が欲しい場合は、30秒以上間隔をあけてアクセスしてください。

## 環境
- 調布飛行場（東京都調布市西町２９０−３）より、500m圏内
- 地上約5m
- 直射日光が当たらない屋外
- センサー：switchbot 防水温湿度計　　
https://www.switchbot.jp/products/switchbot-indoor-outdoor-meter

