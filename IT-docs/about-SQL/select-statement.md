---
sidebar_position: 3
description: ありとあらゆるものを検索せよ
---

# SELECT文

条件に合うデータを検索するための文章です。SELECTを日本語にすると選択になります。データを選択する文章と表現するのが適切かもしれません。

SELECT文に限らず、基本的にSQLのクエリは[この動きをしてほしい][このデータベースで][こういう条件で]という文の組み立て方をするので覚えておくといいと思います。英語よりも簡単だから…

## 指定したテーブル内のデータを全選択して表示

```sql
SELECT * FROM [(スキーマ名.)テーブル名]
```

アスタリスクはすべての列を選択するという意味になっています。

## 指定したテーブル内の指定した列を表示

```sql
SELECT [選択する列],[選択する列],[選択する列] FROM [(スキーマ名.)テーブル名]
```

SELECT句の次に選択したい列をコンマで区切って列挙していきます。最後のやつにはコンマいりません。

## SELECT文で検索をかける

# 比較演算子

|            |                         |
| ---------- | ----------------------- |
| 等しい     | =                       |
| 等しくない |\<\> |
| Varchar | 文字を入力できる |
| date | 年4けた/月2けた/日2けた |