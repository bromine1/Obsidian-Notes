# [Functions](./Topics/Functions.md), [Tuples](./Topics/Tuples.md), [Dictionaries](./Topics/Dictionaries.md), and [Errors](./Topics/errors.md)
## Functions
- Functions act as keywords that allow us to reference sections of code
- Splitting up sections into taking some inputs and giving an output allows you to **Decompose** your code, making it so multiple devs can write their code for one program
### None
- `None` is a value that returns an error if it is used in almostany function
- Something has a `None` value if it has no data within it, such as something `return`ing nothing
- There are 2 situations where you can use `None` safely:
	- Assigning it to a variable `var = None`
	- Comparing to a variable `if var == None:`
## Tuples
- Tuples are an **Immutable**, or unchangeable, data type. Thik a list, except you can't change it
- Tuples are defined with a `()`, such as `var = ()`
- Otherwise function as lists, except you cannot manipulate data.
## Dictionaries
- Dictionaries act as an orderless way to store data
- data can be accessed through a `key`, or a value
- This allows us to make organized sets of data 

## Errors
- Sometimes our code will have errors. Even if we don't necessarily have a bug, there could be an error in user input.
- We can use a `try` and `except` key to run risky or prone parts of ccode. If it fails, the entire program doesn't have to.