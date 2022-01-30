#python-built-in-function
## eval()
The `eval()` function evaluates the specified expression, if the expression is a legal Python statement, it will be executed.

#### Syntax:
`eval(expression, globals, locals)`

#### Parameter Value(s):
| Parameter  | Desc.                                                |
| ---------- | ---------------------------------------------------- |
| expression | A String; evaluated as Python code                   |
| globals    | Optional. A dictionary containing global parameters. |
| locals.    | Optional. A dictionary containing local parameters.                                                     |


#### Use:
```python
x = 'print(55)'
eval(x)
# 55
```

###### See Also:
- [[2_Built in Functions Index]]
- [eval()](https://www.w3schools.com/python/ref_func_eval.asp)