## 基本語法
```SQL
SELECT --查詢
UPDATE --更新
DELETE --刪除
INSERT TO --新增
CREATE DATABASE --創資料庫
ALTER DATABASE --修改資料庫
CREATE TABLE --創資料表
ALTER TABLE --修改資料表
DROP TABLE --刪除資料表
CREATE INDEX -- 創index
DROP INDEX --刪除index
```

## 新增

```SQL
INSERT INTO table_name(col1, col2) VALUES (val1, val2);
```

## 修改
```SQL
UPDATE table_name SET col1 = val1, col2 = val2,  WHERE condition;
```

## 刪除
```SQL
DELETE FROM table_name WHERE condition;
```

## 查詢
```SQL
#search all cloumns in ...
SELECT *FROM table_name;
#查詢特定column
SELECT column FROM table_name;
#找出特定column值的種類
SELECT DISTINCT xx FROM table_name;
#算出特定cloumn的種類的總和
SELECT COUNT(DISTINCT column) FROM table_name;
#加條件查詢
SELECT col FROM table_name WHERE condition;
#排序語法 結尾加上DEDC可以降冪排列
SELECT * FROM table_name  ORDER BY x;
#取兩 cloumns排序
SELECT * FROM table_name ORDER BY x, x;
#Null 
SELECT col  FROM table_name  WHERE col IS NULL;
#SQL SEVER 取前幾筆資料
SELECT TOP number col FROM table_name WHERE condi;
#My Sql 取前幾筆資料
SELECT col FROM table_name WHERE condi LIMIT number ;
#取極值平均...min, max, avg, count, sum 寫法都一樣
SELECT MIN(column_name) FROM table_name WHERE condi;
#查詢資料裡面是否有某一個字元開頭/結尾%放後面
SELECT * FROM table_name WHERE xx LIKE 'x%';
#查詢某資料是否有這些字
SELECT * FROM table_name WHERE xx LIKE '%x%';
#查詢col1中值為x的資料
SELECT * FROM table_name WHERE clo1 in ('x', 'x');
#查詢clo1中值從x-xx中的資料
SELECT * FROM tabale_name WHERE col1 BETWEEN x AND xx;
#col1 縮寫成x, col2所寫成xx
SELECT col1 as x, clo2 as xx FROM table_name;
#join資料表:inner, left, right, full
SELECT * FROM table1 INNER JOIN table2 
ON table1.x = table2.x;
#資料表合併在某一col1裡有一樣的val會合併
SELECT col1 FROM table1 
UNION 
SELECT col2 FROM table2;
#UNION ALL 某一col內不一樣的val視為不同
SELECT col1 FROM table1
UNION ALL 
SELECT col2 FROM table2;
```
