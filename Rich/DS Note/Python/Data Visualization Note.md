###### 設定圖的大小
```Python
fig = plt.figure(figsize=(width, height))
```

###### 設定圖的x, y, title
```Python
#調整字體, fontsize
plt.xlabel('xx', fontsize = 14)
plt.ylabel('xx')
plt.title('xx')
```
###### 繪製折線圖
```Python
sns.lineplot(data=xx)
#可以設置小圖標
sns.lineplot(data=xx, label='')
```
###### plot類型
```Python
#kind參數有以下
#折線圖 line
#區域圖 area
#直方圖 histogram
#長條圖 bar
#圓餅圖 pie
#盒狀圖 box
#散點圖 scatter
xx.plt(kind='')
```

Seaborm
```Python
#畫出regression line
sns.regplot(x = 'x', y= 'x', data = df)

#箱型圖
xx.boxplot(column='x')
sns.boxplot(x='', y='', data=x)
#畫出曲線分布
sns.distplot(xx)
#畫出散點圖
sns.reglot(x='xx', y='xx',data=xx, scatter=True)
df.plot.scatter(title='x', x='', y='')
#畫出散點圖矩陣
sns.pairplot(df)
#畫熱力圖
sns.heatmap('x', 'x')


#畫出特定欄位的圖
df = xx[['x', 'x', 'x']
df.plot()
#設定x座標字體傾斜角度
plt.xticks(rotation=幾度)
```

###### 殘差圖
```Python
#如果圖形存在U or V代表不適用linear關係
import seabron as sns

sns.resiplot(df['feature'], df['label'])
```

###### 分布圖
```Python
import seaborn as asns
import matplotlib.pyplot as plt 

sns.distplot(df[''], hist = False)
plt.show()
```

