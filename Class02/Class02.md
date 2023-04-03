# Test-Driven Development (TDD) in Python

Unit tests are code segments used to test the input, output, and behavior of software. It's important to name the test file according to the module being tested and to separate the tests folder from code.

The tests should be descriptive and include the expected results. The AAA structure (Arrange, Act, Assert) is used to organize tests. In Arrange, you need to organize the data needed to execute the code. In Act, you execute the code being tested. In Assert, you check if the output is the same as expected.

To use TDD with Python, developers typically follow the following process:

* Write a test that defines the behavior or functionality of the code.
* Run the test to see if it fails (since the code doesn't exist yet).
* Write the minimal code needed to pass the test.
* Run the test again to ensure that it passes.
* Refactor the code as needed to improve its design or performance.
* Repeat the process with the next test.

# if __name__ == '__main__':
is used to check if the current module is being run as the main program or if it has been imported into another module


# recursion :
is the process of calling a function within
itself. This allows for the solution of complex
problems by breaking them down into smaller.

# difference between Python modules and packages

* module: it is a file containing Python definitions and statements. It can define functions, classes, and variables, and can be imported into other Python programs

```
import file
obj = file.my_function()
```

* package: it is a collection of modules organized in a directory

```
import package_name.module_name
obj = package_name.module_name.my_function()
```