
### 質問５のDB定義

## 購入テーブル

### d_purchase (購入テーブル)
|属性名|型|PK|NN|FK|
|---|---|---|---|---|
|order_id|bigint(20)|◯|◯||
|customer_code|varchar(50)||◯||
|purchase_date|date||◯||
|total_price|int(11)||◯||

### d_purchase_detail(購入テーブル詳細)
|属性名|型|PK|NN|FK|
|---|---|---|---|---|
|detail_id|bigint(20)|◯|◯||
|order_id|bigint(20)||◯|◯||
|item_code|int(11)||◯||
|price|int(11)||◯||
|num|int(11)||◯||
||||||

### m_customers(ユーザー（顧客）テーブル)
|属性名|型|PK|NN|FK|
|---|---|---|---|---|
|custommer_code|varchar(50)|◯|◯||
|pass|varchar(50)||◯||
|name|varchar(20)||◯||
|address|varchar(100)||◯||
|tel|varchar(20)||◯||
|mail|varchar(100)||◯||
|del_flag|int(1)||||
|reg_date|date||◯||

### m_category(カテゴリテーブル)
|属性名|型|PK|NN|FK|
|---|---|---|---|---|
|category_id|int(11)|◯|◯||
|name|varchar(20)||◯||
|reg_date|date||◯||

### m_items(商品テーブル)
|属性名|型|PK|NN|FK|
|---|---|---|---|---|
|item_code|int(11)|◯|◯||
|item_name|varchar(50)||◯||
|price|int(11)||◯||
|category_id|int(11)||◯|◯|
|image|varchar(200)||◯||
|detail|varchar(500)||||
|del_flag|int(11)||||
|reg_date|date||◯||









