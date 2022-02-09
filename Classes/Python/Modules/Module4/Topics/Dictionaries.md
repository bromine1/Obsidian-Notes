# Dictionaries
- Dictionaries allow us to store sets of data with keys in one variable

```python
#dictionary = {item1: key1, item2: key2}
# dictionaries store a data value which I can call with a key. For example:

data = {'trial1': 12312312, 'trial2': 87880989890}

print(data['trial1'])
#prints 12312312
print(data['trial2'])
# prints 87880989890
```

## Modifying a value
- Dictionaries can modify a key's value
```python
data = {'trial1': 12312312, 'trial2': 87880989890}

data[trial1] = 676778678678

print(data) # prints {'trial1': 676778678678, 'trial2': 87880989890}
```
## Adding a new key
- Dictionaries can have new values added to itself
```python
data = {'trial1': 12312312, 'trial2': 87880989890}

data['trial3'] = 676778678678

print(data) # prints {'trial1': 12312312, 'trial2': 87880989890, 'trial3': 676778678678}

# alternatively, one may use .update()

data = {'trial1': 12312312, 'trial2': 87880989890}

data.update({'trial3':676778678678})

print(data) # prints {'trial1': 12312312, 'trial2': 87880989890, 'trial3': 676778678678}
```
## Deleting a key
```python
data = {'trial1': 12312312, 'trial2': 87880989890}

del data['trial2']

print(data) # prints {'trial1': 12312312}
```




## Methods
### .keys()
- Dictionaries can sort of be iterated over with `for`
- `for` can grabe data with the `.key` method
```python
data = {'trial1': 12312312, 'trial2': 87880989890}

#Justs prints the keys
for key in data.keys():
    print(key)

# prints the keys and the values
for key in data.keys():
	print(key,"->", data[key])
```

### .items()
- `.items()` acts similarly to `.keys()`, except it returns both a key and it's value, and you need 2 variables to store the data
```python
data = {'trial1': 12312312, 'trial2': 87880989890}

# prints the keys and the values
for key, value in data.items():
	print(key,"->", value)
```

### .values()
- `.values()` returns a list of values
- Not really sure what the purpose is since it just shows all values
```python
data = {'trial1': 12312312, 'trial2': 87880989890}

# prints the keys and the values
for value in data.values():
	print(value) # prints a trial value
```