# Experiment 1: Sum, Average, and Product of Three Numbers

## Aim
To write a Python program to compute the sum, average, and product of three user-input numbers.

---

## Program

```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
num3 = int(input("Enter third number: "))

sum = num1 + num2 + num3
average = sum / 3
product = num1 * num2 * num3

print("Sum =", sum)
print("Average =", average)
print("Product =", product)
