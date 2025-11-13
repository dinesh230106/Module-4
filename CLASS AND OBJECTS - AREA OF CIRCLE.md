# Exp.No:19  
## CLASS AND OBJECTS - AREA OF CIRCLE

---

### AIM  
To write a Python program to take the radius from the user and find the area of a circle using the class name `umbrella` and function name `rain`.

---

### ALGORITHM

1. Begin the program.  
2. Create a class named `umbrella`.  
3. Define a method `rain(self, r)` inside the class `umbrella` that accepts a radius `r` as an argument.  
4. Inside the `rain` method:  
   - Calculate the area of a circle using the formula:  
     \[ \text{Area} = \pi \times r^2 \]  
   - Use the `math.pi` constant to get the value of π and perform the calculation.  
   - Print the result, formatted to two decimal places.  
5. Prompt the user for an integer input to represent the radius of the circle.  
6. Create an instance of the `umbrella` class and store it in the variable `u`.  
7. Call the `rain` method of the `umbrella` class, passing the user-provided radius `r` as an argument.  
8. Terminate the program.

---

### PROGRAM

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A
# Program to find the area of a circle using class and object

import math

class umbrella:
    def rain(self, r):
        area = math.pi * r ** 2
        print(f"The area of the circle with radius {r} is: {area:.2f}")

# Taking user input for radius
r = float(input("Enter the radius of the circle: "))

# Creating an object of class umbrella
u = umbrella()
u.rain(r)

```

### OUTPUT

```
Enter the radius of the circle: 5
The area of the circle with radius 5.0 is: 78.54

```

### RESULT
Thus, the Python program to calculate the area of a circle using a class and function was successfully written, executed, and verified.



