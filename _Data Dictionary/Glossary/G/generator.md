## Generators
A function which returns a generator [[iterator]]. It looks like a normal function except that it contains [[yield]] expressions for producing a series of values usable in a *for loop* or that can be retrieved one at a time with the `next()` function. 

You can also define [[iterator]]s using [[_Data Dictionary/Glossary/C/class]]es*.



Sample generator function:
```py
def my_range(x):
	i = 0
	while i < x:
		yield i
		i += 1
```

Since this returns an iterator, we can convert it to a list or iterate through it in a loop to view its contents:
```py
for x in my_range(5):
	print(x)
	
""" 
Output:
0
1
2
3
4
"""
```


%%(https://classroom.udacity.com/courses/ud1110/lessons/bbacebc6-406a-4dc5-83f6-ef7ba3371da6/concepts/50247542-7933-4afe-9130-ff1dff429b03)%%
Related: [[iterator]], [[yield]]