## 資料庫相關
```SQL
#創資料庫
CREATE DATABASE x;
#刪資料庫
DROP DATABASE x;
```

## 新增
###### 新增table
```SQL
CREATE TABLE teble_name(
	col1 type,
	col2 type
);
```

##### 新增現有table的col
```SQL
ALTER TABLE x ADD COLUMN col1 type;
```

###### 不能為空限制敘述
```SQL
CREATE TABLE table_name(
	col1 INT NOT NULL
);
```

###### 不重複
```SQL
CREATE TABLE table_name(
	col1 INT UNIQUE,
	col2 INT
);
```

###### 主鍵
```SQL
CREATE TABLE table_name(
	col1 INT PRIMARY KEY NOT NULL,
	col2 INT
);
```

###### 外來鍵
```SQL
CREATE TEBLE xx(
	col1 INT FOREIGN KEY REFERENCES table_name col_name,
	col2 INT 
);
```

###### 預設值
```SQL
CREATE TABLE xx(
	col1 INT NOT NULL,
	col2 NVARCHAR(50) DEFAULT 'xx'
);
```

###### 自動加值(起始值,遞增)
```SQL
CREATE TABLE Persons (  
    xx int IDENTITY(1,1), 
    xx int  
);
```

## 修改
###### 修改table中某一特定col不能為空
```SQL
ALTER TABLE table_name(
	col INT NOT NULL
);
```

###### 修改table中某一col為不重複
```SQL
ALTER TABLE xx ADD UNIQUE xx;
```

###### 修改table中每一col為主鍵
```SQL
ALTER TABLE table_name
ADD PRIMARY KEY xx;
```

###### 修改table中某一col為外來鍵
```SQL
ALTER TABLE table_name1
ADD CONSTRAINT FK_Per  
FOREIGN KEY (PersonID) REFERENCES table_name1;
```

###### 新增col index
```SQL
CREATE UNIQUE INDEX index_name
ON table_name (col1, _col2, ...);
```

## 刪除
###### 刪除資料表
```SQL
DROP table xx;
```

###### 刪除現有tabe的col
```SQL
ALTER TABLE x DROP COLUMN col
```

###### 刪除table中某一col為不重複的條件
```SQL
ALTER TABLE xx DROP INDEX xx;
```

###### 刪除table中某一col為主鍵
```SQL
ALTER TABLE table_name 
DROP PRIMARY KEY;
```

###### 刪除table中某一col為外來鍵
```SQL
ALTER TABLE table_name 
DROP FOREIGN KEY constraint_name;
```

###### 刪除table中某一col為預設
```SQL
ALTER TABLE table_name  
ALTER COLUMN xx DROP DEFAULT;
```

###### 刪除col index
```SQL
DROP INDEX table_name.index_name;
```



