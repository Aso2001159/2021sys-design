```uml
@startuml
 ユーザー -> webサーバー : ログイン情報入力
 webサーバー -> DB : ログイン情報検索処理
 DB -> DB : 検索処理
 DB -> webサーバー : 検索結果
 webサーバー -> ユーザー : 検索結果
 alt ID,パスワードが一致
 webサーバー -> ユーザー : ログイン
@enduml

```
