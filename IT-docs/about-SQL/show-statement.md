---
sidebar_position: 3
description: ありとあらゆるものを表示しろ
---

# SHOW文

データベースやテーブルの情報を一覧表示する。

## データーベースの一覧表示

データベース名の一覧を表示します。

```sql
SHOW DATABASES [LIKE 'パターン' WHERE '条件'];
```

## テーブルの一覧表示

```sql
SHOW TABLES FROM [スキーマ名] [LIKE 'パターン'];
```

## フィールド/カラムの一覧表示

```sql
SHOW FIELDS/COLUMNS FROM [(スキーマ名.)テーブル名] [LIKE 'パターン' WHERE '条件'];
```
