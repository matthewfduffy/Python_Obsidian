https://hourofpython.trinket.io/python-challenges#/string-challenges/abbreviator-challenge


```py
# Make a function abbreviator that, given a string, returns the string
# if the string is less than 5 charactors.  Otherwise, return the first
# four characters of the string, followed by a ".".
#
# >>>> abbreviator("Trinket")
# Trin.
# >>>> abbreviator("argh!")
# argh!

def abbreviator(string):
  if len(string) < 5:
    return string
  else:
    abbrev = string[:4]
    return abbrev + "."
  
# Add print statements here to test what your code does:
print abbreviator("Trinket")
print abbreviator("Matthew")
```