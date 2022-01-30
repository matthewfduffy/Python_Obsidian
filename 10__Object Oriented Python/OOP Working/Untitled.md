https://www.codecademy.com/courses/learn-intermediate-python-3/projects/python-school-catalogue

class School:

 def __init__(self, name, level, numberOfStudents):

 self.name = name

 self.level = level

 self.numberOfStudents = numberOfStudents

  

 def get_name(self):

 return self.name

  

 def get_level(self):

 return self.level

  

 def get_numberOfStudents(self):

 return self.numberOfStudents

  

 def set_numberOfStudents(self, new_num):

 if isinstance(new_num, int):

 self.numberOfStudents = new_num

 else:

 raise TypeError

  

 def __repr__(self):

 print(f"A {self.level} school named {self.name} with {self.numberOfStudents} students")

  

class PrimarySchool(School):

 def __init__(self, pickupPolicy):

 self.pickupPolicy = pickupPolicy

  
  

# s1 = School("Baker High", "High School", 1300)

# print(s1.get_name())

# print(s1.get_numberOfStudents())

# s1.set_numberOfStudents(1400)

# print(s1.get_numberOfStudents())


These are the essential differences:

#### 🔸 **Class Attributes**

-   They belong to the class.
    
-   There is only one copy of each class attribute.
    
-   Changing their value affects all instances since they all take the value from the same source.
    

#### 🔹 **Instance Attributes**

-   They belong to the instances.
    
-   Each instance has a separate copy of each instance attribute.
    
-   Changing their value only affects a particular instance and the others remain unchanged.


A Class in Python:
```py
class Dog:
	"""A simple attempt to model a dog."""
	
	def __init__(self, name, age):
		"""Initialize name and age attributes."""
		self.name = name
		self.age = age

duncan = Dog()	# instantiating an object from class 'Dog'
```