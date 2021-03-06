---
description: 版本：10
---

# 11.6. 唯一值索引

索引還可用於強制欄位值的唯一性，或多個欄位的組合值唯一性。

```text
CREATE UNIQUE INDEX name ON table (column [, ...]);
```

目前，只能將 B-tree 索引宣告為唯一。

當索引宣告為唯一時，不允許具有相等索引值有多筆資料。但空值不被視為相等， 多欄位唯一索引僅拒絕所有索引欄位在多筆資料中相等的情況。

當為資料表定義唯一限制條件或主鍵時，PostgreSQL 會自動建立唯一索引。索引涵蓋構成主鍵或唯一限制條件的欄位（如果適用，則為多欄位索引），並且是強制執行限制條件的機制。

**注意**  
毋須在宣告唯一性的欄位上手動建立索引；這樣做只會複製自動建立的索引。

