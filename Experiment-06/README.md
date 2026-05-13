
---

# Experiment 06 README

```md
# Experiment 06: Train-Test Split and Label Encoding

## Aim
To encode categorical data and split dataset into training and testing sets.

## Program
```python
import pandas as pd
from sklearn.preprocessing import LabelEncoder
from sklearn.model_selection import train_test_split

df = pd.DataFrame({
    "age":[34,22,21,34,54],
    "genre":["rock","scify","scify","rock","classical"]
})

le = LabelEncoder()
df["genre"] = le.fit_transform(df["genre"])

X = df[["age"]]
y = df["genre"]

train_test_split(X, y, test_size=0.2)
