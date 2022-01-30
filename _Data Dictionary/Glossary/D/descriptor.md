## descriptor
Any [[object]] which defines the [[method]]s `__get__()`, `__set__()`, or `__delete__()`.

When a [[_Data Dictionary/Glossary/C/class]] [[attribute (database)]] is a descriptor, its special binding behavior is triggered upon attribute lookup.
Normally, using *a.b* to get, set or delete an attribute looks up the object named *b* in the class dictionary for *a*,
	However, if *b* is a descriptor, the respective descriptor method gets called.