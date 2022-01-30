#python-keyword 
## None
Empty value constant. The equivalent of **Null**

```python
def f():
	x = 2
f() is None # True
```

```python
import re
match = re.match(r"Goodbye", "Hello World!")

if match is None:
	print("It doesn't match.")
-----------
It doesn't match
```

> When checking for `None` you must use `is` and `is not` instead of `==` and `!=`


%%Source: Finxter Python Cheat Sheet: Keywords [PDF]%%
%%Source: [Null in Python: Understanding Python's None Type Object](https://realpython.com/null-in-python/)%%