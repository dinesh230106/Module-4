# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

---

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

---

### ALGORITHM

1. Begin the program.  
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.  
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.  
4. Close the file (this is automatically done when exiting the `with` block).  
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.  
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.  
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.  
9. Return the dictionary `d1`, which contains the frequency of each character in the file.  
10. Terminate the program.

---

### PROGRAM

```
# Reg.No: 212223060057
# Name: DINESH KUMAR A
# Program to count the frequency of characters in a file

from collections import defaultdict

def create_file(file_path, content):
    # Create and write content to the file
    with open(file_path, 'w') as f:
        f.write(content)

def character_frequency(file_path):
    # Read the file and count character frequencies
    with open(file_path, 'r') as f:
        content = f.read()

    d1 = defaultdict(int)
    for ch in content:
        d1[ch] += 1

    return d1

# Main program
file_path = "sample.txt"
content = "Dinesh Kumar is learning Python programming."

# Create a file with sample content
create_file(file_path, content)

# Get and print character frequencies
freq = character_frequency(file_path)
print("Character frequencies in the file:")
for char, count in freq.items():
    print(f"'{char}': {count}")

```


### OUTPUT
```
Character frequencies in the file:
'D': 1
'i': 4
'n': 4
'e': 2
's': 2
'h': 2
' ': 5
'K': 1
'u': 2
'm': 3
'a': 3
'r': 4
'l': 1
'g': 2
'P': 1
'y': 1
't': 1
'o': 2
'.': 1

```


### RESULT
Thus, the Python program to find the frequency of characters in a file was successfully written, executed, and verified
