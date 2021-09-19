#dictionary-method
## .popitem()
##### Definition and Usage:
The `popitem()` method removes the item that was last inserted into the dictionary
The removed item is the return value of the `popitem()` method, as a tuple.

> Prior to v.3.7, the `popitem()` method removes a random item.

##### Syntax:
 `dictionary.popitem()`

##### Parameter Values:
None.

##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.popitem()  

print(x)

```


###### See Also:
- [[2.4.2 -- Dictionary Methods Index]]
- [popitem()](https://www.w3schools.com/python/ref_dictionary_popitem.asp)