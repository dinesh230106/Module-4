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

from sys import getsizeof
dic1 = {"A": 1, "B": 2, "C": 3}
dic2 = {"Geek1": "Raju", "Geek2": "Nikhil", "Geek3": "Deepanshu"}
dic3 = {1: "Lion", 2: "Tiger", 3: "Fox", 4: "Wolf"}
result1 = getsizeof(dic1)
result2 = getsizeof(dic2)
result3 = getsizeof(dic3)
print("Size of dic1: ", result1, "bytes", sep='')
print("Size of dic2: ", result2, "bytes", sep='')
print("Size of dic3: ", result3, "bytes", sep='')

```

### OUTPUT
<img width="679" height="213" alt="image" src="https://github.com/user-attachments/assets/a2fcb18c-6a2f-4f93-9355-84ec8e48df46" />



### RESULT
Thus, the Python program to find the size of dictionaries using sys.getsizeof() was successfully executed and verified.
