
## Simple Linear Regression

### $y=ax+b$
$a$ is slope
$b$ is intercept 
$x$ is called feature
$y$ is called label
```Python
from sklearn.linear_model import LinearRegression

lm = LinearRegression()
X = x
y =x
lm.fit(X, y)
```

## Multivariable Regression
### $y=a_1x_1+a_2x_2+a_3x_3+...a_nx_n+b$
$a_1$ is coefficient of $x_1$
$a_2$ is coefficient of $x_2$
$b$ is intercept 



## Polynomial Regression

### $y = a_1x_1^n+a_2x_1^{n-1}+a_3x_1^{n-2}+...a_nx_1+b$
### $y = b+a_1x_1+a_2x_2+a_3x_1x_2+a_4x_1^2+a_5x_2^2+...$

```Python
from sklearn.preprocessing import PolynminalFeatures

pr = PloynminalFeatures(degree = x)
pr.fit_transform()

```


### Ridge Regression
```Python
form sklearn.linear_model imoprt Ridge
#alpha值
RidgeModel = Ridge(alpha = )
RidgeModel.fit()

```

## Logistic Regression


## Classification

$Confusion\ Martix$
|                 | Actual True         | Actual False        |     
| --------------- | ------------------- | ------------------- |
| Predicted Ture  | True Positive (TP)  | False Positive (FP) |    
| Predicted False | True Negative (TN)  ) | False Negative (FN)|   

$Accuracy = \frac{TP+TN}{ALL}$
$Percision= \frac{TP}{TP+FP}$
$Recall = \frac{TP}{TP+FN}$
$F1 Score = \frac{2*Accuary*Percisoin}{Accuary+Percisoin}$
$AUC$

 
## Clustering

K-maens


## Dimension reduction

### Principal Component Analysis(PCA)
PCA 是一種降維的機器學習算法，他可以把高維度的數據壓縮成低維度
```Python
from sklearn import PCA
#n_components 選擇要保留的特徵個數
pca = PCA(n_components=xx)
pca.fit()

```

