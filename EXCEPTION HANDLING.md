# Exp.No:17  
## EXCEPTION HANDLING

---

### AIM  
To create a Python program that prompts the user for a list of grades separated by commas, splits the string into individual grades, and uses exception handling to inform the user if the values they entered cannot be converted to integers.

---

### ALGORITHM

1. Begin the program.  
2. Read a string `input_str` from the user using `input()`.  
3. Split the input string using commas (`,`) to create a list of grades.  
4. Use a `try` block to attempt converting each item in the grades list to an integer and store the result in `l1`.  
5. If the conversion is successful, print the list `l1` containing the integer values.  
6. If an error occurs during conversion (for example, if the input is not a valid number), catch the exception and print an error message: `"The grades you entered were in an invalid format."` along with the original grades list.  
7. Terminate the program.

---

### PROGRAM

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A
# Program to demonstrate exception handling for grade input

try:
    # Read input from the user
    input_str = input("Enter grades separated by commas: ")

    # Split the string into individual grades
    grades = input_str.split(",")

    # Convert each grade to integer
    l1 = [int(grade) for grade in grades]

    # Print the converted list
    print("List of integer grades:", l1)

except ValueError:
    # Handle invalid inputs
    print("The grades you entered were in an invalid format.")
    print("Original input:", grades)


```

### OUTPUT
```
Enter grades separated by commas: 85,90,78,88
List of integer grades: [85, 90, 78, 88]

```
or
```
Enter grades separated by commas: 85,abc,90
The grades you entered were in an invalid format.
Original input: ['85', 'abc', '90']

```

### RESULT
Thus, the Python program demonstrating exception handling for invalid grade inputs was successfully executed and verified.
