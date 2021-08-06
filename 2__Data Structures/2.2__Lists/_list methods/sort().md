### .sort()
#list-method 

The `sort()` method sorts the list in alphabetical-ascending order, by default

##### Syntax:
 `list.sort(reverse=True|False, key=myFunc)`

##### Parameter Values:
| Parameter | Description                                                                   |
| --------- | ----------------------------------------------------------------------------- |
| reverse   | Optional. revers=True will sort the list descending. Default is reverse=False |
| key       | Optional. A function to specify the sorting criteria.                         | 


##### Examples:
```py
this_list = ["orange", "mango", "kiwi", "pineapple", "banana"]
this_list.sort()
print(this_list)     # ['banana', 'kiwi', 'mango', 'orange', 'pineapple']
```

###### See Also:
[[2.2.2 -- List Methods index]]
[.sort()](https://www.w3schools.com/python/ref_list_sort.asp)