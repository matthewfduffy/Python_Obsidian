#string-method 
### .zfill()


##### Definition and Usage:
The `zfill()` method adds zeros (0) at the beginning of the string, until it reaches the specified length.

##### Syntax:
 `string.zfill(len)`

##### Parameter Values:
| Parameter | Description                                                    |
| --------- | -------------------------------------------------------------- |
| len       | Required. A number specifying the desired length of the string | 




If the value of the len parameter is less than the length of the string, no filling is done.

##### Examples:
```python
a = "hello"  
b = "welcome to the jungle"  
c = "10.000"  
  
print(a.zfill(10))  	# 00000hello
print(b.zfill(10))  	# welcome to the jungle
print(c.zfill(10))		# 000010.000

```

###### See Also:
[[2.1.0 -- String Methods Index]]
[.zfill()](https://www.w3schools.com/python/ref_string_zfill.asp)