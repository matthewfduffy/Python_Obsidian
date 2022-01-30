#file-method 	
### .readlines()
The `readlines()` method returns a list containing each line in the file as a list item.

Use the hint parameter to limit the number of lines returned.



##### Syntax:
`file.readlines(hint)`

##### Parameter(s):
| Parameter | Desc. |
| --------- | ----- |
| hint    | Optional. If the number of bytes returned exceed the hint number no more lines will be returned. <br> Default -1, which means all lines will be returned.      |

##### Example(s):
```python
f = open("demofile.txt", "r")
print(f.readlines())
```

###### See Also:
[[6.0 -- File Method Index]]
[.readlines()](https://www.w3schools.com/python/ref_file_readlines.asp)