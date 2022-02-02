<!-- Tags: #python #functions #computer_science #loops -->

# Loops
In python, loops allow us to *interate* over code, or perform the same line of code mltiple times

There are 2 main types of loops
- `while` Loops
- `for` Loops

Each loops has its own purpose, and mastering both allows for fast and efficient code

## whileㅤLoops
- `while` accepts a `boolean` and some code
- `while` executes the code until the `boolean` is true
- the syntax is the exact same as the [`if`](Topics/Logic.md#IfㅤStatement) statement
```Python
# Syntax
while bool: # bool is boolean
	functions # note the indents

```

```python
y = True
x = 0

# This program prints x, then adds 1 to x. It does this forever unless stopped

while y:
	print(x)
	x += 1

```

## forㅤloops
- `for` loops work a little differently. They iterate a number of times that the coder specefies, such as in a range of numbers, a random amount of time, or for each item in a [list](Topics/Loops.md).
- the `for` loops needs a variable to store data in, which can be referenced within the function. It also needs the `in` keyword, to specify a range or some data to iterate through
- Check [W3schools](https://www.w3schools.com/python/python_for_loops.asp)
```python
for var in [range(), list, str]: # pick one, not all of these
	code # just a stand in for code
```
```python
for x in range(1, 100):
	print (x) # prints all numbers in a range of 1-100, doesn't print 100 but does print 1.
```
For more information on range, check [w3Schools](https://www.w3schools.com/python/ref_func_range.asp)
```python
fruit_list = ["apple","orange","grape"]
for x in fruit_list:
	print(x) #prints items in a list
```
```Python
string = "string"
for x in string:
	print (x) # prints letters in a string
```
```Python
fruit_list = ["apple","orange","grape"]
for word in fruit_list:
	for letter in word:
		print(letter) #prints all the letters from all the strings in a list
```

- Loops can also use the `else` statement, executing the code whenever they finish or return false