## hashable
An [[object]] is hashable if it has:
+ a hash value which never changes during its lifetime --> it needs a `__hash__()` method
+ can be compared to other objects --> it needs an `__eq__()` method

Hashable objects which compare equal must have the same hash value.
Most of Python's [[immutable]] built-in objects are hashable; [[mutable]] containers (e.g. - [[lists]], dictionaries) are not
Immutable containers (e.g. - tuples, frozensets) are only hashable if their elements are hashable.

Objects which are instances of user-defined classes are hashable by default.
They all compare unequal (except with themselves), and their has value is derived from their `id()`