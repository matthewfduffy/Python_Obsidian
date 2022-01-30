#string-method 
### .translate()


##### Definition and Usage:
The `translate()` method returns a string where some specified characters are replaced with the character described in a dictionary, or in a mapping table.

Use the [[maketrans()]] method to create a mapping table.

If a character is not specified in the dictionary/table, the character will not be replaced.

If you use a dictionary, you must use ascii codes instead of characters.

##### Syntax:
 `string.translate(table)`

##### Parameter Values:
| Parameter | Description                                                                             |
| --------- | --------------------------------------------------------------------------------------- |
| table     | Required. Either a dictionary, or a mapping table describing how to perform the replace | 


##### Examples:
```python
# Use a mapping table to replace "S" with "P":
txt = "Hello Sam!"
mytable = txt.maketrans("S", "P")
print(txt.translate(mytable))		# Hello Pam!


# Use a mapping table to replace many characters:
txt = "Hi Sam!"
x = "mSa"
y = "eJo"
mytable = txt.maketrans(x, y)

print(txt.translate(mytable))		# Hi Joe!

# The third parameter in the mapping table describes characters that you want to remove from the string:

txt = "Good night Sam!"  
x = "mSa"  
y = "eJo"  
z = "odnght"  
mytable = txt.maketrans(x, y, z)  
print(txt.translate(mytable))		# G i Joe!

```

###### See Also:
[[2.1.0 -- String Methods Index]]
[.translate()](https://www.w3schools.com/python/ref_string_translate.asp)