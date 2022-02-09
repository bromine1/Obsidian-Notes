# Errors
- errors can be "handled" with the `try` and `except` keywords.
```python
def func():
    try:
        x = (int(input()))
		print(x/1)
    except:
        print("that was not a number")
        func()
func()
```
- `try` needs an `except` or `finally`



## Specific Exceptions
- `except` can take an argument on what kind of error it should process
```python
def func():
    try:
        x = (int(input()))
        print(1/x)
    except ValueError:
        print("that was not a number")
        func()
    except ZeroDivisionError:
        print("you can't divide by 0")
func()
```

### Kinds of errors
- There are a few usefule errors to know
#### ZeroDivisionError
- `ZeroDivisionError`
- You can't divide by 0, that returns an error
#### ValueError
- `ValueError`
- Occurs if a value recieved by a function is of an unexpected type, such as `int()` recieving a string with `5.2`
#### TypeError
- `TypeError`
- Occurs when the wrong kind of data is inputted into a function
#### AttributeError
- `AttributeError`
- Occurs when you try to use a method that doesn't work
#### SyntaxError
`SyntaxError`
- Occurs when you made a grammar error in your code. Don't try and ahndle this, as it's entirely on you.
### General Exception
- You can specify exceptions, and if an option isn't specefied it becomes the default option
```python
def func():
    try:
        x = (int(input()))
        print(1/x)
    except ValueError:
        print("that was not a number")
        func()
    except ZeroDivisionError:
        print("you can't divide by 0")
        func()
    except:
        print("huh, something went wrong, please try again")
        func()
func()
```
