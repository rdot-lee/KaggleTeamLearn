### 下載套件
```R
install.packages("xx")
```

引入套件
```R
libarary("xx")
```

查看數據集
```R
#查看所有數據
View(x)
#查看n筆數據, x是數據集的名字,n是幾筆資料
head(x, n)
```

使用ggplot繪圖
```R
libarary(ggplot2)
ggplot(data=xx,
	   aes=(x=,y=),
	   geom_layer()=x
)
```