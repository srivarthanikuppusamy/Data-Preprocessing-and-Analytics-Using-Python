
---

# Experiment 09 README

```md
# Experiment 09: Linear Regression

## Aim
To predict house prices using linear regression.

## Program
```python
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

df = pd.read_csv("data.csv")

X = df[["sqft_living"]]
y = df["price"]

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)

model = LinearRegression()
model.fit(X_train, y_train)

model.predict(X_test)
