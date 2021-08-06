### OOP Part 2 Py
[[Python - Under the Hood]]
[[OOP - Part 1 - Py]]

```py

class Circle():
	
	#CLASS OBJECT ATTRIBUTES
	pi = 3.14
	
	def __init__(self, radius=1):	#__init__ aka 'special method'
		self.radius = radius
		
	def area(self):
		return self.radius * self.radius * self.pi
		
	def circumference(self):
		return 2 * self.pi * self.radius
		
mycircle = Circle()
print(mycircle.radius)	#1 because default when no radius provided
print(mycircle.area)	#will not execute because area is a method
#corrected
print(mycircle.area())
print(mycircle.circumference())	#5:51 video 53
```