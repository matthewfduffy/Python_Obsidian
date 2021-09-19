#dictionary-method
## .values()
##### Definition and Usage:
The `values()` method returns a view object. The view object contains the values of the dictionary as a list.
The view object will reflect any changes done to the dictionary.


##### Syntax:
 `dictionary.values()`

##### Parameter Values:
None.

##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.values()

car["year"] = 2018

print(x)

```


###### See Also:
[[2.4.2 -- Dictionary Methods Index]]
[values()](https://www.w3schools.com/python/ref_dictionary_values.asp)