#file-method 	
### .truncate()
The `truncate()` method resizes the file to the given number of bytes.

If the size is not specified, the current position will be used


##### Syntax:
`file.truncate(size)`

##### Parameter(s):
| Parameter | Desc.                                                                                                                           |
| --------- | ------------------------------------------------------------------------------------------------------------------------------- |
| size      | Optional. The size of the file (in bytes) after the truncate. <br> Default: none - which means the current file stream position | 

##### Example(s):
```python
f = open("demofile.txt", "a")
f.truncate(20)
f.close()

# open and read the file after the truncate:
f = open("demofile2.txt", "r")
print(f.read())
```

###### See Also:
[[6.0 -- File Method Index]]
[.truncate()](https://www.w3schools.com/python/ref_file_truncate.asp)