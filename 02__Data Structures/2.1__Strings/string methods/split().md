#string-method 
### .split()
The `split()` method splits a string into a list.
You can specify the separator, default separator is any whitespace.

Syntax:
`string.split(separator, maxsplit)`

Parameter Values:
| Parameter | Description                                                                                                     |
| --------- | --------------------------------------------------------------------------------------------------------------- |
| separator | Optional. Specifies the separator to use when spliting the string.<br> By default any whitespace is a separator |
| maxsplit  | Optional. Specifies how many splits to do. Default value is -1, which is "all occurrences"                      | 


```python
txt = "hello, my name is Peter, I am 26 years old"  
  
x = txt.split(", ")  
  
print(x)
```

See Also:
[[advanced splitting]]
[[2.1.0 -- String Methods Index]]
[.split()](https://www.w3schools.com/python/ref_string_split.asp)


```python
print("I Love Python".spint())
-------------------------------
['I', 'Love', 'Python']

text = 'cat, dog, cow, lion'
print(text.split(', ', 1))
---------------------------
['cat', 'dog, cow, lion']

```