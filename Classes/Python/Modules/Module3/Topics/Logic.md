<!-- Tags: #if #elif #else #logic #loops #conditionals -->


# Logical Functions
## If Statement
```python
if condition # colon is necessary
	Code to execute # note the indent
Rest of the program
```
- If statement - The funtion
- condition - accepts operators and comparisons to return a boolean value. Alternatively may just use a boolean value, such as one stored in a variable previously
- Code to execute - executes when the `if` condition returns True, otherwise it is skipped
## Elif Statement
- `elif` takes a conditional. When `if` returns `False`, the next elif after it may execute, and so on. It then acts as an `if` statement
```python
if False == True:
	do x # This would fail to execute as false is not true
elif False == False:
	do y # This would execute as the if before it failed
```
## Else Statement
- `else` executes only if all `if` and `elif` statements before it return `False`. Code under it is executed
```python
if False == True:
	do x # This would fail to execute as false is not true
elif False == "Hello World":
	do y # This would fail as well, as a string is not False
else:
	print ("oops")
# oops would print, as both conditionals before would have failed
```
# Comparison Operators

- Conditional functions need a condition to be defined. These give the condition to the function by returning a boolean, which si either `True` or `False`. In this manner their output may be stored in variables for later.

#### Equality Comparisons
- `==`
- Takes 2 arguments, one to the left, one to the right
- If the left is the same as the right, return True

#### Not Equal
- `! =` (No space, render issue)
- Returns true if one value is not equal to another

#### Greater than
- `>`
- if left is greater than the right, return `True`

#### Less than
- `<`
- if left is less than the right, return `True`

#### Greater than or Equal too
- `> =` (No space, Render issue)
- if left is greater than or equal to the right, return `True`

#### Less than
- `< =` (No space, Render issue)
- if left is less than or equal to the right, return `True`



# Logic Operators
Logic Operators act as an aditional function you can use to modify and compare the results of comparison operators, allowing for complex comparisons

## and
- written as `and`, no capitals
- Takes a minimum 2 booleans as arguments
- both comparrison operators must be `True`
- can be chained for multiple arguments
- Returns a boolean
```python
x = 3
y = 5
z = 8

print(y == 5 and x+y == z)
# Returns as True, as y is equal to 5 an x + y does equal z

print(y == 5 and x+y == z and z == 8)
# Returns as True, as all 3 arguments are correct

print(y == 5 and x+z == y)
# Returns as False, as while y is equal to 5, x+z (3+8) does not equal 5
```
## or
- written as `or`, no capitals
- takes a minimum of 2 boolean arguments
- Only 1 argument must be `True`
- can be chained together for multiple arguments
- returns a boolean
```python
x = 3
y = 5
z = 8

print(y == 5 or x+y == z)
# Returns as True, as y is equal to 5 an x + y does equal z

print(y == 5 or x+z == y)
# Returns as True, as only one argument, in this case y==5, must be true

print(y == 5 or x+y == 2 or z == 3)
# Returns as True, as no matter the number, only one argument must be true
```

 ## not
 written as `not`, no capitals
- takes a minimum of 2 boolean arguments
- inverts a boolean value
<!-- think of truth in python as a `binary` system, hehe-->
	- `not False` --> `True`
	- `not True` --> `False`
- Rather than thinking of this as changing, think of it as a function that inverts a result.
- returns a boolean
```python
x = 3
y = 5
z = 8

print(not (y == 5 and x+y == z))
# Returns as False, as y is equal to 5 an x + y does equal z, then not inverts it

print(not(y == 5 and x+y == z and z == 8))
# Returns as False, as all 3 arguments are correct, then not inverts it

print(not(y == 5 and x+z == y))
# Returns as True, as while y is equal to 5, x+z (3+8) does not equal 5, then not inverts it
```

## All Together
- Multiple Logic operators can be used together to achieve results. For example:

```python

x = 3
y = 4
z = 2


if x == 3 and y == 2 or z==2:
	print("True")
# This program will output true, as while the and returns false, the or has a succesful argument, and will 
#retun everything as true. It may be helpful to visualise the program with parenthases like so:

if (x == 3 and y == 2) or z==2:
	print("True")

```

- Try mixing together a few logic operators and thinking of reasons why you might want to do so