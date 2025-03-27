SOLID
===================================

SOLID tells us how to arrange functions and data structures into classes / modules, and how those classes / modules should be interconnected. SOLID is therefore applied at the mid-level (class / module level).

- There are other sets of principles for the component level and the high-level architecture. We will study these later.

SOLID is not limited OOP. In the context of SOLID, a "class / module" is a grouping of functions and data (all software have this grouping, whether it is called a class a module or something else). We will refer to this grouping as class or a module interchangeably in this part.

- For many languages and teams a module is coded in a single source file, but this doesn't have to be the case.

SOLID goals: produce mid-level software structures that:

- Tolerate change
- Are easy to understand
- Are the basis of components that can be used in many systems (are reusable).



**1. What is Single Responsibility Principle?**

A class should have only one reason to change.

**2. What is Open/Closed Principle?**

Software entities (classes, modules, functions, etc.) should be open for extension but closed for modification.
Changing by adding new code rather than by changing existing code.
Keep the things that change frequently away from things that don't change.

**3. What is Liskov Substitution Principle?**

Subtypes must be substitutable for their base types.

**4. What is Interface Segregation Principle?**

Clients should not be forced to depend on methods they do not use.

**5. What is Dependency Inversion Principle?**

High-level modules should not depend on low-level modules. Both should depend on abstractions.
Abstractions should not depend upon details. Details should depend upon abstractions.



