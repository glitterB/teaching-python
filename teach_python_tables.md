
# 🐍 Teaching Python using Multiplication Tables
I have always wondered how I would teach Python.

This guide walks you through how to teach core Python concepts using a relatable example: **Printing Multiplication Tables**.

---

## ✅ Part 1: The Basics

### 1. Numbers and Texts

We want to print the multiplication table of 2. We can either print it in the number format or we can 

```
2
4
6
8
10
```

---

### 2. Use `print()`

```python
print(2)
print(4)
print(6)
print(8)
print(10)
```

---

### 3. Use a Loop

```python
for i in range(2, 11, 2):
    print(i)
```

**Output:**
```
2
4
6
8
10
```

---

### 4. Create a Function

```python
def table(n):
    for i in range(1, 11):
        print(n * i)
```

**Calling the function:**
```python
table(5)
```

**Output:**
```
5
10
15
20
25
30
35
40
45
50
```

---

## ➕ Add More Concepts

### 1. Conditionals

```python
def table(n):
    if n <= 0:
        print("Please enter a positive number.")
        return
    for i in range(1, 11):
        print(f"{n} x {i} = {n*i}")
```

---

### 2. Taking User Input

```python
num = int(input("Enter a number to print its table: "))
table(num)
```

---

### 3. While Loop

```python
while True:
    entry = input("Enter a number (or type 'exit' to quit): ")
    if entry.lower() == 'exit':
        break
    if entry.isdigit():
        table(int(entry))
    else:
        print("Please enter a valid number.")
```

---

### 4. Lists

```python
tables = [2, 3, 5]
for t in tables:
    table(t)
    print("-" * 20)
```

---

### 5. Dictionaries

```python
def get_table(n):
    result = {}
    for i in range(1, 11):
        result[i] = n * i
    return result

my_table = get_table(4)
print(my_table)
```

---

### 6. List Comprehension

```python
table_of_7 = [7 * i for i in range(1, 11)]
print(table_of_7)
```

---

### 7. Modules and Random Quiz

```python
import random

n = random.randint(1, 10)
i = random.randint(1, 10)
answer = int(input(f"What is {n} x {i}? "))
if answer == n * i:
    print("Correct!")
else:
    print(f"Nope! The answer is {n * i}")
```

---

### 8. Error Handling

```python
try:
    n = int(input("Enter a number: "))
    table(n)
except ValueError:
    print("That was not a valid number.")
```

---

## 🧠 Summary Table

| Concept        | Example                     | Skill              |
|----------------|-----------------------------|---------------------|
| `print()`      | `print(2)`                  | Output              |
| `for` loop     | `for i in range(1,11)`      | Repetition          |
| `def`          | `def table(n):`             | Function            |
| `if`           | `if n <= 0:`                | Decision Making     |
| `input()`      | `int(input(...))`           | User Interaction    |
| `while`        | `while True:`               | Looping             |
| `list`         | `[2,3,5]`                   | Grouping Data       |
| `dict`         | `{1:2, 2:4}`                | Key-Value Structure |
| `try-except`   | `try: int(input())`         | Error Handling      |
| `import`       | `import random`             | Using Libraries     |

---

## ✅ What’s Next?
- File I/O: Save tables to `.txt`
- GUI: Build with `tkinter`
- Classes: Wrap logic in objects

---

Happy Teaching! 🎓🐍
