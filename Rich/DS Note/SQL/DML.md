

## 新增

```SQL
INSERT INTO table_name(col1, col2) VALUES (val1, val2);
```

## 修改
```SQL
#SET寫的是要更改的值
UPDATE table_name SET col1 = val1, col2 = val2,  WHERE condition;
```

## 刪除
```SQL
DELETE FROM table_name WHERE condition;
```

## 查詢

###### search all cloumns in ...
```SQL
SELECT *FROM table_name;
```

###### 查詢特定column
```SQL
SELECT column FROM table_name;
```

###### 找出特定column值的種類
```SQL
SELECT DISTINCT xx FROM table_name;
```

###### 算出特定cloumn的種類的總和
```SQL
#DISTINCT 查詢不重複的值
SELECT COUNT(DISTINCT column) FROM table_name;
```

###### 加條件查詢
```SQL
SELECT col FROM table_name WHERE condition;
```

###### 排序語法 結尾加上DEDC可以降冪排列
```SQL
SELECT * FROM table_name  ORDER BY x;
```

###### 取兩 cloumns排序
```SQL
SELECT * FROM table_name ORDER BY x, x;
```

###### 查詢是空值的data
```SQL
SELECT col  FROM table_name  WHERE col IS NULL;
```

###### 取前幾筆資料
```SQL
#MS SQL
SELECT TOP number col FROM table_name WHERE condi;
#My Sql 取前幾筆資料
SELECT col FROM table_name WHERE condi LIMIT number ;
```

###### 取極值平均...min, max, avg, count, sum 寫法都一樣
```SQL
SELECT FROM table_name WHERE condi;
```

###### 查詢資料裡面是否有某一個字元開頭/結尾%放後面
```SQL
SELECT * FROM table_name WHERE xx LIKE 'x%';
```

###### 查詢某資料是否有這些字
```SQL
SELECT * FROM table_name WHERE xx LIKE '%x%';
```

###### 查詢col1中值為x的資料
```SQL
SELECT * FROM table_name WHERE clo1 in ('x', 'x');
```

###### 查詢clo1中值從x-xx中的資料
```SQL
SELECT * FROM tabale_name WHERE col1 BETWEEN x AND xx;
```

###### col1 縮寫成x, col2所寫成xx
```SQL
SELECT col1 as x, clo2 as xx FROM table_name;
```

###### join資料表:inner, left, right, full
```SQL
SELECT * FROM table1 INNER JOIN table2 
ON table1.x = table2.x;
```

###### 資料表合併在某一col1裡有一樣的val會合併
```SQL
SELECT col1 FROM table1 
UNION 
SELECT col2 FROM table2;
```

###### 某一col內不一樣的val視為不同
```SQL
SELECT col1 FROM table1
UNION ALL 
SELECT col2 FROM table2;
```
