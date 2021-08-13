#string-method 
### .index()


##### Definition and Usage:
The `index()` method finds the first occurrence of the specified value.
The `index()` method raises an exception if the value is not found.
The `index()` method is almost the same as the `find()` method, the only difference is that the `find()` method returns `-1` if the value is not found. (See example below)

##### Syntax:
 `string.index(value, start, end)`

##### Parameter Values:
| Parameter | Description                                                            |
| --------- | ---------------------------------------------------------------------- |
| value     | Required. The value to search for.                                     |
| start     | Optional. Where to start the search. Default is 0.                     |
| end       | Optional. Where to end the search. Default is to the end of the string | 

##### Example(s):
```py
txt = "Hello, welcome to my world."  
  
x = txt.index("e")  		# searching full text for the first occurrence of 'e'
y = txt.index("e", 5, 10)	# seaching for first occurrence of 'e' between 5th and 10th position
print(x)	# => 1
print(y)	# => 8
```




###### See Also:
- [[2.1.2 -- String Methods Index]]
- [[find()]]
- [.index()](https://www.w3schools.com/python/ref_string_index.asp)
