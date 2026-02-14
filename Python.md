# Python Basics
> Extra resources for learning Python

[Python tutorial](https://www.geeksforgeeks.org/python/python-programming-language-tutorial/)

[Bro Code python tutorial](https://www.youtube.com/watch?v=ix9cRaBkVe0&t=41351s)

[Bro Code NumPy tutorial](https://www.youtube.com/watch?v=VXU4LSAQDSc&t=159s)

[Bro Code Matplotlib tutorial](https://www.youtube.com/watch?v=c9vhHUGdav0)

[Bro Code Pandas tutorial](https://www.youtube.com/watch?v=VXtjG_GzO7Q&t=1s)


## Table of Contents
1. [Variables & Data Types](#-1-variables--data-types)
2. [Operators](#-2-operators)
3. [Control Flow](#-3-control-flow)
4. [Functions](#-4-functions)
5. [Data Structures](#-5-data-structures)
6. [Common Built-ins](#-6-common-built-ins)
7. [File Handling](#-7-file-handling)
8. [Exceptions](#-8-exceptions)
9. [Classes (OOP)](#-9-classes-oop)
10. [Useful Tips](#-10-useful-tips)
11. [Quick Reference Links](#-11-quick-reference-links)

---

## 1. Variables & Data Types

```python
# Basic types
x = 5              # int
y = 3.14           # float
name = "Alice"     # str
is_active = True   # bool

# Multiple assignment
a, b, c = 1, 2, 3
```

| Type | Example | Description |
|------|----------|-------------|
| `int` | `5` | Whole numbers |
| `float` | `3.14` | Decimal numbers |
| `str` | `"Hello"` | Text data |
| `bool` | `True` / `False` | Logical values |
| `list` | `[1,2,3]` | Ordered, changeable |
| `tuple` | `(1,2,3)` | Ordered, unchangeable |
| `set` | `{1,2,3}` | Unordered, unique items |
| `dict` | `{"a":1,"b":2}` | Key-value pairs |

---

## 2. Operators

| Type | Example | Description |
|------|----------|-------------|
| Arithmetic | `+ - * / % ** //` | Basic math |
| Comparison | `== != > < >= <=` | Compare values |
| Logical | `and or not` | Combine conditions |
| Assignment | `= += -= *= /=` | Update variables |

---

## 3. Control Flow

```python
if x > 0:
    print("Positive")
elif x == 0:
    print("Zero")
else:
    print("Negative")
```

```python
for i in range(5):
    print(i)  # 0–4

while x < 10:
    x += 1
```

---

## 4. Functions

```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
```

With default parameters:
```python
def add(a, b=1):
    return a + b
```

---

## 5. Data Structures

### Lists
```python
nums = [1, 2, 3]
nums.append(4)
nums.remove(2)
print(nums[0])  # 1
```

### Tuples
```python
point = (10, 20)
x, y = point
```

### Sets
```python
unique = {1, 2, 3}
unique.add(4)
```

### Dictionaries
```python
person = {"name": "Alice", "age": 25}
print(person["name"])
person["age"] = 26
```

---

## 6. Common Built-ins

```python
len(), type(), range(), input(), print(), int(), str(), list(), sum(), max(), min()
```

---

## 7. File Handling

```python
with open("file.txt", "r") as f:
    data = f.read()

with open("output.txt", "w") as f:
    f.write("Hello file!")
```

---

## 8. Exceptions

```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
finally:
    print("Done")
```

---

## 9. Classes (OOP)

```python
class Dog:
    def __init__(self, name):
        self.name = name

    def bark(self):
        print(f"{self.name} says woof!")

dog = Dog("Rex")
dog.bark()
```

---

## 10. Useful Tips

- Use `pip install package` to install external modules  
- Use **f-strings** for cleaner output → `f"Hello {name}!"`  
- Use **list comprehensions** → `[x**2 for x in range(5)]`  
- Check attributes → `dir(object)`  
- Get documentation → `help(object)`  
- Use `_` in loops if you don’t need the variable:
  ```python
  for _ in range(3):
      print("Hi!")
  ```

---

## 11. Quick Reference Links

- [Python Official Docs](https://docs.python.org/3/)
- [Real Python Tutorials](https://realpython.com/)
- [Learn X in Y Minutes – Python](https://learnxinyminutes.com/docs/python/)

---

### Contribute
Found something missing or want to improve this guide?  
Fork the repo and open a pull request — contributions are always welcome!
