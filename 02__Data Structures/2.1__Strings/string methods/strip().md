#string-method
### .strip()



##### Syntax:
`string.strip(character)`

##### Example:
```python

featuring = "           rob thomas                 "
print(featuring.strip())
# => 'rob thomas'
```

You can also use `.strip()` with a character argument, which will strip that character from either end of the string.
```python
featuring = "!!!rob thomas       !!!!!"
print(featuring.strip('!'))
# => 'rob thomas       '
```

By including the argument `'!'` we are able to strip all of the '!'' characters from either side of the string. 

Notice that now that we’ve included an argument we are no longer stripping whitespace, we are ONLY stripping the argument.


###### See Also:
[[2.1.0 -- String Methods Index]]
[.capitalize()](https://www.w3schools.com/python/ref_string_capitalize.asp)