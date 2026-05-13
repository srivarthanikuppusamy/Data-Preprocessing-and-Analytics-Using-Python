
---

# Experiment 02 README

```md
# Experiment 02: Prime Number Detection

## Aim
To display prime numbers between 1 and 100 using a function.

## Program
```python
def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

for number in range(1, 101):
    if is_prime(number):
        print(number, end=" ")
