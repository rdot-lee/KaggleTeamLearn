###### 使用python連接資料庫
```SQL
import pymysql

db_settings = {

"host": "localhost",

"port": 3306,

"user": "root",

"db": "new_schema",

"charset": "utf8"

}

try:

# 建立Connection物件

conn = pymysql.connect(**db_settings)

except Exception as ex:

print("Connection Error:", ex)
```