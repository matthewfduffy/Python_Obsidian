## dictionary views
The objects returned from `dict.keys()`, `dict.values()`, and `dict.items()` are called *dictionary views*.

They provide a dynamic view on the [[dictionary]]'s entries, whcih means that when the dictionary changes, the view reflects these changes.

To force the dictionary view to become a full list use `list(dictview).`

See Also: [[2.4.1 -- Dictionaries]]