#python-keyword 
## class
A template for creating user-defined objects. Class definitions normally contain [[method]] definitions which operate on instances of the class.

```python
class Beer:
	def __init__(self):
		self.content = 1.0
	def drink(self):
		self.content = 0.0

becks = Beer()	# Constructor -> creates class
becks.drink() 	# beer empty: b.content == 0
```

See Also: [[class variable]]