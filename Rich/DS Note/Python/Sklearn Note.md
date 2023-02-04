
###### 把data標準化, 參數0,1可修改
```Python
from sklearn.model_select
scaler = MinMaxScaler(feature_range=(0, 1)).fit(df) 
df_scaled = scaler.transform(df)
```

###### 拆分資料
```Python
from sklearn.model_selection import train_test_split
train_X, val_X, train_y, val_y = train_test_split(X, y, train_size=0.8, test_size=0.2, random_state = 0)
```

###### 決策數
```Python
from sklearn.tree import DecisionTreeRegressor
from sklearn import tree

model = DecisionTreeRegressor(random_state=1)
```

###### 隨機叢林
```Python
from sklearn.ensemble import RandomForestRegressor
model = RandomForestRegressor(n_estimators=x, random_state=0)
```

衡量指標
```Python
from sklearn.metrics import mean_absolute_error
meam_absoulte_error(x, xx)
```

使用統計值填補缺失值
```Python
from sklearn.impute import SimpleImputer
my_imputer = SimpleImputer()
imputed_X_train = pd.DataFrame(my_imputer.fit_transform(X_train))

imputed_X_valid = pd.DataFrame(my_imputer.transform(X_valid))
```