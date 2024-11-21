Syntax ref out and in in C#
===================================

**Syntax ref**

``ref`` Passes the argument by reference, allowing the method to read and modify the value. The variable must be initialized before being passed.
``ref`` It also changes the semantics if you use with a reference type like a or a . In the method below if you would not use the modifier, “myString” would still be “Original String” after the call due to the immutability of string

**Syntax out**

``out`` Similar to , but the variable doesn't need to be initialized before being passed. The method must assign a value before it returns.
``out`` You find this typical with the “Try” pattern where the return value is a boolean type and the value gets passed via out to the caller.

**Syntax in**

``in`` Passes the argument by reference, but the method can only read the value, not modify it. Useful for performance when passing large structs.

**Summary**

- Use when you want to allow a method to read and modify a value
- Use when you want a method to initialize and return a value
- Use when you want to pass a large struct by reference without allowing modifications.