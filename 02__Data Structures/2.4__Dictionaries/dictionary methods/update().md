#dictionary-method
## .update()
##### Definition and Usage:
The `update()` method inserts the specified items to the dictionary.
The specified items can be a dictionary, or an iterable object with key value pairs.


##### Syntax:
 `dictionary.update(iterable)`

##### Parameter Values:
| Parameter | Description                                                                                     |
| --------- | ----------------------------------------------------------------------------------------------- |
| iterable  | A dictionary or an iterable object with key value pairs that will be inserted to the dictionary | 



##### Examples:
```py
car = {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}  
  
car.update({"color": "White"})  

print(car)

```


###### See Also:
- [[2.4.2 -- Dictionary Methods Index]]
- [update()](https://www.w3schools.com/python/ref_dictionary_update.asp)




