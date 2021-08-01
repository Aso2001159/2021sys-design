# 自分のECサイトのDB定義書
### ER図

# DBテーブルカラム名詳細一覧

### goods(商品テーブル)
|和名|属性名(カラム名)|型|PK|NN|FK|
|---|---|---|---|---|---|
|グッズID|goodsid|int(10)|◯|◯||
|グッズ名|goodsname|varchar(50)||◯||
|グッズ量|goodsamount|int(5)||◯||
|カテゴリ|category|varchar(50)||◯||
|料金|AmountofGoods|int(6)||◯||
|商品画像|goodsimage|varchar(256)||◯||/*相対パスを記述する*/
|||||||

### user(ユーザーテーブル)
|和名|属性名(カラム名)|型|PK|NN|FK|
|---|---|---|---|---|---|
|ユーザーID|userid|varchar(64)|◯|◯||
|ユーザー名|username|varchar(64)||◯||
|メールアドレス|mail|varchar(254)||◯||/*RFC5321 4.5.3で規定されている。*/
|パスワード|pass|varchar(32)||◯||
|住所|address|varchar(128)||◯||
|郵便番号|postalcode|char(8)||◯||
|カートID|cartid|int(5)||◯|◯|


### cart(カートの中テーブル)
|和名|属性名(カラム名)|型|PK|NN|FK|
|---|---|---|---|---|---|
|カートID|cartid|int(5)|◯|◯||
|グッズID|goodsid|int(10)||◯|◯|
|カート内グッズの数|cartquantity|int(2)||◯||
|ユーザーid|userid|carchar(64)||◯|◯|
|||||||


/*画像テーブルは作らない<br>
パスを補填でいい<br>
プログラム的に(サーバーサイド??)パスを合体させるので、ここでは相対パスのみを記述する<br>
E-R図とはどっちから作っても構わん<br>
BLOB型に関してはあんまりメジャーな型ではなさそう<br>
