#string-method 
### .casefold()
The `casefold()` method returns a string where all the characters are lower case.

This method is similar to the `[[lower()]]` method, but the `casefold()` method is stronger, more aggressive, meaning that it will convert more characters into lower case, and will find more matches when comparing two strings and both are converted using the `casefold()` method.

##### Example(s):
```py
txt = "Hello, And Welcome To My World!"  
  
x = txt.casefold()  
  
print(x)
```

###### See Also:
[[2.1.2 -- String Methods Index]]
[.casefold()](https://www.w3schools.com/python/ref_string_casefold.asp)