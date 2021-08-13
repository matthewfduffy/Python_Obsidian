#string-method
### .format()
Formats specified values in a string.

##### Definition and Usage:
The `format()` method formats the specified value(s) and insert them inside the string's placeholder.
The placeholder is defined using curly brackets: `{}`. Read more about the placeholders in the Placeholder section below.
The `format()` method returns the formatted string. <br>

##### Syntax:
 `string.format(value1, value2...)`

##### Parameter Value(s):
| Parameter         | Description                                                                       |
| ----------------- | --------------------------------------------------------------------------------- |
| value1, value2... | Required. One or more values that should be formatted and inserted in the string. | 

<br>

> Note: The values are either a list of values separated by commas, a key=value list, or a combination of both.
> The values can be of any data type.

<br>

##### Example(s):
```py
txt1 = "My name is {fname}, I'm {age}".format(fname = "John", age = 36)  
txt2 = "My name is {0}, I'm {1}".format("John",36)  
txt3 = "My name is {}, I'm {}".format("John",36)
```


```py
def favorite_song_statement(song, artist):
	return "My favorite song is {} by {}.".format(song, artist)


print(favorite_song_statement("Smooth", "Santana"))
# => "My favorite song is Smooth by Santana"
```
<br>

#### Formatting Types:
Inside the placeholders you can add a formatting type to format the result:
==return to w3 schools for this section==

| Symbol | Behavior                                  |
| ------ | ----------------------------------------- |
| `:<`   | Left aligns the result                    |
| `:>`   | Right aligns the result                   |
| `:^`   | Center aligns the result                  |
| `:=`   | Places the sign to the left most position |
|        |                                           |

##### See Also:
[[2.1.3 -- String Formatting]]
[[2.1.2 -- String Methods Index]]
[.format()](https://www.w3schools.com/python/ref_string_format.asp)