## **sequence**
An [[iterable]] which supports efficient element access using integer indices via the `__getitem__()` [[special method]] and defines a `__len__()` method that returns the length of the sequence.

Some built-in sequence types are [[lists]], [[strings]], [[tuple]], and [[bytes]]

Note: [[2.4.1 -- Dictionaries]] also supports `__getitem__()` and `__len__()`, but is considered a mapping rather than a sequence because the lookups use arbitrary [[immutable]] keys rather than integers. 

P.53 -> `collections.abc.Sequence`