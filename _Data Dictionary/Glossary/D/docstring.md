## docstring
A string literal which appears as the first expression in a [[_Data Dictionary/Glossary/C/class]], [[function]] or [[module]] that describes what a program is trying to accomplish.
Denoted by `""" """` block.

While ignored when the suite is executed, it is recognized by the compiler and put into the `__doc__` attribute of the enclosing class, function, or module.

```py
class Dog:
	"""A simple attempt to model a dog."""	# this is a docstring
	...
```
