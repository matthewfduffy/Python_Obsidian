#list-method 
### .insert()
The `insert()` method inserts the specified value at the specified position.

##### Syntax:
 `list.insert(pos, elmnt)`

##### Parameter Values:
| Parameter | Description                                                         |
| --------- | ------------------------------------------------------------------- |
| pos       | Required. A number specifying in which position to insert the value |
| elmnt     | Required. An element of any type                                    | 


##### Examples:
```py
fruits = ['apple', 'banana', 'cherry']  
  
fruits.insert(1, 'orange')
print(fruits)	
# ['apple', 'orange', 'banana', 'cherry']
```

###### See Also:
[[2.2.2 -- List Methods index]]
[.insert](https://www.w3schools.com/python/ref_list_insert.asp)