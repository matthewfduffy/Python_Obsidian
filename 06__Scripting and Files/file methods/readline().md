#file-method 	
### .readline()
The `readline()` method returns one line from the file.

You can also specify how many bytes from the line to return by using the size parameter.



##### Syntax:
`file.readline(size)`

##### Parameter(s):
| Parameter | Desc. |
| --------- | ----- |
| size      | Optional. The number of bytes from the line to return. <br> Default -1, which means the whole line.      |

##### Example(s):
```python
f = open("demofile.txt", "r")
print(f.readline())
print(f.readline(5))
```

###### See Also:
[[6.0 -- File Method Index]]
[.readline()](https://www.w3schools.com/python/ref_file_readline.asp)