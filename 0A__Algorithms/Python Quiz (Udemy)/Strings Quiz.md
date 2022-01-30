
Considering the following string referenced by the **fact** variable, please select the correct answer to the question below.

`fact = "Romania is the home of the heaviest building in the world, the Palace of Parliament in Bucharest."`

  

1. What is the string method that will turn all lowercase characters to uppercase and vice-versa?
	`fact.swapcase()`
2. Which of the following options will remove all the white spaces in the string?
	`fact.replace(" ", "")`
	
3. What would be the result of `fact.index("s")` ? --> `9`
4. How would you count the number of white spaces in the string using a string method? --> 	`fact.count(" ")`
5. What would be the result of `fact.index("he") * fact.count("P")` ? --> `24`
6. What would be the result of:

`fact.split(" ")[7].upper()` --> `BUILDING`

7. Which of the following options will insert a `%` in between every two letters of **Bucharest** _(do not include the dot at the end)_ ?
			`"%".join(fact.split(" ")[-1].strip("."))`
8. What is the correct result of:
	```py
	a = "Hi"
	b = "Hello"
	((a + b) * 5).count("h")
	
	# 0 b/c "h" != "H"
	```

