# **Data Types in Python**

## **What are Data Types?**  
A data type defines the kind of value a variable can hold. Python has several built-in data types, which are dynamically assigned when a variable is created.

## **1. Numeric Types**  
These are used to store numbers.

| Data Type | Example | Description |
|-----------|---------|-------------|
| **int** | `x = 10` | Whole numbers (positive or negative) |
| **float** | `y = 3.14` | Decimal numbers |
| **complex** | `z = 2 + 3j` | Complex numbers |

### **Examples:**
```python
x = 100         # Integer
y = 3.14        # Float
z = 2 + 3j      # Complex Number

print(type(x))  # Output: <class 'int'>
print(type(y))  # Output: <class 'float'>
print(type(z))  # Output: <class 'complex'>
```

---

## **2. Boolean Type**  
A Boolean (`bool`) can hold only two values: **True** or **False**.

### **Example:**
```python
is_python_fun = True
is_raining = False

print(type(is_python_fun))  # Output: <class 'bool'>
print(5 > 3)  # Output: True
print(5 == 10)  # Output: False
```

---

## **3. String Type**  
A **string** (`str`) is a sequence of characters enclosed in **single** or **double quotes**.

### **Example:**
```python
name = "Alice"
message = 'Hello, World!'

print(type(name))  # Output: <class 'str'>
print(name[0])     # Output: A (Strings are indexed)
print(name[1:4])   # Output: lic (Slicing)
print(len(name))   # Output: 5 (String length)
```

---

## **4. Sequence Types**  
### **4.1 List (`list`)**  
A **list** is an ordered, mutable (changeable) collection of items.

#### **Example:**
```python
fruits = ["Apple", "Banana", "Cherry"]
print(type(fruits))  # Output: <class 'list'>

fruits.append("Mango")  # Add an item
print(fruits)  # Output: ['Apple', 'Banana', 'Cherry', 'Mango']

print(fruits[1])  # Output: Banana (Indexing)
fruits[1] = "Blueberry"  # Modify an element
print(fruits)  # Output: ['Apple', 'Blueberry', 'Cherry', 'Mango']
```

---

### **4.2 Tuple (`tuple`)**  
A **tuple** is similar to a list but **immutable** (cannot be changed after creation).

#### **Example:**
```python
coordinates = (10, 20, 30)
print(type(coordinates))  # Output: <class 'tuple'>

print(coordinates[1])  # Output: 20
# coordinates[1] = 50  # This will cause an error because tuples are immutable
```

---

### **4.3 Range (`range`)**  
A **range** generates a sequence of numbers.

#### **Example:**
```python
numbers = range(5)  # Creates a sequence: 0, 1, 2, 3, 4
print(list(numbers))  # Output: [0, 1, 2, 3, 4]
```

---

## **5. Set Types**  
### **5.1 Set (`set`)**  
A **set** is an unordered collection of unique items.

#### **Example:**
```python
my_set = {1, 2, 3, 4, 4, 5}
print(type(my_set))  # Output: <class 'set'>
print(my_set)  # Output: {1, 2, 3, 4, 5} (Duplicates are removed)

my_set.add(6)  # Adding an element
print(my_set)  # Output: {1, 2, 3, 4, 5, 6}
```

---

### **5.2 Frozen Set (`frozenset`)**  
A **frozenset** is an immutable version of a set.

#### **Example:**
```python
frozen = frozenset([1, 2, 3, 4])
# frozen.add(5)  # This will cause an error because frozensets are immutable
print(frozen)  # Output: frozenset({1, 2, 3, 4})
```

---

## **6. Dictionary Type (`dict`)**  
A **dictionary** is an unordered collection of key-value pairs.

#### **Example:**
```python
person = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}

print(type(person))  # Output: <class 'dict'>

print(person["name"])  # Output: Alice
person["age"] = 30  # Modify value
print(person)  # Output: {'name': 'Alice', 'age': 30, 'city': 'New York'}
```

---

## **7. None Type (`NoneType`)**  
`None` represents the absence of a value.

#### **Example:**
```python
result = None
print(type(result))  # Output: <class 'NoneType'>
```

---

# **Type Conversion (Casting)**
Python allows converting one data type to another.

### **Example:**
```python
x = 10
y = float(x)  # Convert int to float
print(y)  # Output: 10.0

z = str(x)  # Convert int to string
print(z)  # Output: '10'

a = list("hello")  # Convert string to list
print(a)  # Output: ['h', 'e', 'l', 'l', 'o']
```

---

# **Summary Table**
| Data Type | Description | Example |
|-----------|-------------|---------|
| `int` | Integer numbers | `x = 10` |
| `float` | Decimal numbers | `y = 3.14` |
| `complex` | Complex numbers | `z = 2 + 3j` |
| `bool` | Boolean values | `is_valid = True` |
| `str` | Text data | `name = "Alice"` |
| `list` | Ordered, mutable collection | `fruits = ["Apple", "Banana"]` |
| `tuple` | Ordered, immutable collection | `coords = (10, 20)` |
| `range` | Sequence of numbers | `range(5)` |
| `set` | Unordered collection of unique items | `s = {1, 2, 3}` |
| `frozenset` | Immutable set | `fs = frozenset({1, 2, 3})` |
| `dict` | Key-value pairs | `person = {"name": "Alice"}` |
| `NoneType` | Represents no value | `result = None` |
