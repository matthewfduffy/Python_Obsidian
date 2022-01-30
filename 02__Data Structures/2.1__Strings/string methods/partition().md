#string-method 
### .partition()

##### Definition and Usage:
The `partition()` method searches for a specified string, and splits the string into a tuple containing three elements.
1. The first element contains the part before the specified string.
2. The second element contains the specified string.
3. The third element contains the part after the string.

##### Syntax:
 `string.partition(value)`

##### Parameter Values:
| Parameter | Description                         |
| --------- | ----------------------------------- |
| value     | Required. The string to search for. | 



##### Examples:
```python

txt = "I could eat bananas all day"

x = txt.partition("bananas")  
y = txt.partition("apples")

print(x)					# ('I could eat ', 'bananas', ' all day')
print(y)					# ('I could eat bananas all day', '', '')
```

If the specified value ==is found==, the `partition()` method returns a tuple containing: 1 - everything before the 'match', 2 - the 'match', 3 - everything after the 'match'

If the specified value ==is not found==, the partition() method returns a tuple containing: 1 - the whole string, 2 - an empty string, 3 - an empty string:


###### See Also:
[[2.1.0 -- String Methods Index]]
[.partition()](https://www.w3schools.com/python/ref_string_partition.asp)
