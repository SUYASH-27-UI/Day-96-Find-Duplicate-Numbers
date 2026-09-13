# Day-96-Find-Duplicate-Numbers
# Python Day 96 - Find Duplicate Numbers

This program finds the duplicate numbers in a list.

## Example

Input:

```text
[10, 20, 10, 30, 20, 40, 50, 30]
```

Output:

```text
Duplicate numbers: [10, 20, 30]
```

## Concepts Used

* Lists
* `for` loop
* `count()` method
* `not in` operator
* `append()` method
* `if` condition

## How It Works

1. Store numbers in a list.
2. Use a `for` loop to check each number.
3. Use `count()` to check how many times a number appears.
4. If the number appears more than once, it is a duplicate.
5. Use `not in` to make sure the duplicate is added only once.
6. Use `append()` to store the duplicate number.

## Python Code

```python
numbers = [10, 20, 10, 30, 20, 40, 50, 30]

duplicates = []

for number in numbers:
    if numbers.count(number) > 1 and number not in duplicates:
        duplicates.append(number)

print("Duplicate numbers:", duplicates)
```

## Output

```text
Duplicate numbers: [10, 20, 30]
```
