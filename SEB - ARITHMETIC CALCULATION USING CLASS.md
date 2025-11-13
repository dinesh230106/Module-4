# Exp.No:20  
## SEB - ARITHMETIC CALCULATION USING CLASS

---

### AIM  
To write a Python program to perform addition and division operations using a class. The class should be named `Saveetha`, and the function names should be `setvalues` (to set `a` and `b` values), `add`, and `div`. The program should handle the following cases:  
- `choice 1` → Perform addition  
- `choice 2` → Perform division  
- `choice 0` → Exit  
- For other choices, print 'Invalid choice'

---

### ALGORITHM

1. Begin the program.  
2. Create a class `Saveetha`.  
3. Define the following methods inside the `Saveetha` class:  
   - `__init__(self)`: Initializes `a` and `b` to zero.  
   - `setvalues(self, a, b)`: Sets the values of `a` and `b`.  
   - `add(self)`: Performs the addition operation.  
   - `div(self)`: Performs the division operation. If `b` is zero, returns an error message for division by zero.  
4. Create a `main()` function.  
5. Take input from the user for the values of `a` and `b` using `setvalues(a, b)` method.  
6. Use a `while True` loop to repeatedly ask the user for a choice:  
   - If the choice is 1, call the `add()` method and print the result.  
   - If the choice is 2, call the `div()` method and print the result. Handle division by zero.  
   - If the choice is 0, print "Exiting!" and exit the loop.  
   - If the choice is not 1, 2, or 0, print "Invalid choice".  
7. Terminate the program.

---

### PROGRAM

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A
# Program to perform arithmetic operations using a class

class Saveetha:
    def __init__(self):
        self.a = 0
        self.b = 0

    def setvalues(self, a, b):
        self.a = a
        self.b = b

    def add(self):
        return self.a + self.b

    def div(self):
        try:
            return self.a / self.b
        except ZeroDivisionError:
            return "Error: Division by zero is not allowed."

# Main function
def main():
    s = Saveetha()

    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))

    s.setvalues(a, b)

    while True:
        print("\n1. Addition")
        print("2. Division")
        print("0. Exit")
        choice = int(input("Enter your choice: "))

        if choice == 1:
            print("Result of addition:", s.add())
        elif choice == 2:
            print("Result of division:", s.div())
        elif choice == 0:
            print("Exiting!")
            break
        else:
            print("Invalid choice")

# Run the program
main()



```

### OUTPUT
```
Enter first number: 10
Enter second number: 5

1. Addition
2. Division
0. Exit
Enter your choice: 1
Result of addition: 15.0

1. Addition
2. Division
0. Exit
Enter your choice: 2
Result of division: 2.0

1. Addition
2. Division
0. Exit
Enter your choice: 0
Exiting!

```
or
```
Enter first number: 10
Enter second number: 0
Enter your choice: 2
Result of division: Error: Division by zero is not allowed.

```

### RESULT
Thus, the Python program to perform arithmetic operations (addition and division) using a class and object was successfully written, executed, and verified.
