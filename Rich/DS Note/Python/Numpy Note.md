###### 切一個interval
```Python
#a是左端點, b是右端點, num是總共幾個點
np.linspace(a, b ,num=x)
```

###### 算出該list or array有幾個元素
```Python
xx.size()
```

###### 矩陣乘法
```Python
x = np.array()
y = np.array()

np.dot(x, y)
```

###### 讀取txt並存成np.array
```Python
#txt如果有標題會報錯, 需要跳過title, 如果是cvs檔需加delimiter
np.loadtxt('x', skiprows=1, delimiter = ',')

```