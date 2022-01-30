### Access Modifiers in other Programming Languages
In other programming languages, you can control the "visibility" of an attribute or method of a class using what we call **access modifiers**, special keywords that come with the language.

For example, **Java** has three access modifiers:
- `public` - it has the widest scope. The element can be accessed anywhere in the program.
	Example: `public int a = 5;`
- `protected` - the element is accessible within the same package (you can think of a package as a "folder") or within subclasses in different packages. 
	Example: `protected int a = 5;`
- `private` - the element is only accessible within the same class. 
		Example: `private int a = 5;`

Java also has a default access when no keyword is used. In this case, the element is accessible within the same package.

There can be different access modifiers depending on the programming language. For more information on this topic, [please refer to this article](https://en.wikipedia.org/wiki/Access_modifiers).

###### See Also:
- [[4.4.1 -- Scope & Namespaces]]