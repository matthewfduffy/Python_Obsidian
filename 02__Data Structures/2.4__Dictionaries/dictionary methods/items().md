#dictionary-method
## .items()

The `items()` method returns a view object. The view object contains the key-value pairs of the dictionary, as tuples in a list.

The view object will reflect any changes done to the dictionary.

##### Syntax:
 `dictionary.items()`

##### Parameter Values:
None.

##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.items()
car["year"] = 2018

print(x)
```


###### See Also:
- [[2.4.0 -- Dictionary Methods Index]]
- [items()](https://www.w3schools.com/python/ref_dictionary_items.asp)