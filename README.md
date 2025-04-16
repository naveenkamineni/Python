# Python

Here's a **Python Fundamentals Cheat Sheet** — perfect for quick revision:

---

### **1. Variables & Data Types**
```python
x = 10         # int
name = "Naveen"  # str
pi = 3.14      # float
is_ready = True # bool
```

---

### **2. Strings**
```python
msg = "Hello"
print(msg.upper())   # HELLO
print(msg[0:3])      # Hel
```

---

### **3. Collections**
- **List**: Ordered, mutable
```python
fruits = ['apple', 'banana']
```

- **Tuple**: Ordered, immutable
```python
coordinates = (10, 20)
```

- **Set**: Unordered, unique
```python
nums = {1, 2, 3}
```

- **Dictionary**: Key-value pairs
```python
person = {"name": "Naveen", "age": 25}
```

---

### **4. Conditional Statements**
```python
if age > 18:
    print("Adult")
elif age == 18:
    print("Just 18")
else:
    print("Minor")
```

---

### **5. Loops**
```python
for i in range(5):
    print(i)

while x > 0:
    x -= 1
```

---

### **6. Functions**
```python
def greet(name):
    return f"Hello {name}"
```

---

### **7. OOP (Classes and Objects)**
```python
class Student:
    def __init__(self, name):
        self.name = name

    def greet(self):
        return f"Hi, I'm {self.name}"

s = Student("Naveen")
print(s.greet())
```

---

### **8. File Handling**
```python
with open("file.txt", "r") as f:
    content = f.read()
```

---

### **9. Exception Handling**
```python
try:
    x = 10 / 0
except ZeroDivisionError:
    print("Error!")
```

---

### **10. List Comprehension**
```python
squares = [x**2 for x in range(5)]
```

---

### **11. Lambda Functions**
```python
add = lambda a, b: a + b
```

---

### **12. JSON Handling**
```python
import json
data = json.loads('{"key": "value"}')
```

---

### **13. `*args` and `**kwargs`**
```python
def demo(*args, **kwargs):
    print(args)
    print(kwargs)
```

---

### **14. Virtual Environment (Terminal)**
```bash
python -m venv env
source env/bin/activate  # macOS/Linux
env\Scripts\activate     # Windows
```

---

Want this as a downloadable PDF or printable version? I can make one for you.


Perfect! Here’s your **Python Cheatcodes** for those advanced (but super useful) concepts — explained simply and ready to use:

---

## 🔷 **1. Working with JSON**

### 🔹 Parse JSON (string → Python)
```python
import json

json_data = '{"name": "Naveen", "age": 25}'
python_dict = json.loads(json_data)
print(python_dict['name'])  # Naveen
```

### 🔹 Convert Python → JSON
```python
data = {'name': 'Naveen', 'course': 'Data Science'}
json_string = json.dumps(data)
print(json_string)
```

### 🔹 Read from JSON file
```python
with open('data.json', 'r') as f:
    data = json.load(f)
```

### 🔹 Write to JSON file
```python
with open('data.json', 'w') as f:
    json.dump(data, f)
```

---

## 🔷 **2. `*args` and `**kwargs`**

### 🔹 `*args`: accepts **multiple positional arguments**
```python
def add(*args):
    return sum(args)

print(add(1, 2, 3))  # 6
```

### 🔹 `**kwargs`: accepts **multiple keyword arguments**
```python
def greet(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

greet(name='Naveen', age=25)
```

### 🔹 Combine both
```python
def demo(*args, **kwargs):
    print("Args:", args)
    print("Kwargs:", kwargs)

demo(1, 2, name='Naveen', country='India')
```

---

## 🔷 **3. Iterators & Generators**

### 🔹 Iterator
```python
nums = [1, 2, 3]
it = iter(nums)
print(next(it))  # 1
print(next(it))  # 2
```

### 🔹 Generator Function
```python
def countdown(n):
    while n > 0:
        yield n
        n -= 1

for num in countdown(3):
    print(num)
```

✅ Generators are **memory-efficient** and great for big data or pipelines.

---

## 🔷 **4. Decorators**

### 🔹 Basic Decorator
```python
def decorator(func):
    def wrapper():
        print("Before function")
        func()
        print("After function")
    return wrapper

@decorator
def say_hello():
    print("Hello!")

say_hello()
```

---

## 🔷 **5. List Comprehensions Cheatcodes**

### 🔹 Basic
```python
squares = [x**2 for x in range(5)]
```

### 🔹 With condition
```python
evens = [x for x in range(10) if x % 2 == 0]
```

### 🔹 Nested
```python
matrix = [[1,2],[3,4]]
flat = [item for row in matrix for item in row]
```

### 🔹 Using function
```python
def square(x): return x*x
result = [square(x) for x in range(5)]
```

---

Want this bundled into a **downloadable PDF or code notebook (.ipynb)** for practice? I can prep that for you!
