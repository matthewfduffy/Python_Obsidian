#file-method 	
### .fileno()
The `fileno()` method returns the file descriptor of the stream, as a number.

An error will occur if the operator system does not use a file descriptor.

##### Syntax:
`file.fileno()`

##### Example(s):
```python
f = open("demofile.txt", "r")
print(f.fileno())

```

###### See Also:
[[6.0 -- File Method Index]]
[.fileno()](https://www.w3schools.com/python/ref_file_fileno.asp)