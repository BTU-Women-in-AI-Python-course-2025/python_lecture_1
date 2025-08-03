# **Bitwise Operators in Python**  

## **What are Bitwise Operators?**  
Bitwise operators are used to perform operations on **binary numbers** (bits). These operators work on individual bits of a number.

Python represents numbers in **binary form**, where:  
- `0` represents **False**  
- `1` represents **True**  

Each bitwise operation is performed at the **bit level**.

---

## **Bitwise Operators Table**

| Operator | Name | Description | Example (`a = 5`, `b = 3`) |
|----------|------|-------------|----------------------|
| `&` | **Bitwise AND** | Returns 1 if both bits are 1 | `5 & 3 → 1` (`101 & 011 = 001`) |
| `\|` | **Bitwise OR** | Returns 1 if at least one bit is 1 | `5 \| 3 → 7` (`101 \| 011 = 111`) |
| `^` | **Bitwise XOR** | Returns 1 if only one of the bits is 1 | `5 ^ 3 → 6` (`101 ^ 011 = 110`) |
| `~` | **Bitwise NOT** | Inverts all bits (one’s complement) | `~5 → -6` (`~101 = -(101+1) = -110`) |
| `<<` | **Left Shift** | Shifts bits to the left (multiplies by 2) | `5 << 1 → 10` (`101 << 1 = 1010`) |
| `>>` | **Right Shift** | Shifts bits to the right (divides by 2) | `5 >> 1 → 2` (`101 >> 1 = 010`) |

---

## **1. Bitwise AND (`&`)**
Returns **1** only if both bits are **1**.

### **Example:**
```python
a = 5  # Binary: 101
b = 3  # Binary: 011

print(a & b)  # Output: 1 (Binary: 001)
```

### **Explanation:**
```
   101  (5 in binary)
 & 011  (3 in binary)
  ------
   001  (1 in decimal)
```

---

## **2. Bitwise OR (`|`)**
Returns **1** if at least one of the bits is **1**.

### **Example:**
```python
a = 5  # Binary: 101
b = 3  # Binary: 011

print(a | b)  # Output: 7 (Binary: 111)
```

### **Explanation:**
```
   101  (5 in binary)
 | 011  (3 in binary)
  ------
   111  (7 in decimal)
```

---

## **3. Bitwise XOR (`^`)**
Returns **1** if only one of the bits is **1**, but not both.

### **Example:**
```python
a = 5  # Binary: 101
b = 3  # Binary: 011

print(a ^ b)  # Output: 6 (Binary: 110)
```

### **Explanation:**
```
   101  (5 in binary)
 ^ 011  (3 in binary)
  ------
   110  (6 in decimal)
```

---

## **4. Bitwise NOT (`~`)**
Inverts all bits (**one’s complement**). In Python, `~x` is equivalent to `-(x+1)`.

### **Example:**
```python
a = 5  # Binary: 101

print(~a)  # Output: -6 (Binary: -110)
```

### **Explanation:**
```
   101  (5 in binary)
  ~101  (Invert all bits)
  ------
  -110  (Equivalent to -6 in decimal)
```

---

## **5. Left Shift (`<<`)**
Moves bits to the left, **multiplying by 2** for each shift.

### **Example:**
```python
a = 5  # Binary: 101

print(a << 1)  # Output: 10 (Binary: 1010)
```

### **Explanation:**
```
   101  (5 in binary)
 << 1   (Shift left by 1 position)
  ------
  1010  (10 in decimal)
```
> **Formula:** `a << n` = `a * (2^n)`

---

## **6. Right Shift (`>>`)**
Moves bits to the right, **dividing by 2** for each shift.

### **Example:**
```python
a = 5  # Binary: 101

print(a >> 1)  # Output: 2 (Binary: 10)
```

### **Explanation:**
```
   101  (5 in binary)
 >> 1   (Shift right by 1 position)
  ------
    10  (2 in decimal)
```
> **Formula:** `a >> n` = `a // (2^n)`

---

## **Summary Table**
| Operator | Name | Effect |
|----------|------|--------|
| `&` | **Bitwise AND** | 1 if both bits are 1 |
| `\|` | **Bitwise OR** | 1 if at least one bit is 1 |
| `^` | **Bitwise XOR** | 1 if only one bit is 1 |
| `~` | **Bitwise NOT** | Inverts all bits |
| `<<` | **Left Shift** | Multiplies by `2^n` |
| `>>` | **Right Shift** | Divides by `2^n` |
