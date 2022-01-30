## function annotation
An annotation of a [[function]] parameter or return value.

Function annotations are usually used for [[type hint]]s.
For example, this function is expected to take two `int` arguments and is also expected to have an `int` return value:

```py
def sum_two_numbers(a: int, b: int) -> int:
	return a + b
```

See Also: 
- [[variable annotation]]
#PEP-484