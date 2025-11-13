# Exp.No:16  
## DICTIONARY - SIZE OF DICTIONARY

---

### AIM  
To write a Python program to print the size of a dictionary using `getsizeof()` from the `sys` module.

---

### ALGORITHM

1. Begin the program.  
2. Import the `sys` module to use the `getsizeof()` function.  
3. Define the dictionaries with key-value pairs (`dic1`, `dic2`, `dic3`).  
4. Use `sys.getsizeof()` to calculate the memory size of each dictionary.  
5. Print the size of each dictionary in bytes.  
6. Terminate the program.

---

### PROGRAM

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A
# Program to find the size of dictionaries using sys.getsizeof()

import sys

# Defining dictionaries
dic1 = {"a": 1, "b": 2, "c": 3}
dic2 = {"name": "Dinesh", "age": 21, "place": "Chennai"}
dic3 = {1: "apple", 2: "banana", 3: "mango", 4: "orange"}

# Printing size of each dictionary
print("Size of dic1:", sys.getsizeof(dic1), "bytes")
print("Size of dic2:", sys.getsizeof(dic2), "bytes")
print("Size of dic3:", sys.getsizeof(dic3), "bytes")


```

### OUTPUT
```
Size of dic1: 232 bytes
Size of dic2: 248 bytes
Size of dic3: 264 bytes

```


### RESULT
Thus, the Python program to find the size of dictionaries using sys.getsizeof() was successfully executed and verified.
