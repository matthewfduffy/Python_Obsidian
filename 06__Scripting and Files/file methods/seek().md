#file-method 	
### .seek()
The `seek()` method sets the current file position in a file stream and returns the new position.


##### Syntax:
`file.seek(offset)`

##### Parameter(s):
| Parameter | Desc. |
| --------- | ----- |
| offset    | Required. A number representing the position to set the current file stream position.

##### Example(s):
```python
f = open("demofile.txt", "r")
f.seek(4)
print(f.readline())
```

###### See Also:
[[6.0 -- File Method Index]]
[.seek()](https://www.w3schools.com/python/ref_file_seek.asp)