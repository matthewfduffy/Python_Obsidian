#python-keyword 
## global
The `global` keyword is used within a local scope to associate a variable name with a name in the global namespace.

The `global` statement can be used even if the name has not been defined in the global namespace. 
```python
def some_function():  
	global x  
	x = 30 

some_function()
print(x)
```

This would output:
```
30
```

###### See Also:
[[4.4.1 -- Scope & Namespaces]]