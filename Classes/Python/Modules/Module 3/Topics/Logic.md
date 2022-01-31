<!-- Tags: #if #elif #else #logic #loops #conditionals -->


# Logical Functions
## If Statement
```python
if condition:
	Code to execute # notice the indent
Rest of the program
```
- If statement - The funtion
- condition - accepts operators and comparisons to return a boolean value
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

- Conditional functions need a condition to be defined. These give the condition to the function

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

## And
- Takes 2 