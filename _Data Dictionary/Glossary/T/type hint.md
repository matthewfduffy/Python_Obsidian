## type hints
An annotation that specifies the expected type for a variable, a class attribute, or a function parameter or return value.

Type hints are optional and are not enforced by Python, but they are useful to static type analysis tools and can aid IDEs with code completion and refactoring.

Type hints of global variables, class attributes, and functions (but non local variables) can be accessed using `typing.get_type_hints()`

See Also: 
- [[function annotation]]
#PEP-484