###### 資料標準化
```Python
#參數可修改
from sklearn.model_select
scaler = MinMaxScaler(feature_range=(0, 1)).fit(df) 
df_scaled = scaler.transform(df)
```

###### 拆分資料
```Python
from sklearn.model_selection import train_test_split
train_X, val_X, train_y, val_y = train_test_split(X, y, train_size=0.8, test_size=0.2, random_state = 0)
```

###### 使用統計值填補缺失值
```Python
from sklearn.impute import SimpleImputer
#strategy參數可填mean, constant, median, most_frequent
#strategy = 'constant'將和fill_value搭配使用
my_imputer = SimpleImputer(strategy=)
imputed_X_train = my_imputer.fit_transform(x)
```

###### 將數據按等地編號
```Python
from sklearn.preprocessing import OrdinalEncoder
ordinal_encoder = OrdinalEncoder()

label_X_train[object_cols] = ordinal_encoder.fit_transform(X_train[object_cols])
label_X_valid[object_cols] = ordinal_encoder.transform(X_valid[object_cols])
```

###### One-Hot(將非數值col欄位更改為vector)
```Python
from sklearn.preprocessing import OneHotEncoder 
encoder = OneHotEncoder() 
encoder.fit(X) 
X_encoded = encoder.transform(X)
```

###### 交差驗證
```Python
form sklearn.model_selection import cross_val_score

#第一個參數填使用模型,cv切成幾等分,scoring參數填寫評估模型的指標
scores = cross_val_score(estimator  , test_X, test_y, cv = x, scoring = '')
```

###### Grid Serach
```Python
form sklear.model_select import GridSearchCV, cross_val_score
```