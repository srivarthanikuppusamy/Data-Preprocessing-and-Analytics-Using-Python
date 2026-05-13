
---

# Experiment 04 README

```md
# Experiment 04: JSON to CSV Conversion

## Aim
To convert JSON data into CSV format using pandas.

## Program
```python
import pandas as pd

df = pd.DataFrame(json_file)
df.to_csv("data.csv")

print("CSV file created successfully")
