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

###### 排序語法 
```SQL
#升冪
SELECT * FROM table_name  ORDER BY x;
#降冪
SELECT * FROM table_name  ORDER BY x DESC;
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
SELECT sum(col_name) FROM table_name;
```

###### 四捨五入到指定位數
```SQL
SELECT ROUND(col, x) FROM table_name
```

###### 返回字串的長度
```SQL
SELECT LENGTH(col) FROM table_name
```

###### 取出的資料換成大小寫
```SQL
#大寫
SELECT UPCASE(col) FROM table_name
#小寫
SELECT LCASE(col) FROM table_name
```

###### 資料取出後改title
```SQL 
SELECT example as ex FROM x; 
```

###### 查詢資料裡面是否有某一個字元開頭or某一字結尾
```SQL
#x開頭
SELECT * FROM table_name WHERE xx LIKE 'x%';
#x結尾
SELECT * FROM table_name WHERE xx LIKE '%x';
```

###### 查詢某一column中相同的值有多少個
```SQL
SELECT col_name FROM tabale_name GROUP BY col_name
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
#inner join是取交集(不會有空值)
#left join左邊為主右邊沒值時會用NULL填
#outer join取聯集
SELECT * FROM table1 () JOIN table2 
ON table1.x = table2.x;
```

###### 資料表合併在某一col裡有一樣的val會合併
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

###### 子查詢
```SQL
#子查詢要加()
SELECT col1, col2 FROM table_name 
WHERE col (SELECT col FROM table_name WHERE condi);
```