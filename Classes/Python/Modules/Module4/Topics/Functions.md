# Functions

- Functions allow us to write pieces of code and reference
## Defining functions
- Functions are defined with the `def` keyword
- Functions have to be defined before you can use them
- Functions can call themselves, allowing you to make rudimentary loops upon failure of an `if` statement

```python
def myfunction (argument, paramater): # note colon
	print(argument, paramater) # note indent


myfunction(1, 2) #prints 1 2

myfunction(paramater = 2, argument = 1) #prints 1 2

myfunction() # returns an error, as the arguments are necessary. Note you still need a set of parenthases
```

### Return parameter
- `return` gives a value back to the main code
- Think of the function `float()`, for example. You give it a string or integer, and it **returns** a *floating point value*. If you define a function to give backa value, you are **returning** it in the same way.
```python
def myFunc(val)
	if val == "code"
		return("correct")
	else:
		return("Not right")
print(myFunc(input()))

```
- if something is `return`ed with nothing it has a type of `None`
### Scope of Names
- Variables only work within their scope
- For example, if one defines a variable within a function that variable doesn't exist outside of that function
- Variables defined outside of functions work **within functions**
- the `global` keyword can extend scope beyond functions

```python
def myFunc():
    global number # makes variable global
    number += 1

number = 1
print(number)
# Prints 1

myFunc() #function occurs, but nothing is returned
print(number) #number is printed
```
