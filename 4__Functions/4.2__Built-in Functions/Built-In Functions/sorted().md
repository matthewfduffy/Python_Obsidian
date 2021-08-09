#built-in-function 
## sorted()
Use the `sorted()` function to sort an iterable such as a list or a tuple.
-   Strings are sorted alphabetically
-   Numbers are sorted numerically.
-   You may also choose between ascending and descending order.

Here are some examples:

#### Sort strings
```py
numbers = ["C", "A", "B"]  
print(sorted(numbers))

# Output:
['A', 'B', 'C']
```
#### Sort strings in reversed order
```py
numbers = ["C", "A", "B"]  
print(sorted(numbers, reverse=**True**))

# Output:
['C', 'B', 'A']
```
#### Sort numbers
In the examples above, you sorted lists. Let’s sort a tuple of numbers:
```py
numbers = (3, 1, 7)  
print(sorted(numbers))

# Output:
[1, 3, 7]
```