#dictionary-method
## .fromkeys()
##### Definition and Usage:
The `fromkeys()` method returns a dictionary with the specified keys and the specified value.


##### Syntax:
 `dict.fromkeys(keys, value)`

##### Parameter Values:
| Parameter | Description                                                     |
| --------- | --------------------------------------------------------------- |
| keys      | Required. An iterable specifying the keys of the new dictionary |
| value     | Optional. The value for al keys. Default valus is None.         | 


##### Examples:
```py
x = ('key1', 'key2', 'key3')
y = 0

this_dict = dict.fromkeys(x, y)
print(this_dict)
# {'key1': 0, 'key2': 0, 'key3': 0}
```


###### See Also:
- [[2.4.0 -- Dictionary Methods Index]]
- [fromkeys()](https://www.w3schools.com/python/ref_dictionary_fromkeys.asp)