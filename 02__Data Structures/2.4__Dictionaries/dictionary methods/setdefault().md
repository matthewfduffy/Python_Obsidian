#dictionary-method
## .setdefault()
##### Definition and Usage:
The `setdefault()` method returns the value of the item with the specified key.
If the key does not exist, insert the key, with the specified vlaue.


##### Syntax:
 `dictionary.setdefault(keyname, value)`

##### Parameter Values:
| Parameter | Description                                                                                                                  |
| --------- | ---------------------------------------------------------------------------------------------------------------------------- |
| keyname   | Required. The keyname of the item you want to return the value from                                                          |
| value     | Optional. If the key exists, this parameter has no effect <br> If the key does not exist, the value becomes the key's value. | 


##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.setdefault("color", "white")  

print(x)

```


###### See Also:
- [[2.4.2 -- Dictionary Methods Index]]
- [setdefault()](https://www.w3schools.com/python/ref_dictionary_setdefault.asp)