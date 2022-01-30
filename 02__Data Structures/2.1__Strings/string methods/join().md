#string-method
### .join()
 	

Syntax: 
`string.join(iterable)`

The `join()` method takes all items in an iterable and joins them into one string.
A string must be specified as the separator.

```python
myDict = {"name": "John", "country": "Norway"}
mySeparator = "TEST"

x = mySeparator.join(myDict)
print(x)

#nameTESTcountry
```

> Note: When using a dictionary as an [[iterable]], the returned values are the keys, not the values.


###### See Also:
[[2.1.0 -- String Methods Index]]
[.join()](https://www.w3schools.com/python/ref_string_join.asp)