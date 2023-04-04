# Read & Write Files in Python

* the with statement is used to open and close a file automatically

```
   with open('file.extention', 'r') as file:
        data = file.read()
   
    // The file is automatically closed 
```
* read() reads the entire file at once
```
 with open('file.extention', 'r') as file:
    data = file.read()
    print(data)
```
* readline() reads a single line at a time.

```
 with open('file.extention', 'r') as file:
    line = file.readline()
    while line:
        print(line)
        line = file.readline()
```
# Exceptions handling
it is used in Python to handle runtime errors that can occur during the execution of a program.

* the try block contains the code that is to be executed.

* the except block contains the code that handles the error.

* The finally block contain code that must be executed regardless of whether an exception is raised or not.