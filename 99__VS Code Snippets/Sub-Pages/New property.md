`property`

```py
@property
def foo(self):
	"""The foo property."""
	return self._foo
@foo.setter
def foo(self, value):
	self._foo = value
```