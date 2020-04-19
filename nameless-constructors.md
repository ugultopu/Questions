Why are constructors nameless in most programming languages?
============================================================

A constructor is nothing but a "special" method that is executed when a class has been instantiated. Usually there are multiple ways to instantiate a class. Wouldn't it be more readable to mandate/allow the constructors to have names?

Pros
----
- More readable code.
- Would remove the necessity for the first reason of Item 1 of Chapter 2 in Joshua Block's Effective Java (3rd Edition), where;
  - Item 1 is "Consider static factory methods instead of constructors", and the first reason for this is
  - "One advantage of static factory methods is that, unlike constructors, they have names."

Cons
----
- Hard to distinguish the constructor from a regular method. But this shouldn't be an issue because usually (in straight-forward OOP), the only method that returns a value of the type that the method is defined in is the constructor, unless the builder design pattern is being used.
