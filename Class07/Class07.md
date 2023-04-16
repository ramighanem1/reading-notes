#
In Python, variable scope refers to the part of the code where a variable is visible and accessible. There are two types of variable:


* Local scope : refers to variables that are declared inside a function. These variables can only be accessed within that function and are not visible outside of it. Once the function completes execution, the variables declared inside the function are destroyed.

* Global scope : refers to variables that are declared outside of any function, and they can be accessed from anywhere in the code. 

code : 

```
name = "rami"

def function():
    # Local scope variable
    name = "saif"
    print("Hello, " + name + "!")
  
function()  # Output: Hello, saif!
print("Goodbye, " + name + "!")  # Output: Goodbye, rami!
```

# the global and nonlocal keywords


global is used to access and modify a variable defined in the global scope (outside any function) from within a function

```
count = 0

def increment():
    global count
    count += 1

increment()
print(count)  # Output: 1
```

nonlocal is used to access and modify a variable defined in an outer function scope from within an inner function
```

def outer():
    x = 1

    def inner():
        nonlocal x
        x += 1
        print(x)

    inner()

outer()  # Output: 2

```


# Big O

Big O notation is a mathematical notation used to describe the performance of an algorithm in terms of its input size and its predictor of real-world performance


#  simulate a dice roll

To simulate a dice roll using Python, you can use the random module, specifically the randint() function which generates a random integer between two specified values.

To calculate the probability of rolling a specific number over a large number of trials, you can use a loop to simulate multiple rolls and count how many times the desired number is rolled. 
