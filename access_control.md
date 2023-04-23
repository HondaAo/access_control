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

## まとめると

>> ACL: Your name is on the list
>> RBAC: You have a pink wristband
>> ABAC: You're the right age
>> RAdAC: You haven't been to a country with Spanish Flu

## Jでの提案

- RBAC方式をテーブルで持つ
- ABACをチェックする関数を用意、都度チェック
- オプション設定・隠しオプ設定も都度チェック、ドキュメントでまとめる必要あり
