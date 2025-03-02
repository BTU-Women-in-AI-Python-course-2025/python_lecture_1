# **Variables in Python**

## **What is a Variable?**
A variable in Python is a container used to store data. It holds a value that can be changed during the execution of a program.

### **Declaring Variables**
Python does not require explicit declaration of variables. A variable is created the moment a value is assigned to it.

#### **Example:**
```python
x = 10       # Integer
y = 3.14     # Float
name = "Alice"  # String
is_valid = True  # Boolean
```

## **Variable Naming Rules**
1. A variable name must start with a **letter** (a-z, A-Z) or an **underscore (_)**.
2. The name can contain letters, digits (0-9), and underscores but **cannot start with a digit**.
3. Variable names are **case-sensitive** (`name` and `Name` are different).
4. Reserved words (keywords) **cannot** be used as variable names.

#### **Valid Variable Names:**
```python
age = 25
_name = "John"
my_var = "Python"
```

#### **Invalid Variable Names:**
```python
2name = "Error"  # Starts with a number (Invalid)
my-var = 10      # Hyphen (-) is not allowed (Invalid)
class = "Python" # 'class' is a reserved keyword (Invalid)
```

## **Multiple Assignments**
Python allows multiple variable assignments in a single line.

#### **Example:**
```python
a, b, c = 1, 2, 3  # Assigns 1 to a, 2 to b, and 3 to c
x = y = z = 100    # Assigns 100 to x, y, and z
```

## **Variable Types in Python**
Python variables are **dynamically typed**, meaning you don’t need to specify the type explicitly.

### **Basic Data Types:**
| Data Type | Example |
|-----------|---------|
| Integer (`int`) | `x = 10` |
| Float (`float`) | `y = 3.14` |
| String (`str`) | `name = "Alice"` |
| Boolean (`bool`) | `is_valid = True` |

#### **Example with Type Checking:**
```python
x = 10
y = 3.5
name = "Python"
is_valid = False

print(type(x))       # Output: <class 'int'>
print(type(y))       # Output: <class 'float'>
print(type(name))    # Output: <class 'str'>
print(type(is_valid)) # Output: <class 'bool'>
```

## **Reassigning Variables**
Variables can be reassigned with different values, even of different types.

#### **Example:**
```python
x = 10
print(x)  # Output: 10

x = "Hello"
print(x)  # Output: Hello
```

## **Global and Local Variables**
- A **local variable** is declared inside a function and can only be accessed within that function.
- A **global variable** is declared outside a function and can be accessed throughout the program.

#### **Example:**
```python
global_var = "I'm global"

def my_function():
    local_var = "I'm local"
    print(local_var)  # Accessible inside the function

my_function()
print(global_var)  # Accessible anywhere

# print(local_var)  # This will cause an error because local_var is not accessible here.
```

## **Using `global` Keyword**
To modify a global variable inside a function, use the `global` keyword.

#### **Example:**
```python
counter = 0  # Global variable

def update_counter():
    global counter
    counter += 1  # Modify the global variable
    print("Counter updated:", counter)

update_counter()
update_counter()
```
