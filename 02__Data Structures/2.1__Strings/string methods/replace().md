### .replace()
#string-method 

Replace takes two arguments and replaces all instances of the first argument in a string with the second argument.

##### Syntax:
`string.replace(old_value, new_value, count)`

##### Parameter Values:
| Parameter | Description                                                                                                               |
| --------- | ------------------------------------------------------------------------------------------------------------------------- |
| old_value | Required. The string to search for.                                                                                       |
| new_value | Required. The string to replace the old value with.                                                                       |
| count     | Optional. A number specifying how many occurrences of the old value you want to replace. <br> Default is all occurrences. | 

> Note: All occurrences of the specified phrase will be replaced, if nothing else is specified.

##### Basic Example:
```py
txt = "I like bananas"

x = txt.repalce("bananas", "apples")
print(x)
# => I like apples

```

##### Intermediate Example:
```py
with_spaces = "You got the kind of loving that can be so smooth"

with_underscores = with_spaces.replace(' ', '_')

print(with_underscores)
# => You_got_the_kind_of_loving_that_can_be_so_smooth
```


[[2.1.2 -- String Methods Index]]
[.replace()](https://www.w3schools.com/python/ref_string_replace.asp)