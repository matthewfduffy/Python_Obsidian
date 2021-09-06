https://hourofpython.trinket.io/python-challenges#/string-challenges/number-of-things-challenge

```py
# Make a function how_many that, given a list of a number
# and a thing name, returns a grmmatically correct sentence
# describing the number of things.
#
# >>>> how_many([5, "trinket"])
# There are 5 trinkets.
# >>>> how_many([1, "king"])
# There is 1 king.

def how_many(the_list):
  thing_count = the_list[0]
  thing = the_list[1]
  
  if thing_count == 1:
    return "There is 1 {}".format(thing)
  else:
    return "There are {} {}s".format(thing_count, thing)

  
# Add print statements here to test what your code does:
print how_many([5, "trinket"])
print how_many([1, "king"])
```