*Everything in Python is an object*

> *An __Object__ is a collection of data (variables) and methods that operate on data*

We can inspect an object (anything) in Python by using the built-in function: `dir()`

```py
>>> len(5)
Traceback (most recent call last):
	File "<stdin>", line 1, in <module>
TypeError: object of type 'int' has no len()
```


```py
dir(5)
['__abs__', '__add__', '__and__', '__bool__', '__ceil__', '__class__',...]
```

The dunder (double-under) output are called **magic methods**
The list above is truncated but if expanded you'll notice that there's no `__len__`
dunder method for objects of type `int`

This is how Python's `len()` function knows that a number does not have a length.

All `len()` does, is call the `__len__()` method on the object it was offered.

> _When a function is part of an object, we call it a **method.**_

In contrast,  an object of type string does have a `__len__` method:
```py
print(len("test"))
#>>> 4

dir("test")
[..., '__len__', ...]
```

Since `__len__` is a method on type string, we can call it too:
```py
>>> "test".__len__()
4
```

> Note: This is equivalent to `len("test")`, but a lot less elegant.
___
Since everything in Python is an object and because objects are the building blocks of Python, it's only logical that users are allowed to create their own objects.

If you want to create your own type of object, you first need to define what methods it has and what data it can hold. This blueprint is called a class.

> *A __Class__ is a blueprint for an object*

All objects are based on a class. When we create an object, we call this '_creating an instance of a class_'

strings, numbers, and booleans are instances of classes

```py
>>> type('a')
<class 'str'>

>>> type(1)
<class 'int'>

>>> type(True)
<class 'bool'>
```

#### Self-Defined Class Example
```py
#Defining Class "Car"
class Car:
	speed = 0
	started = False
	
	def start(self):
		self.started = True
		print("Car started, let's ride!")
		
	def increase_speed(self, delta):
		if self.started:
			self.speed = self.speed + delta
			print('Vrooooom!')
		else:
			print("You need to start the car first.")
	
	def stop(self):
		self.speed = 0
		print('Halting')

#Creating object of type car
#Create an instance of class Car using Car() and assigned it to the variable car
>>> car = Car()

#call one of the methods on our car object
>>> car.increase_speed(10)
#output: You need to start the car first

>>> car.start()
#output: Car Started, let's ride!

>>> car.increase_speed(40)
#output: Vrooooom!


```
---
> An **object** is always an instance of a **class.** 
> One class can have many instances.
> Creating an instance looks like calling a function


Reviewing _class_ **Car** steps:
> A class is defined using the class statement followed by the name of the class (Car)
> Two variables were defined, speed and started
> Defined three methods that operate on the variables

### Self
1. When we call a method on an object, Python automatically fills in the first variable; called `self` by convention
2. This first variable is a reference to the object itself (hence its name)
3. We can use this variable to reference other instance variables and functions of this object, like `self.speed` and `self.start()` <br />

> Only inside the class definition do we use self to reference variables that are part of the instance

> To modify the `started` variable that's part of out class, we use `self.started` and not just `started` <br />
> By using `self`, it's made clear that we are operating on a variable that's part of this instance and not some other variable that is defined outside the object and that happens to have the same name.

---
> Interpreted and adapted  from [The Most Important Python Concept That You Need to Understand](https://towardsdatascience.com/the-most-important-python-concept-that-you-need-to-understand-985b98bbb84)

[[10.0 -- OOP Intro]]