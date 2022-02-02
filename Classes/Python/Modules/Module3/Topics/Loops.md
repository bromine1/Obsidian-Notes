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
- 