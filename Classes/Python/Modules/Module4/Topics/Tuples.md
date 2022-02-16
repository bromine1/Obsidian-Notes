# Tuples
- Tuples are immutable in that the data within them cannot **Change.** This does not mean, however, that we cannot add to a tuple during a runtime
- Tuples can be used as keys for dictionaries
- Search is faster as the program does not need to reindex often

## Addition
- You can add tuples onto other tuples
```python
t1 = (1, 2, 3)
t2 = (4, 5, 6)

tuple = t1 + t2

print(tuple)
#returns (1, 2, 3, 4, 5, 6)
```

## Multiplication
- Tuples can be multiplied like lists
```python
t = (1, 2, 3)

t *= 3

print(t)
#returns (1, 2, 3, 1, 2, 3, 1, 2, 3)
```