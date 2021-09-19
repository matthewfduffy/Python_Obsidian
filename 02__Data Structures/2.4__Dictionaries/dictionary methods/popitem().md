#dictionary-method
## .popitem()
##### Definition and Usage:
The `pop()` method removes the specified item from the dictionary.
The value of the removed item is the return value of the `pop()` method


##### Syntax:
 `dictionary.pop(keyname, defaultvalue)`

##### Parameter Values:
| Parameter    | Description                                                      |
| ------------ | ---------------------------------------------------------------- |
| keyname      | Required. The keyname of the item you want to remove.            |
| defaultvalue | Optional. A value to return if the specified key does not exist. |

> Note: If a default value is not specified, and no item with the specified key is found, an error will be raised.

##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.pop("model")  

print(x)

```


###### See Also:
[[2.4.2 -- Dictionary Methods Index]]
[popitem()](https://www.w3schools.com/python/ref_dictionary_popitem.asp)