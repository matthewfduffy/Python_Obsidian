## multiple context managers
A [[context manager]] is a special code construct that allow the simple handling of resources (e.g. - files)

Prior to Python 3.10:
```py
# single context manager construct

with open('output.log', 'rw') as fout:  
    fout.write('hello')
```
 
 #pyversion-3-10 Provides Multiple Context managers

Now, with parenthesized context managers, you can use multiple context managers in one `with` block:

```py
with (open('output.log', 'w') as fout, open('input.csv') as fin):  
    fout.write(fin.read())
```

This feature will be useful for bits of code that work with async resources, as you no longer need to have multiple `with` statements.