
---

# Experiment 08 README

```md
# Experiment 08: Data Profiling and Correlation

## Aim
To generate data profiling report and analyze correlations.

## Program
```python
import pandas as pd
import seaborn as sns
from ydata_profiling import ProfileReport

df = pd.read_csv("dataset.csv")

df.corr()
sns.heatmap(df.corr(), annot=True)

report = ProfileReport(df)
report
