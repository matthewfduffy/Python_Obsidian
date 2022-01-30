# Built-In Functions:
###### *Everything in Python is an object and we can inspect an object by using the built-in function `dir()`*
---
### Max and Min:
```python
#max and min

print(max([1,4,7,12,100]))

print(min(2, 100))

```

==highlight==
**bold**
_italic_

https://medium.com/analytics-vidhya/the-art-of-one-lining-in-python-1b96fc6fc5a9

Join (method):
```python
mylist = ['a', 'b', 'c', 'd']
#goal to return 'abcd'

#''.join(mylist)
#where '' is the character you wish to join on
print(''.join(mylist()))

print('--'.join(mylist))
#>>> a--b--c--d
```

Optimizing (Boolean) Functions:
```python
"""
Given a string and a target sub-string, 
write a program that determines whether the target sub-string is contained with in the string.
"""
# Ex. (Not Optimized)
def secret_check(mystring):
    if 'secret' in mystring:
        return True
    else:
        return False

print(secret_check('this is a secret'))
# >>> True
print(secret_check('sample test'))
# >>> False

# Optimized
def secret_check(mystring):
	return 'secret' in mystring
	
print(secret_check('this is a secret'))
# >>> True
print(secret_check('this is a Secret'))
# >>> False
# function does not account for upper/lower values
# modified 
def secret_check(mystring):
	return 'secret' in mystring.lower()

```