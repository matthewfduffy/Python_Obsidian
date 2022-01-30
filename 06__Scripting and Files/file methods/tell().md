#file-method 	
### .tell()
The `tell()` method returns the current file position in a file stream.

You can change the current file position with the [[seek()]] method.

A file is seekable if it allows access to the file stream, like the [[seek()]] method.

##### Syntax:
`file.tell()`

##### Example(s):
```python
f = open("demofile.txt", "r")
print(f.readline())
print(f.tell())
```

###### See Also:
[[6.0 -- File Method Index]]
[.tell()](https://www.w3schools.com/python/ref_file_tell.asp)