### Statistics

P-value < 0.001 Strong
P-value < 0.05 Moderate
P-value < 0.1 Weak
P-value >0.1 No realtion

```Python
from scipy.stats import pearsonr

corr, p_value = pearsonr(df['x'], df['x'])
```

### Chi-square Test

 $\sum_{i=1}^n\frac{(O_i-E_i)^2}{E_i}$~$\chi^2$
$O_i$ is observe value
$E_i$ is except value
$df = n-1$ is degree of freedom
查表看自由度$aplha$值通常是0.05 如果$\chi^2$ > 查出來的值拒絕$H_0$

```Python
from sci.py
scipy.stats.chi2()
```


### Loss Funtion

##### MSE/SSD
$MSE(Mean\ Squared\ Error) =\frac{\sum(y_i-\hat{y})^2}{n}$
$RMSE=\sqrt{MSE}$

```Python
from sklearn.metrics import mean_squared_error

perdict = model.predict(X)
mean_squared_error(Y, perdict)
```

###### MAE/SAD

$cost = \sum \mid estimate-actual\mid$
```Python
from sklearn import mean_absloute_error

perdict = model.predict(X)
mean_absloute_error(Y, perdict)
```

$R^2= 1-\sum\frac{(y_i-\hat{y})^2}{(y_i-\bar{y})^2}$
```Python
from sklear.linear_model import LinearRegression

lm = LinearRegression()
R_2 = lm.score(X, y)
```