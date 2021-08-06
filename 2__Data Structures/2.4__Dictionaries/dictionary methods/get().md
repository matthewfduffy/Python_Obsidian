#dictionary-method
## .get()
##### Definition and Usage:
The `get()` method returns the value of the item with the specified key.


##### Syntax:
 `dictionary.get(keyname, value)`

##### Parameter Values:
| Parameter | Description                                                                            |
| --------- | -------------------------------------------------------------------------------------- |
| keyname   | Required. The keyname of the item you want to return the value from                    |
| value     | Optional. A value to return if the specified key does not exist. Default value is None | 


##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.get("model")  
print(x)

# when value does not exist
x = car.get("price", 15000)    
print(x)
```

###### See Also:
[[2.4.2 -- Dictionary Methods Index]]
[get()](https://www.w3schools.com/python/ref_dictionary_get.asp)