### .extend()
#list-method 

The `extend()` method adds the specified list elements (or any iterable) to the end of the current list.

##### Syntax:
 `list.extend(iterable)`

##### Parameter Values:
| Parameter | Description                                     |
| --------- | ----------------------------------------------- |
| iterable  | Required. Any iterable (list, set, tuple, etc.) |


##### Example(s):
```py
fruits = ['apple', 'banana', 'cherry']  
  
cars = ['Ford', 'BMW', 'Volvo']  
  
fruits.extend(cars)
# ['apple', 'banana', 'cherry', 'Ford', 'BMW', 'Volvo']  
```

###### See Also:
[[2.2.2 -- List Methods index]]
[.extend()](https://www.w3schools.com/python/ref_list_extend.asp)