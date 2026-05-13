
---

# Experiment 05 README

```md
# Experiment 05: Outlier Detection using Z-Score

## Aim
To detect and remove outliers using Z-score method.

## Program
```python
import numpy as np
from scipy import stats

data = np.array([10,12,11,13,12,100,11,12])

z = np.abs(stats.zscore(data))
cleaned = data[z < 2.5]

print(cleaned)
