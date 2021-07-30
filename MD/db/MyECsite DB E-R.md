```uml
@startuml
!define MASTER ff6600
!define TABLE 0073ff
entity goods as "goods\n商品テーブル" <<M,MASTER>>{
-goodsid int(10)[PK]
---
goodsname varchar(50)
goodsamount int(5)
category varchar(50)
AmountofGoods int(6)
goodsimage varchar(256)
}

entity user as "user\nユーザーテーブル" <<M,MASTER>>{
-userid varchar(64)[PK]
---
username varchar(64)
mail varchar(254)
pass varchar(32)
address varchar(128)
postalcode char(8)
+cartid int(5)[FK]
}

entity cart as "cart\nカートの中テーブル" <<T,TABLE>>{
-cartid int(5)[PK]
---
+goodsid int(10)[FK]
cartquantity int(2)
+userid carchar(64)[FK]
}

goods }o-|| cart
user ||-do-|| cart


@enduml
```
