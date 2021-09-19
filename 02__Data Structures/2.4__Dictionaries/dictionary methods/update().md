#dictionary-method
## .update()
##### Definition and Usage:
The `update()` method inserts the specified items to the dictionary.
The specified items can be a dictionary, or an iterable object with key value pairs.


##### Syntax:
 `dictionary.update(iterable)`

##### Parameter Values:
| Parameter | Description                                           |
| --------- | ----------------------------------------------------- |
| iterable  | Required. The keyname of the item you want to remove. |

> Note: If a default value is not specified, and no item with the specified key is found, an error will be raised.

##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
x = car.update("model")  

print(x)

```


###### See Also:
[[2.4.2 -- Dictionary Methods Index]]
[update()](https://www.w3schools.com/python/ref_dictionary_update.asp)




