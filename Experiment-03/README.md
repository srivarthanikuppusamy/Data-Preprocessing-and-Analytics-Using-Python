
---

# Experiment 03 README

```md
# Experiment 03: Data Indexing, Sorting and Filtering

## Aim
To perform indexing, sorting and filtering using pandas.

## Program
```python
import pandas as pd

arr = {
    "name": ["alice","bob","charlie"],
    "age": [25,30,35],
    "salary": [50000,60000,70000]
}

df = pd.DataFrame(arr)

df["salary"]
df.sort_values("name")
df[df["salary"] >= 60000]
