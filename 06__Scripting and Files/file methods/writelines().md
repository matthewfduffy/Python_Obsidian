#file-method 	
### .writelines()
The `writelines()` method writes the items of a list to the file where the texts will be inserted depends on the file mode and stream position.

"a" : The text will be inserted at the current file stream position; default at the end of the file.

"w" : The file will be emptied before the text will be inserted at the current file stream position; default is 0



##### Syntax:
`file.writelines(list)`

##### Parameter(s):
| Parameter | Desc.                                                    |
| --------- | -------------------------------------------------------- |
| list      | The list of texts or byte objects that will be inserted. | 

##### Example(s):
```python
f = open("demofile.txt", "a")
f.writelines(["\nSee you soon!", "Over and out."])
f.close()

# Open and read the file after the appending:
f = open("demofile.txt", "r")
print(f.read())
```

###### See Also:
[[6.0 -- File Method Index]]
[.writelines()](https://www.w3schools.com/python/ref_file_writelines.asp)