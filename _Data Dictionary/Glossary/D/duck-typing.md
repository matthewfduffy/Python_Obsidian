## duck-typing
A programming style which does not look at an [[object]]'s type to determine if it has the right interface;
	instead, the [[method]] or [[attribute (database)]] is simply called or used.
	
By emphasizing interfaces rather than specific types, well-designed code improves its flexibility by allowing polymorphic substitution.

Duck-typing avoids tests using `type()` or `isinstance()`; however, it can be complemented with [[abstract base class]]es