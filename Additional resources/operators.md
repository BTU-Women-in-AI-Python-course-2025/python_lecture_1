# **Operators in Python**  

## **What are Operators?**  
Operators are special symbols in Python that perform operations on variables and values.  

---

## **1. Arithmetic Operators**  
These operators perform mathematical operations.  

| Operator | Description | Example |
|----------|-------------|---------|
| `+` | Addition | `5 + 3 = 8` |
| `-` | Subtraction | `10 - 2 = 8` |
| `*` | Multiplication | `4 * 3 = 12` |
| `/` | Division (float) | `10 / 2 = 5.0` |
| `//` | Floor Division | `10 // 3 = 3` |
| `%` | Modulus (remainder) | `10 % 3 = 1` |
| `**` | Exponentiation | `2 ** 3 = 8` |

### **Example:**
```python
a = 10
b = 3

print(a + b)  # Output: 13
print(a - b)  # Output: 7
print(a * b)  # Output: 30
print(a / b)  # Output: 3.333...
print(a // b) # Output: 3
print(a % b)  # Output: 1
print(a ** b) # Output: 1000
```

---

## **2. Comparison (Relational) Operators**  
These operators compare values and return **True** or **False**.  

| Operator | Description | Example |
|----------|-------------|---------|
| `==` | Equal to | `5 == 5` → `True` |
| `!=` | Not equal to | `5 != 3` → `True` |
| `>` | Greater than | `10 > 5` → `True` |
| `<` | Less than | `3 < 8` → `True` |
| `>=` | Greater than or equal to | `5 >= 5` → `True` |
| `<=` | Less than or equal to | `3 <= 5` → `True` |

### **Example:**
```python
x = 10
y = 5

print(x == y)  # False
print(x != y)  # True
print(x > y)   # True
print(x < y)   # False
print(x >= y)  # True
print(x <= y)  # False
```

---

## **3. Logical Operators**  
These operators are used to combine multiple conditions.  

| Operator | Description | Example |
|----------|-------------|---------|
| `and` | Returns `True` if both conditions are `True` | `(5 > 3 and 10 > 5) → True` |
| `or` | Returns `True` if at least one condition is `True` | `(5 > 3 or 10 < 5) → True` |
| `not` | Reverses the condition | `not(5 > 3) → False` |

### **Example:**
```python
a = True
b = False

print(a and b)  # Output: False
print(a or b)   # Output: True
print(not a)    # Output: False
```

---

## **4. Assignment Operators**  
These operators assign values to variables.  

| Operator | Example | Equivalent To |
|----------|---------|--------------|
| `=`  | `x = 5` | Assign 5 to x |
| `+=` | `x += 3` | `x = x + 3` |
| `-=` | `x -= 2` | `x = x - 2` |
| `*=` | `x *= 4` | `x = x * 4` |
| `/=` | `x /= 2` | `x = x / 2` |
| `//=` | `x //= 3` | `x = x // 3` |
| `%=` | `x %= 2` | `x = x % 2` |
| `**=` | `x **= 2` | `x = x ** 2` |

### **Example:**
```python
x = 10
x += 5  # Same as x = x + 5
print(x)  # Output: 15
```

---

## **5. Identity Operators**  
These check if two variables refer to the **same object in memory**.  

| Operator | Description | Example |
|----------|-------------|---------|
| `is` | Returns `True` if both variables point to the same object | `x is y` |
| `is not` | Returns `True` if both variables do not point to the same object | `x is not y` |

### **Example:**
```python
x = [1, 2, 3]
y = x  # y points to the same object as x
z = [1, 2, 3]  # z is a different object

print(x is y)   # Output: True
print(x is z)   # Output: False
print(x == z)   # Output: True (Because their values are the same)
```

---

## **6. Membership Operators**  
These check for the presence of a value in a sequence.  

| Operator | Description | Example |
|----------|-------------|---------|
| `in` | Returns `True` if a value exists in a sequence | `'a' in 'apple'` |
| `not in` | Returns `True` if a value does not exist in a sequence | `'x' not in 'apple'` |

### **Example:**
```python
fruits = ["apple", "banana", "cherry"]

print("banana" in fruits)  # Output: True
print("grape" not in fruits)  # Output: True
```

---

# **Summary Table**
| Operator Type | Operators |
|--------------|----------|
| **Arithmetic** | `+`, `-`, `*`, `/`, `//`, `%`, `**` |
| **Comparison** | `==`, `!=`, `>`, `<`, `>=`, `<=` |
| **Logical** | `and`, `or`, `not` |
| **Assignment** | `=`, `+=`, `-=`, `*=`, `/=`, `//=`, `%=`, `**=` |
| **Identity** | `is`, `is not` |
| **Membership** | `in`, `not in` |
