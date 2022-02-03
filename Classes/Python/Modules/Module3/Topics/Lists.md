
<!--Tags: #Lists #data_types #python #computer_science--> 

# Lists
## Info
- Lists are there own data type specefied as `list = []`
- Lists work differently than variables. They call to a specific point, and if you clone a list with `x = y`, for example, any changes to x will reflect in y
- Lists can nests lists, which allow for coordinates and multiple dimensions
<!-- time for 8 nested lists lol -->

## List Information Retrieval
- Lists are organized by **Indexing**. Python starts at 0, and you can count back with negative numbers.
- Indexes are decided with brackets `List[int]`
```python
numbers = [1, 2, 3, 4, 5]
print(numbers[0]) # prints 1, as 0 is the start
print(numbers[1]) # prints 2, as 2 is in the 1 index position
print(numbers[-1]) # prints 5, as 5 is the first number from the right

rnumbers = [5, 4, 3, 2, 1]
grid = [numbers, rnumbers]

print(grid[0][0]) # prints 1, as it looks for the first list, then the first number in that list
print(grid[1][0]) # prints 5, as it looks for the second list, then the first number in that list
```

- one can find the length of a list with `len()`
- `len()` returns an integer with the length of a list. This doesn't follow the weird 0 thing, just the straight up number of items
```python
numbers = [1, 2, 3, 4, 5]

print(len(numbers)) # returns 5

# practical use

for x in range(len(numbers)):
	print(x)
# This can be used if you need to iterate over a number related to a list and not 
#the list itself. While you just print here, it has more uses in more complex tasks

```
 - You may wish to find if an item is in a list, say from user input. What if you want to find out if something sin't in a list? the `in` keyword is used for this purpose
 - `in`, for the purposes of strings, takes a data point, then sees if it is in a list. If it is, in returns `True`. This means that we can also use `not in` to see if something isn't in a list
 - requires a string as an argument
  ```python

# example
str in list
places = ["home","school","here","there"]
fairytale_land = ["mordor, hogsmeade, australia"]

x = input("please name a place")

if x in places:
	print("I've been there")
elif x in fairytale_land:
	print("Thats not a real place!")
elif x not in places:
	print("You'll have to take me there sometime")

# else would be better here, but this is just for demonstration purposes


```
 - You way want to make a seperate list when copying it, or specify a range of items. we can do this with `[:]`. 
 - The left side specefies the start, and the right side specefies the end. 
 - Negative values can be used
 - If the left side is greater than the right side `[]` is the result
```python
numbers = [1, 2, 3, 4, 5]

print numbers[1:3] # prints 2 and 3

print numbers[-4:-4] # prints 2 and 3

section = numbers[1:3] # creates a new list with just the numbers 2 and 3. 
#Any changes made to numbers will not affect this

print(setion)

```
 - This is also known as **slicing**, and can be used in some methods or functions that take lists

 ## List manipulation
- Lists are a **mutable** data type. We can manipulate and change the contents of lists through various methods, functions, and keywords.

### del
- `del` is shorthand for delete
- `del` deletes an item based on an index
- `del` can use slicing to manipulate multiple index items at once
```python
numbers = [1, 2, 3, 4, 5]

del numbers[0] # deletes the item 1
print (numbers)

numbers = [1, 2, 3, 4, 5]

del numbers[0:4] # deletes all numbers except for 5

```

### Methods
- Lists have a few notable methods you can use to manipulate their contents, `.append()`, `.insert()`, `.reverse()`,and `.sort()`

#### .append()
- append means to add to the end, and thats exactly what it does
- `.append()` places a value at the end of a list
```python
numbers = [1, 2, 3, 4, 5]

numbers.append(6)

print(numbers) # Will print [1, 2, 3, 4, 5, 6]

```

#### .insert()
- `.insert()` is a bit more inteligent than `.append()`. It can insert a value at a specific **index**
```python
# list.insert(index,data) syntax

numbers = [1, 2, 4, 5]
numbers.insert(2, 3) # puts 3 in the correct place
print(numbers)

```
#### .reverse()
- `.reverse()` does exactly what it sounds like it does. It reverses a list
- `.reverse()` takes no arguments, it simply reverses the list.

```python
numbers = [1, 2, 3, 4, 5]
numbers.reverse() # reverses the list
print(numbers) # prints [5, 4, 3, 2, 1]
```
#### .sort()
- `.sort()` is also self explanitory. It sorts a list.
- Lists are asorted ascending by default
- Sort takes 2 arguments
	- The first is a `boolean` value, `reverse =`. This allows you to have a list sort by descending order
	- The second is `key=`. This allows you to sort based off of a diferent criteria defined by a function. W3Schools has a good example for them, but the function needs to do a few things:
		- Iterate over a list
		- return a value associated with an index
		- sort indexes according to their asigned value
```Python
def myFunction(var):
	# do something
	return var_changed

list = []
list.sort(reverse= True|False, key=myFunction)

```



```python
numbers = [3, 2, 1, 5, 4]
numbers.sort()
print (numbers)

numbers = [1, 2, 3, 4, 5]
numbers.sort(reverse=True)
print(numbers)

words = ["'stralia", "is", "not", "real"]

def myFunc(i):
	return len(i)

words.sort(key=myFunc)
print(words)

```

 

<!--### List data
Lists 
- List information
	- data type
	- Syntax
	- Shared memory
	- A list can contain a list. This allows lists to contain 2 values at one index, given that you have a second index to point 2. 2 numbers makes 2D. X and y, perhaps?
- info retrieval
	- indexes
	- negative indexes
	- displaying items 
	- len()
	- `in`
- List manipulation
	- deleting items `del`
	- List methods
		- `.append()`
		- `.insert()`
		- `.reverse()`
		- `.sort()` `not in`-->