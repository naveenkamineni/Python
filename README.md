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
