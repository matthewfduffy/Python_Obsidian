#file-method 	
### .writable()
The `writable()` method returns `True` if the file is writable, `False` if not.

A file is writable if it is opened using "a" for append or "w" for write.

##### Syntax:
`file.writable()`

##### Example(s):
```python
f = open("demofile.txt", "a")
print(f.writable())
```

###### See Also:
[[6.0 -- File Method Index]]
[.writable()](https://www.w3schools.com/python/ref_file_writable.asp)