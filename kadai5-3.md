## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
エンドポイントはhttps://zipcloud.ibsnet.co.jp/api/search
郵便番号から住所に変換する機能がある。
* リクエストとレスポンスのフォーマット
リクエスト
https://zipcloud.ibsnet.co.jp/api/search?zipcode={郵便番号}
レスポンスはjson形式
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
OpenStreetMap Nominatim_API
https://nominatim.org/release-docs/latest/api/Reverse/
* エンドポイントと機能
エンドポイント
https://nominatim.openstreetmap.org/reverse
機能
緯度と経度を入力すると入力された座標の地点にある構造物や住所を返す
* リクエストとレスポンスのフォーマット
リクエスト
https://nominatim.openstreetmap.org/reverse?lat={緯度}&lon={経度}&{任意の条件}

レスポンス
&format=jsonを追加することでフォーマットがjson形式になる
### Q3-3. 感想
* 今回の課題で苦労したこと
jsonからほしい値だけを取り出す処理を作ること
* 演習を通して理解できたこと
文字列からjson形式への変更などのjsonの扱い
* Web APIの利便性や課題など
公開されているAPIを使うことで様々な処理を行うことができる。
アプリに組み込んだ場合、インターネット接続が必要になってしまう。
