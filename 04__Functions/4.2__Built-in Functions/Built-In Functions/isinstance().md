#built-in-function 
## isinstance()
You can use the `isinstance()` function to check if an object is an instance of some class. 

##### Syntax:
`isinstance(item_to_check, data_type)`

##### Use:
Use when performing object-type comparisons.

```python
numbers = [1, 2, 3]

isinstance(numbers, list)	# True
isinstance(numbers, bool)	# False
isinstance(numbers, (list, float, int, bool))	# True
```