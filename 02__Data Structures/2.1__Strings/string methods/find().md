#string-method 
### .find()
Searches the string for a specified value and returns the position of where it was found.

##### Definition and Usage:
The `find()` method finds the first occurrence of the specified value.
The `find()` method returns `-1` if the value is not found.
The `find()` method is almost the same as the [[02__Data Structures/2.1__Strings/string methods/index() | index()]] method.
The only difference is that the `index()` method raises an exception if the value is not found. (See example below) <br>

##### Syntax:
 `string.find(value, start, end)`

##### Parameter Value(s):
| Parameter | Description                                                              |
| --------- | ------------------------------------------------------------------------ |
| value     | Required. The value to search for.                                       |
| start     | Optional. Where to start the search. <br> Default is 0                   |
| end       | Optional. Where to end the search. <br> Default is to the end of string. | 

##### Example(s):
```py
print('smooth'.find('t'))
# => '4'
```

We searched the string `'smooth'` for the string `'t'` and found that it was at the fourth index spot, so `.find()` returned `4`.

You can also search for larger strings, and `.find()` will return the index value of the first character of that string.
```py
print("smooth".find('oo'))
# => '2'
```

Notice here that 2 is the index of the first `o`.


[[2.1.2 -- String Methods Index]]
[[02__Data Structures/2.1__Strings/string methods/index()]]
[.find()]((https://www.w3schools.com/python/ref_string_find.asp))