### 画面詳細図
# プロフィールページ
### [プロトタイプURL](https://www.figma.com/proto/mLtKn6PWgLvXVqKqVRbDCl/My-ECsite-Prototype?node-id=1%3A2&scaling=contain&page-id=0%3A1)
<img src="../img/プロフィール.png" width="500">

#### 対応DB要素の「???」は未定

|ID|要素|内容|アクション|カテゴリ,イベント|対応DB要素(テーブル名:カラム)|
|---|---|---|---|---|---|
|1|バナー|サイト名表示|クリック|遷移,トップページ|-|
|2|検索バナー|入力欄|テキスト入力|-|-|
|3|検索ボタン|ボタン|クリック|遷移,検索結果ページ|goods:goodsid,goodsname,goodsamount,category,goodsimage|
|4|プロフィールアイコン|ボタン(?)|クリック|遷移,プロフィールページ|user:userid,username,mail,pass,address|
|5|アカウント登録|ボタン|クリック|遷移,アカウント登録ページ|user:userid,username,mail,pass,address|
|6|ログイン|ボタン|クリック|遷移,ログインページ|user:mail,pass|
|7|カート|ボタン|クリック|遷移,カート内ページ|cart:cartquantity goods:id user:userid|
|8|チェスセット|リンク|クリック|遷移,検索結果ページ|goods:goodsid,goodsname,goodsamount,category,goodsimage|
|9|チェス駒|リンク|クリック|遷移,検索結果ページ|goods:goodsid,goodsname,goodsamount,category,goodsimage|
|10|チェス盤|リンク|クリック|遷移,検索結果ページ|goods:goodsid,goodsname,goodsamount,category,goodsimage|
|11|商品サムネイル|画像,リンク|クリック|遷移,商品詳細ページ|goods:goodsid,goodsname,goodsamount,category|
|12|プロフィール|ボタン|クリック|遷移,プロフィールページ|user:username,userid,mail,pass,address|
|13|プロフィールを変更する|ボタン|クリック|遷移,プロフィール変更ページ|user:userid,username,mail,pass,address|
|14|退会する|ボタン|クリック|ポップアップ,警告|user:userid,username,mail,pass,address|
