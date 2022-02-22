# Random Functions
## Function Functions
### yield()
- Yield acts like return, but it's for generator functions
- The basic explanation for a generator function is a function that can only be read once, as it doesn't store values but creates them on the fly.
## Iterable Functions
### map()
- map takes a function and an iterable, and then applies the function to every time in the iterable.
- Returns an address in memory, must be specified as a list, tuple, etc or printed after being iterated over, such as with a for loop
```python
def plusOne(list):
    return (list + 1)

x = [1, 2, 3, 4, 5]

print(list(map(plusOne, x)))
```

### filter()
- returns an iterable with all iterables, when the first argument evaluates as true
- `filter(boolean, iterable)`
```python
x = [1, 2, 3, 4, 5, "hello"]

def condition(val):
    if val == "hello" or val > 3:
        return True

for val in filter(condition, x):
    print (val)
```

### reduce()
- must be imported from functools
- reduce takes 2 values, a function and an iterable
- `reduce(boolean, iterable)`
- takes the first 2 values of the iterables and applies them as arguments to the function
- does this with all option
- does it again until there is one value left
- returns a integer or float

### reversed()
- reverses an iterable and returns it as an iterable value in memory
- `reversed(iterable)`
### sorted() and .sort()
- both sort a list either alphabetically or numerically
	- `Sorted()` is a function that sorts the instance in the line it is being sued on. This allows it to be used with tuples, as it never changes the actual data
	- .`sort()` is a method you add to the end of a string. This permanently changes the string, rather than changing an instance in memory for temporary usage
```python
letters = ['a', 'c', 'd', 'r', 'f', 'b']
print(f"unsorted list: {letters}")

print(f"sorted list, didn't change the list {sorted(letters)}")
print(f"notice {letters} is not sorted")
letters.sort() # sorts the list itself
print(f"notice {letters} itself is sorted, even though the sorting happened before")
```