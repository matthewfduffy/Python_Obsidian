#file-method 	
### .seekable()
The `seekable()` method returns `True` if the file is seekable, `False` if not.

A file is seekable if it allows access to the file stream, like the [[seek()]] method.

##### Syntax:
`file.seekable()`

##### Example(s):
```python
f = open("demofile.txt", "r")
print(f.seekable())
```

###### See Also:
[[6.0 -- File Method Index]]
[.seekable()](https://www.w3schools.com/python/ref_file_seekable.asp)