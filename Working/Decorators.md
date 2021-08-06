## Decorators
Functions that extend the behavior of other functions without explicitly modifying them.
*Decorators are a type of higher-order function*
```py
# defining a decorator function
def echo_wrapper(func):
	def wrapper():
		func()
		func()
	return wrapper


# defining a function that is decorated by wrapper
@echo_wrapper
def say_hello():
	print('Hello!')


# calling the decorated function
say_hello()
-----------
Hello!
Hello!
```

https://betterprogramming.pub/how-to-write-python-decorators-that-take-parameters-b5a07d7fe393