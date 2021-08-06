### Object Oriented Programming (Part 1)
[[Python - Under the Hood]]
> **Object Oriented Programming** allows developers to create their own objects that have methods and attributes. <br>
> These methods act as functions that use information about the object, as well as the object itself to return results, or change the current object.<br>
> In general, OOP allows us to create code that is repeatable and organized.

<br>
Basic Syntax for OOP:

```py
class NameofClass():	#define class; camelCase is standard

	def __init__(self, param1, param 2):	#initializes class
		self.param1 = param1	#attribute
		self.param2 = param2
		
	def some_method(self):		#method call
		#perform some action
		print(self.param1)

```


```py
#OOP Example
class Dog():

	#CLASS OBJECT ATTRIBUTES
	#by convention comes before __init__ and outside methods of class

	def __init__(self, input_breed, name):	
		self.breed = input_breed
		self.name = name
		
sam = Dog('lab', 'Sammy')	#this is an instance of a dog
#print(type(x.breed))

print(sam.breed)
print(sam.name)
		
#__init__ called automatically called after creating an instance of object
# each attribute in the class definition begins with a reference to the actual instance object (self keyword)
```

>_**Class Object Attributes**_ by convention come before `__init__` and outside methods of the class.<br/>
>The purpose of COAs is for things that are going to be true regardless of the instance of the dog

```py
#OOP Example
class Dog():

	#CLASS OBJECT ATTRIBUTES
	species = 'mammal'

	def __init__(self, breed, name):	
		self.breed = breed
		self.name = name

Duncan = Dog('Lab', 'Duncan')
		
print(Duncan.breed)		#Lab
print(Duncan.name)		#Duncan
print(Duncan.species)	#mammal



```