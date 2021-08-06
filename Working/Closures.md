## Closures
Closures are nested functions that capture non-local variables of the outer functions.

[higher-order functions] functions that use other functions as input and output

```py
# create a closure
def make_multiplier(coefficient):	# outer function
	product = 1
	
	def multiplier():		# nested function
		nonlocal product		# non local variable
		product *= coefficient
		return product
	
	return multiplier		# outer function returns inner function
	
	
multiplier3 = make_multiplier(3)

>>> multiplier3()
3
>>> multiplier3()
9
>>> multiplier3()
27
>>> multiplier3.__code__.co_freevars	# variable binding
('coefficient', 'product')
>>> multiplier3.__closure__[1].cell_contents	#value capturing
27
```

1. `make_multiplier()` is the outer function
2. `multiplier()` is the nested function
3. The outer function returns the nested function as its return value
4. The nested function uses and modifies a *non-local* variable defined within the scope of the outter function

Everytime we call the multiplier3, the product is multiplied by three and the closure remembers the state of the product after it's last use.

https://medium.com/swlh/anatomize-pythons-closures-dbf0fa217d38


