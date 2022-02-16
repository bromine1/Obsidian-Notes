# Classes and Objects
- Classes are a way to model real life situations 
- Classes can store data in themselves, and you can also make **Objects** from classes, essentially instances with data, such as a specific cat from the class cats
Classes have a few things you can do with them

```python
class day:
    day_of_week = ('Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')
    vacation = (True, False)
    def __init__ (day, day_of_week = day_of_week, vacation = vacation):
        day.weekday = day_of_week[random.randint(0,6)]
        day.vacation = vacation[random.randint(0, 1)]
    def sleepIn(day):
        if day.weekday == 'Sunday'or day.weekday == 'Saturday':
            return True
        if day.vacation:
            return True
```

Lets break this down a little

## Class Definition
```python
class day:
	# Don't forget the indent!
```
- This is how one starts a class. Like other functions that contain items, you need a colon and an indent for python to determine what belongs to who
- day is an example here, but its really just a name, which could be anything
```python
class day:
	# new code
    day_of_week = ('Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')
    vacation = (True, False)
```
- Variables defined like this, inside a class, are held by every object made from the class
```python
class day:
    day_of_week = ('Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')
    vacation = (True, False)
	# New code: init
    def __init__ (self, day_of_week = day_of_week, vacation = vacation):
        self.weekday = day_of_week[random.randint(0,6)]
        self.vacation = vacation[random.randint(0, 1)]
```
- the first function in a class should be the `def __init__()` function
- This function executes whenever an instance is created

Here, we should break away to talk about something special when defining functions in a class. The first argument isn't an argument, but rather a reference to the object. This lets you store data on a per-object basis

Standard practice is to use `self` as the first variable, as you are describing the object, but it can be anything

- after this, it acts as any other function definition
- using `self.var`, one can assign variables on a per object basis.

```python
class day:
    day_of_week = ('Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')
    vacation = (True, False)
    def __init__ (self, day_of_week = day_of_week, vacation = vacation):
        self.weekday = day_of_week[random.randint(0,6)]
        self.vacation = vacation[random.randint(0, 1)]
	# New Code
    def sleepIn(self):
        if self.weekday == 'Sunday'or self.weekday == 'Saturday':
            return True
        if self.vacation:
            return True

```
- Functions can also be assigned to classes.
- within a function, the first variable is also a reference to the object
- Data from within objects can be called, but functions can also take external arguments
- These functions are called as method to a class, in this case `.sleepIn()`
Fully commented, our class looks like this:
```python
class day:
	# Set class attributes
    day_of_week = ('Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')
    vacation = (True, False)
	# get data for the day
    def __init__ (self, day_of_week = day_of_week, vacation = vacation):
        self.weekday = day_of_week[random.randint(0,6)]
        self.vacation = vacation[random.randint(0, 1)]
	# define function to see if we can sleep in
    def sleepIn(self):
        if self.weekday == 'Sunday'or self.weekday == 'Saturday':
            return True
        if self.vacation:
            return True


```
## Working with classes
- Classes work a little differently than some other things. You need to assign an instance of a class to a variable as an object in most cases, and can start working with them then. There is an exception if you are working with data that pertains to a class only, such as `vacation` in the examples above
```python
date = day()
print(date.weekday)
print(date.vacation)
if date.sleepIn() == True:
    print("I'm sleepin in!")
else:
    print("Time to get up!")
```
This is also a lot, lets break it down by piece. Keep in mind that you will need the example code above to use this
```python
date = day()
```
- This makes an instance of `day` and gives it the name `data`
```python
date = day()
# new code
print(date.weekday)
print(date.vacation)
```
- This displays a few attributes. Note that we are calling the attributes specific to our instance, `data`.
```python
date = day()
print(date.weekday)
print(date.vacation)
# new code
if date.sleepIn() == True:
    print("I'm sleepin in!")
else:
    print("Time to get up!")
```
- we call the function we defined earlier, `sleepIn`, by referencing our object, `data`, with `.sleepIn()`. By doing this, we specify which object's data we want to use. 

There are a few more things you can do, such as [Class methods and static methods](https://stackabuse.com/pythons-classmethod-and-staticmethod-explained/), but those are a topic for another time.