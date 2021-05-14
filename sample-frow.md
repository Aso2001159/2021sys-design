```uml

@startuml
  ユーザー -> webサーバー : 登録情報
  webサーバー -> DB : 登録情報
  DB -> DB : 入力処理
  DB -> webサーバー : 結果出力
  webサーバー -> ユーザー : 結果出力
  alt ID,アドレスの値の重複無し
  webサーバー -> ユーザー : 登録結果
  else ID,アドレスの値の重複あり
  webサーバー -> ユーザー : エラーを出力
  end
@enduml

```
