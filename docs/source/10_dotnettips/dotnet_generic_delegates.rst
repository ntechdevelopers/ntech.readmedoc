Generic Delegates in .Net
===================================

**There are generic delegates.**

But let’s first get an idea of what delegates are.
The simplest way to explain this is to say that delegates are variables holding method signatures.
There are three steps involved while working with delegates:

- Declare
- Create an instance and reference a method
- Invoke

However, defining every delegate using these steps above can lead to performance degradation.
This is where generic delegates step in.
The main difference between classic delegates and them is that you only need to define a generic type parameter or return type.

**Three types are present in C#:**

- Func: It takes 1-16 input parameters and must have one return type
- Action: It also takes 1-16 input parameters but without return type
- Predicate: It takes one input parameter and always has a Boolean return type

LINQ relies on predicates in almost all methods.
They play a crucial role in simplifying code structure and enhancing flexibility.