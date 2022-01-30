# Counter
A _Counter_ is a dict subclass for counting hashable objects. It is a collection where elements are stored as dictionary keys and their counts are stored as dictionary values. Counts are allowed to be any integer value including zero or negative counts. The _Counter_ class is similar to bags or multisets in other languages.

#### Initializing Counter
```python
from collections import Counter

c = Counter()								# a new, empty counter
c = Counter('gallahad')						# a new counter from an iterable
c = Counter({'red': 4, 'blue': 2})			# a new counter from a mapping
c = Counter(cats=4, dogs=8)					# a new counter from keyword args
```

Counter objects support three methods beyond those available for all dictionaries:

##### elements()
Return an iterator over elements repeating each as many times as its count. Elements are returned in the order first encountered. If an element’s count is less than one, `elements()`will ignore it.
```python
c = Counter(a=4, b=2, c=0, d=-2)
sorted(c.elements())
# ['a', 'a', 'a', 'a', 'b', 'b']
```

##### most_common([n])
Return a list of the _n_ most common elements and their counts from the most common to the least. If _n_ is omitted or `None`, `most_common()` returns _all_ elements in the counter. Elements with equal counts are ordered in the order first encountered:
```python
Counter('abracadabra').most_common(3)
#[('a', 5), ('b', 2), ('r',2)]
```

##### subtract([iterable-or-mapping])
Elements are subtracted from an _iterable_ or from another _mapping_ (or counter). Like `dict.update()` but subtracts counts instead of replacing them. Both inputs and outputs may be zero or negative.
```python
c = Counter(a=4, b=2, c=0, d=-2)
d = Counter(a=1, b=2, c=3, d=4)
c.subtract(d)

print(c)
# Counter({'a': 3, 'b': 0, 'c': -3, 'd': -6})
```

##### total()
Compute the sum of the counts.
```python
c = Counter(a=10, b=5, c=0)
c.total()	# 15
```