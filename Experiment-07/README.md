
---

# Experiment 07 README

```md
# Experiment 07: Data Visualization

## Aim
To visualize data using scatter plot and pair plot.

## Program
```python
import seaborn as sns
import matplotlib.pyplot as plt

df = sns.load_dataset("iris")

plt.scatter(df["sepal_length"], df["petal_length"])
plt.show()

sns.pairplot(df, hue="species")
plt.show()
