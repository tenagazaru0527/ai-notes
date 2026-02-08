# タイトル
Webアプリ構成

## なぜ重要か
構成の簡易図




## 要点
Express / FastAPI / Spring Boot はあなたが書く「アプリサーバ」の土台。
Apache / Nginx はその前段でHTTPをさばく専門職。  
  
　　　[ ブラウザ ]  
↓  
　　　 HTTPリクエスト  
↓  
┌───────┐  
│ Webサーバ │ ← Apache / Nginx / LB  
└───────┘  
↓  
┌───────┐  
│ アプリサーバ │ ← Express / FastAPI / Spring  
│（あなたが書く） │  
lux───────┘  
↓  
┌───────┐  
│ 業務ロジック │  
└───────┘  
↓ 処理結果  
　 [ Webサーバ ]  
　↓ HTTP応答  
[ ブラウザ表示 ]  
