# 権限設定について

## ACL(Access Control List)

- アクセス権限をリスト化したもの
- 現在のJの管理者権限はこれ

## RBAC(Role-Based Access Control)

- ユーザーに対してロールを与える仕組み
- ロールのプロトタイプなど用意すれば便利そう(カスタムロール)

## ABAC(Attribute-Based Access Control)

- ユーザーの属性によって権限を設定
- ユーザーはロール上実行可能であるがユーザーの属性上不可能的な

## RAdAC(Risk Adaptive-Based Access Control)

- リスク回避での判断

## わかりやすく置き換えると

> ACL: Your name is on the list  
> RBAC: You have a pink wristband  
> ABAC: You're the right age  
> RAdAC: You haven't been to a country with Spanish Flu  

## 権限設定はこんな感じ

- カスタムロールを設定しテーブルで持ち、それをユーザーに割り振る
- ABACをチェックする関数を用意、都度チェック

### 参考
- https://dzone.com/articles/acl-rbac-abac-pbac-radac-and-a-dash-of-cbac