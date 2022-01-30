#file-method 	
### .write()
The `write()` method writes a specified text to the file where the specified text will be inserted depends on the file mode and stream position.

"a" : The text will be inserted at the current file stream position; default at the end of the file.

"w" : The file will be emptied before the text will be inserted at the current file stream position; default is 0


##### Syntax:
`file.write(byte)`

##### Parameter(s):
| Parameter | Desc.                                          |
| --------- | ---------------------------------------------- |
| byte      | The text or byte object that will be inserted. | 

##### Example(s):
```python
f = open("demofile.txt", "a")
f.write("\nSee you soon!")
f.close()

# Open and read the file after the appending:
f = open("demofile.txt", "r")
print(f.read())
```

###### See Also:
[[6.0 -- File Method Index]]
[.write()](https://www.w3schools.com/python/ref_file_write.asp)