## Enumerate
`enumerate()` is a function useful when iterating over an iterator and you want to keep track of the value and the index both.
+ It adds a counter to an iterable and returns it.
+ Used mostly for keeping track of the index of items in a sequence

```py
# Syntax
enumerate(iterable, start=0)
```

Example 1:
```py
animals = ['cat', 'dog', 'cow']
print(list(enumerate(animals)))
------------------------------
[(0, 'cat'), (1, 'dog'), (2, 'cow')]

"""
As shown above, enumerate returns both index and value.
You can also set the index of the same by specifying the index value after the iterable
"""
animals = ['cat', 'dog', 'cow']
print(list(enumerate(animals, 10)))
------------------------------
[(10, 'cat'), (11, 'dog'), (12, 'cow')]
```

Example 2: Combine Enumerate with a loop to access the elements and index of an iterable at each iteration
```py
animals = ['cat', 'dog', 'cow']
for index, animal in enumerate(animals):
	if animal == 'cow':
		print(index)
```


%%[10 Must Know Built-in Functions in Python](https://medium.com/pythoneers/10-must-known-built-in-functions-in-python-2f196b9c0359)%%