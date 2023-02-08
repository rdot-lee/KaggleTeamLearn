## MSE/SSD

 $cost = \sum(estiamte-actual)^2$

```Python
def mse(estimate ,actual):
	return numpy.sum((estimate-actual)**2)
```

## MAE/SAD

$cost = \sum \mid estimate-actual\mid$
```Python
from sklearn import mean_absloute_error

perdict = model.predict(X)
mean_absloute_error(Y, perdict)

def mae(estimate, actual):
	return numpy.sum(abs(estimate-actual))

```

