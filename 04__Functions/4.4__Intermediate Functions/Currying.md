## Currying
refers to creating new functions from existing functions by applying partial arguments. (i.e. - partial functions).

```python
# define a function returns a value
def add_upp(num1, num2):
	sum_n = num1 + num2
	return sum_n
	

# define a partial function that adds seven
add_seven = lambda x: add_up(7, x)

>>> add_seven(10)
17
>>> add_seven(72)

# use a regular def keyword
def add_eight(x):
	return add_up(8, x)
	
>>> add_eight(10)
18
```

In the code above, we use the lambda function to set the number 7 as the first argument for the add_up function. In other words, the created add_seven function is a partial function of the original add_up with the first argument constantly set to be 7. Besides using the lambda function, it’s certainly acceptable to use the regular way to define a function with the def keyword.
Another handy tool to create partial functions is available in the functools module. Consider the following example. We use the partial function to create the add_ten function that has a default argument of 10 that’s calling the add_up function:

```py
>>> # import the module
>>> from functools import partial
>>> # using the partial function
>>> add_ten = partial(add_up, 10)
>>> add_ten(100)
110
```