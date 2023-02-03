###### 設定圖的x, y, title
```Python
plt.xlabel('xx')
plt.ylabel('xx')
plt.title('xx')
```
###### plot類型
```Python
#kind參數有以下
#line, area, 
# Histograms
xx.plt(kind=)''
```

```Python
#折線圖
plt.plot(x, y)
#長條圖
plt.bar(x, y)#x是數字
#也可以這樣xx是cloumn name
xx.plot(kind = 'bar')
#直方圖
plt.hist(x, y)#x是有組距
#圓餅圖
plt.pie(x)
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
#用sklearn把data標準化參數0,1可修改
scaler = MinMaxScaler(feature_range=(0, 1)).fit(df) 
df_scaled = scaler.transform(df)