##  iterator
An object that represents a stream of data. This is different from a *list*, which is also an [[iterable]], but is not an iterator because it is not a stream of data.

a [[generator]] iterator is an object created by a generator function.
Each `yield` temporarily suspends processing, remembering the location execution state (including local variables and pending try-statements.)
When the *generator iterator* resumes, it picks up where it left off (in contrast to functions which start fresh on ever invocation).

Related: [[generator]], [[yield]]
