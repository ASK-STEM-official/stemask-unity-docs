---
sidebar_position: 5
description: ありとあらゆるものを削除しろ(テロ)
---

# DROP文

データベースやテーブルを削除する。

## データベースの削除
```sql
DROP DATABASE データベース名
```

## テーブルの削除
```sql
DROP TABLE テーブル名  
```


## IF EXISTS

```sql
DROP DATABASE/TABLE IF EXISTS データベース名/テーブル名
```

削除の際指定したデータベースやテーブルが存在しないとエラーが発生します。

そこで IF EXISTS を使用するとデータベースが存在した時だけ削除してくれるので、

エラーが発生しません

便利だね。