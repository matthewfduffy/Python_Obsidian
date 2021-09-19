#dictionary-method
## .keys()
##### Definition and Usage:
The `keys()` method returns a view object. The view object contains the keys of the dictionary, as a list.
The view object will reflect any changes done to the dictionary.


##### Syntax:
 `dictionary.keys()`

##### Parameter Values:
None.


##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.keys()
car["color"] = "white"

print(x)
```


###### See Also:
- [[2.4.2 -- Dictionary Methods Index]]
- [keys()](https://www.w3schools.com/python/ref_dictionary_keys.asp)