# List comprehension

List comprehension is different from using a for loop to create a list because it allows you to create a new list in a single line of code, without the need to initialize an empty list, iterate over the iterable, apply the operation, and append the results to the new list.

An example of using a list comprehension to square the elements in a given list of integers:

```
numbers = [1, 2, 3, 4, 5]
squares = [num ** 2 for num in numbers]
print(squares)
#[1, 4, 9, 16, 25]
```


# Python decorator


a decorator is a design pattern that allows a user to modify or enhance the behavior of a function, method or class without directly modifying its code. It is a callable object that takes another function as input and returns a new function that adds some additional functionality to the original function.

code : 

```
def my_decorator(func):
    def wrapper():
        print("Before the function is called.")
        func()
        print("After the function is called.")
    return wrapper

@my_decorator
def my_function():
    print("Hello, world!")

my_function()

```

