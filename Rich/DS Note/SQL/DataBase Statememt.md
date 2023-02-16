## 資料庫相關
```SQL
#創資料庫
CREATE DATABASE x;
#刪資料庫
DROP DATABASE x;
```

## 新增資料表
```SQL
#新增table
CREATE TABLE xx(
	col1 type,
	col2 type
);
#新增現有table的col
ALTER TABLE x ADD COLUMN col1 type;
#不能為空限制敘述
CREATE TABLE table_name(
	col1 INT NOT NULL
);
#其他限制
#不重複
CREATE TABLE table_name(
	col1 INT NOT NULL UNIQUE,
	col2 INT
);
#主鍵
CREATE TABLE table_name(
	col1 INT NOT NULL PRIMARY KEY,
	col2 INT
);
#外來鍵
CREATE TEBLE xx(
	col1 INT NOT NULL PRIMARY,
	xx INT FOREIGN KEY REFERENCES xx
);
#預設值
CREATE TABLE xx(
	col1 INT NOT NULL,
	xx NVARCHAR(50) DEFAULT 'xx'
);
#自動加值(起始值,遞增)
CREATE TABLE Persons (  
    xx int IDENTITY(1,1) PRIMARY KEY, 
    xx int  
);
```

## 修改資料表
```SQL
#修改table中某一特定col不能為空
ALTER TABLE table_name(
	col INT NOT NULL
);
#修改table中某一col為不重複
ALTER TABLE xx ADD UNIQUE xx;
#修改table中每一col為主鍵
ALTER TABLE table_name
ADD PRIMARY KEY xx;
#修改table中每一col為外來鍵
ALTER TABLE table_name1
ADD CONSTRAINT FK_Per  
FOREIGN KEY (PersonID) REFERENCES table_name1;
＃新增col index
CREATE UNIQUE INDEX index_name
ON table_name (col1, _col2, ...);
```

## 刪除資料表
```SQL
#刪除table
DROP table xx;
#刪除現有tabe的col
ALTER TABLE x DROP COLUMN col
#刪除table中某一col為不重複的條件
ALTER TABLE xx DROP INDEX xx;
#刪除table中某一col為主鍵
ALTER TABLE talbe_name  
DROP CONSTRAINT xx;
#刪除table中某一col為主鍵
ALTER TABLE Orders  
DROP CONSTRAINT FK_PersonOrder;
#刪除table中某一col為預設
ALTER TABLE table_name  
ALTER COLUMN xx DROP DEFAULT;
#刪除col index
DROP INDEX table_name.index_name;
```
