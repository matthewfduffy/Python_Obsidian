#file-method 	
### .flush()
The `flush()` method cleans out the internal buffer.


##### Syntax:
`file.flush()`

##### Example(s):
```python
f = open("demofile.txt", "a")
f.write("No the file has one more line!")
f.flush()
f.write("...and another one!")
```

###### See Also:
[[6.0 -- File Method Index]]
[.flush()](https://www.w3schools.com/python/ref_file_flush.asp)